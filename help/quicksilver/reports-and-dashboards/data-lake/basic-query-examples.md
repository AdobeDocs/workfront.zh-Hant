---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查詢範例
description: 您可以使用查詢範例來熟悉特定型別查詢的語法和結構。
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Workfront Data Connect查詢範例

為協助您更妥善運用Workfront Data Connect資料，本頁包含基本範例查詢，讓您熟悉特定型別查詢的語法和結構。

## 自訂資料查詢

此範例示範如何撰寫查詢以傳回Workfront中的自訂資料，例如自訂表單和自訂欄位。

### 情境

您的組織使用名為Finance Integration的自訂表單。 此表單會附加至每個專案，並包含下列欄位：

* **業務單位**：包含字串的自訂欄位。
* **ProjectID**：包含數字字串的自訂欄位。
* **展開的專案名稱**：將商業單位、專案ID和原生Workfront專案名稱的值串連為單一字串的計算自訂資料欄位。

您需要將此資訊包含在針對Data Connect的查詢的回應中。 資料湖中記錄的自訂資料值包含在標題為`parametervalues`的欄中。 此欄會儲存為JSON物件。

### 查詢

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 回應

上述查詢會傳回下列資料：

* `projectid`：原生Workfront專案識別碼。
* `parametervalues`：儲存JSON物件的資料行。
* `name`：原生Workfront專案名稱。
* `Business Unit`： `parametervalues`物件中包含的自訂資料值。
* `Project ID`： `parametervalues`物件中包含的自訂資料值。
* `Expanded Project Name`： `parametervalues`物件中包含的自訂資料值。

### 解釋

查詢`parametervalues` JSON物件時，每個自訂資料欄位都可透過下列專案以欄的形式存取：

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>`是正在查詢之資料表中的JSON物件名稱。 若是自訂資料，一律為`parametervalues`。
* `<parameter_name>`是在表單設定工具中找到的`parametername`字串，雖然它可能並不總是符合這個值。

>[!NOTE]
>
>如果引數名稱在Workfront表單設定工具中變更，則會在JSON物件中呈現為新欄。 因此，我們建議在表單設定工具中建立欄後，不要變更其名稱。 不過，標籤可以變更，而不會影響JSON物件。
>
>如果引數名稱的文字字串不正確，欄將傳回NULL值，而不是錯誤。

* `<data_type>`會將從JSON物件傳回的值轉換為適合欄位的資料型別。 為傳回的值選擇不相容的資料型別會導致資料型別不符錯誤。 可能的資料型別包括：

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` （例如，`Number(32,4)`會傳回1234.0987）
   * `date`
   * `timestamp`

* `<column_name>`是您為每個自訂資料行建立的標籤。

>[!NOTE]
>
>只有已在表單中指派值的引數才會包含在JSON物件中。 如果表單上的自訂資料欄位為空，將不會顯示。

## 狀態查詢中的時間

此範例示範如何測量專案在先前指派狀態中逗留的時間。 它可以很輕鬆地調整以測量狀態中的任務或問題時間，也可以調整以測量物件套用了任何其他屬性（包括自訂資料值）的時間長度。

### 情境

您的組織領導認為您在工作生命週期的每個階段都花太多時間。 建議改善程式之前，建議您建立基線測量，測量專案狀態在一段時間內變更的頻率，以及專案處於任何指定狀態的天數。

您即將使用PROJECTS_EVENT資料檢視，針對專案物件提取每個狀態變更的清單。 您將比較新狀態與先前狀態、取得先前指派狀態的有效時間範圍，然後計算該狀態所花費的天數。

使用每個專案每個狀態所花時間的原始輸出，您可以開始建立視覺效果或進一步彙總資料，以按狀態、專案型別或一年時間建立狀態持續時間平均值。 然後，此基準會被用來設定基準，以符合領導層的期望，供您衡量。

下列查詢使用Data Connect PROJECTS_EVENTS資料檢視來比較每個專案狀態變更事件並顯示狀態中的時間。

### 查詢

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### 回應

上述查詢會傳回下列資料：

* `PROJECTID`：與狀態變更事件相關聯的Workfront專案識別碼。
* `PROJECT_NAME`： Workfront專案名稱。
* `PREVIOUS_STATUS`：專案在變更前的狀態。
* `STATUS`：變更後的專案狀態。
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`：設定先前狀態時的變更事件時間戳記。
* `STATUS_END_EFFECTIVE_TIMESTAMP`：設定更新狀態值時的變更事件時間戳記。
* `STATUS_DURATION_DAYS`：結束有效時間戳記與開始有效時間戳記之間的差異（以天為單位）。

### 解釋

查詢使用Data Connect的變更事件追蹤功能。  它會判斷觸發事件的日期，該事件的新狀態值與先前的事件不同。 

從內到外檢查查詢： 

1. 計算先前狀態不同的記錄： 
   * 對於每個變更事件，請使用lag()函式來識別狀態的上一個值。 

2. 僅篩選已變更的記錄： 

   * 在步驟1中從計算中選取記錄，其中先前狀態！=目前狀態。 

3. 以天為單位計算開始/結束有效時間戳記及持續時間： 

   * `<status_begin_effective_timestamp>`：已在步驟2中計算。 

   * `<status_end_effective_timestamp>`：根據下一個(lead())計算。 `<status_begin_effective_timestamp>`：僅在`<status_begin_effective_timestamp>`不是NULL時顯示狀態。 
   * `<status_duration_days>`： `<status_begin_effective_timestamp>`與`<status_end_effective_timestamp>`之間的資料差異。 

>[!NOTE]
>
>建議您在PowerBI或Tableau中使用此查詢作為自己的「檢視」。  如果您要從`<object>_event view`引進其他欄位，請將此查詢的輸出連線回`<object>_event view`。  加入欄位會如下所示： <br>
>&#x200B;>若為projects_event： 
>&#x200B;>`From projects_event p`
>&#x200B;>`Join <above query> c on c.projectid = p.projectid  `
>&#x200B;>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
