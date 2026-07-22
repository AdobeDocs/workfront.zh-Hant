---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查詢範例
description: 您可以使用查詢範例來熟悉特定型別查詢的語法和結構。
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
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

查詢使用Data Connect的變更事件追蹤功能。它會判斷事件觸發之新狀態值與先前事件不同之事件的日期。 

從內到外檢查查詢： 

1. 計算先前狀態不同的記錄： 
   * 對於每個變更事件，請使用lag()函式來識別狀態的上一個值。 

2. 僅篩選已變更的記錄： 

   * 在步驟1中從計算中選取記錄，其中先前狀態!=目前狀態。 

3. 以天為單位計算開始/結束有效時間戳記及持續時間： 

   * `<status_begin_effective_timestamp>`：已在步驟2中計算。 

   * `<status_end_effective_timestamp>`：根據下一個(lead())計算。 `<status_begin_effective_timestamp>`：僅在`<status_begin_effective_timestamp>`不是NULL時顯示狀態。 
   * `<status_duration_days>`： `<status_begin_effective_timestamp>`與`<status_end_effective_timestamp>`之間的資料差異。 

>[!NOTE]
>
>建議您在PowerBI或Tableau中使用此查詢作為自己的「檢視」。如果要從`<object>_event view`引進其他欄位，請將此查詢的輸出連線回`<object>_event view`。連線欄位將如下： <br>
>若為projects_event： 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Planning：單一記錄型別查詢

此範例示範如何查詢Workfront Planning資料，以取得儲存在Data Connect資料湖中的單一記錄型別。

### 情境

您的組織使用Workfront Planning來追蹤行銷活動。 每個行銷活動記錄包含名稱、狀態、開始日期、結束日期和擁有者。 您想要提取所有作用中行銷活動的清單及其重要詳細資訊，以用於控制面板。

* Planning記錄型別資料儲存在PLANNINGRECORD_CURRENT檢視中。
* 每一列代表單一記錄，而所有欄位值都儲存在名為FIELD_VALUES的JSON欄中。
* 記錄型別由RECORDTYPEID欄識別。
* 記錄的工作區由WORKSPACEID欄（或人類可讀篩選器的WORKSPACENAME欄）識別。

### 查詢

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### 回應

上述查詢會傳回下列資料：

* **recordid**：行銷活動的唯一Planning記錄ID。
* **campaign_name**：從FIELD_VALUES JSON物件擷取的促銷活動名稱。
* **campaign_status**：行銷活動的目前狀態。
* **start_date**：行銷活動的開始日期，已轉換為日期資料型別。
* **end_date**：行銷活動的結束日期，已轉換為日期資料型別。
* **所有者**：指派為行銷活動擁有者的使用者或團隊名稱。

### 解釋

Data Connect中的Planning記錄共用單一表格結構，無論記錄型別為何。 RECORDTYPEID欄用於將查詢的範圍設定為特定的記錄型別 — 在此例中為「促銷活動」。 將`<your_campaign_record_type_id>`取代為您要查詢的記錄型別ID，可在Workfront Planning記錄型別設定中或透過查詢RECORDTYPE_CURRENT找到。

欄位值會儲存為FIELD_VALUES欄中的JSON物件，並使用用於自訂表單資料的相同冒號標籤語法來存取：

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

欄位名稱參照必須與Planning記錄型別欄位組態中定義的欄位名稱完全相符，包括大寫、間距和表情符號。

>[!NOTE]
>
>在Workfront Planning中檢視記錄型別時，可在URL中找到Planning記錄型別ID。 它是以「Rt...」開頭的URL路徑。 在Data Connect中，也可以使用下列SQL呼叫找到記錄型別：
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning：連線記錄型別查詢

此範例示範如何跨兩個連線的Planning記錄型別（父記錄型別及其連線的記錄型別）查詢資料。

### 情境

您的組織會將Campaign記錄連結至Workfront Planning中的策略記錄。 您想要產生一份報告，顯示每個行銷活動及其相關策略的重要詳細資訊。 他們特別想要顯示策略名稱、策略優先順序和預算分配，以便領導可以檢閱依策略組織的行銷活動活動。

在「資料連線」中，原生Planning記錄型別之間的連線會直接儲存在PLANNINGRECORD_CURRENT的FIELD_VALUES_RAW資料欄。 對於名為「戰術」的參考欄位，值是連線記錄物件的JSON陣列，每個物件都包含具有連線記錄的RECORDID的id屬性。 使用Snowflake的LATERAL FLATTEN將此陣列展開為列，並聯結至連線的記錄型別。

### 查詢

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### 回應

上述查詢會傳回下列資料：

* **campaign_id**：行銷活動的唯一Planning記錄ID。
* **campaign_name**：行銷活動紀錄的名稱。
* **campaign_status**：行銷活動的目前狀態。
* **tactics_name**：連線的Tactics記錄的名稱。
* **strategic_priority**：來自連線策略記錄的Strategic Priority欄位值。
* **budget_allocation**：來自連線策略記錄的「預算分配」欄位值，已轉型為浮點數。

### 說明 — 修改的KP

原生Planning記錄型別之間的連線儲存在REFERENCE_CURRENT聯結表格中。  REFERENCE_CURRENT聯結表格用於RecordType之間的聯結。   在RecordType之間連線時，應該使用TO_RECORDID欄位。

PLANNINGRECORD檢視表中的REFERENCE_ID欄位包含適用於該計畫記錄的所有REFERENCEID欄位清單。 您可以使用與field_value相同的JSON標籤法來存取ID。

```
<reference_ids>:"<reference_name>"::text
```

REFERENCE_CURRENT檢視包含一或多個記錄，其中TO_RECORDID指向PLANNINGRECORD_*檢視中的其他計畫`recordId`欄位。

若要將另一個REFERENCE欄位聯結至其他計畫記錄，則上述查詢中會加入相同的聯結至REFERENCE_CURRENT與PLANNINGRECORD_*的模式。


## Planning：聯結至Workfront工作流程資料查詢的記錄型別

此範例示範如何使用Planning的原生連線功能（其將外部物件參考儲存在REFERENCE_CURRENT檢視中），將Workfront Planning記錄型別聯結至原生Workfront Workflow物件（在此例中為Project）。

### 情境

貴組織使用Planning的原生連線功能，將Workfront Planning中的Campaign記錄連線至Workfront專案。 您想要產生一份合併報告，顯示行銷活動詳細資訊以及連結專案的即時執行資料（特別是專案的目前完成百分比、計畫完成日期和指派的專案所有者），以便行銷活動經理可以追蹤傳遞進度，而不離開其Planning工作區內容。

### 查詢

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### 回應

上述查詢會傳回下列資料：

* **campaign_id**：行銷活動的唯一Planning記錄ID。
* **campaign_name**：行銷活動紀錄的名稱。
* **campaign_status**：來自Planning的行銷活動目前狀態。
* **linked_project_id**：來自REFERENCE_CURRENT.TO_EXTERNALID的Workfront專案識別碼，可識別已連線的Workfront專案。
* **project_name**：來自PROJECTS_CURRENT的原生Workfront專案名稱。
* **project_percent_complete**：專案目前的完成百分比值。
* **project_planned_completion**：已連結Workfront專案的計畫完成日期。
* **project_owner_id**：專案所有者的Workfront使用者ID。
* **project_owner_name**：專案所有者的顯示名稱，已加入USERS_CURRENT加以解析。

### 解釋

從Planning記錄型別到原生Workfront Workflow物件的連線會儲存在REFERENCE_CURRENT中。 此檢視中的每一列代表一個方向連結：TO_EXTERNALID儲存連線的Workfront物件識別碼。 代表Workfront連線的列由`TO_EXTERNALCONNECTIONNAME = 'workfront'`和對應至Workfront物件型別的API程式碼的TO_EXTERNALOBJECTNAME值（例如，專案的PROJ）識別。

PLANNINGRECORD表格中的REFERENCE_ID欄包含適用於該記錄的所有REFERENCEID欄位清單。  您可以使用與field_value相同的JSON標籤法來存取ID。\
PLANNINGRECORD_CURRENT中的單一REFERENCE_ID可能包含REFERENCE_CURRENT表格中的一或多個參照連結，這些連結會連結至Workfront表格中特定物件型別的物件。

```
<reference_ids>:"<reference_name>"::text
```

請注意，Planning檢視(PLANNINGRECORD_CURRENT、REFERENCE_CURRENT)位於WORKFRONT.PLANNING架構中，而原生Workfront工作流程檢視（PROJECTS_CURRENT、USERS_CURRENT等）位於 位於WORKFRONT.WF結構描述中。 跨結構描述聯結需要完整的資料表名稱。

查詢會執行三個聯結：

1. **參考資料表** REFERENCE_CURRENT的Planning記錄已在`TO_RECORDID = c.RECORDID`上聯結，以尋找源自每個Campaign記錄的所有連線。 `TO_EXTERNALCONNECTIONNAME = 'workfront'`和`TO_EXTERNALOBJECTNAME = 'PROJ'`上的篩選器會將結果縮小為專門表示與Workfront專案的連線的列。
1. **參考資料表至Workfront專案：** TO_EXTERNALID儲存已連線專案的原生Workfront projectid。 此專案已直接加入`PROJECTS_CURRENT.projectid`以擷取即時專案資料。
1. **給使用者的專案：** USERS_CURRENT的LEFT JOIN將專案上的ownerid外部索引鍵解析為人類可讀的名稱。 這裡使用LEFT JOIN，因此沒有指派擁有者的專案仍會包含在結果中。

>[!NOTE]
>
>當聯結至Planning外部的表格時，請勿使用查詢中的TO_RECORDID欄位。  連結至外部表格時不需要此專案。
>
>此模式可套用至Planning支援連線的任何Workfront Workflow物件（例如「專案」、「產品組合」或「程式」），方法是將TO_EXTERNALOBJECTNAME篩選器變更為適當的物件API程式碼（例如「產品組合」的PORT或「程式」的PRGM），並加入對應的WORKFRONT.WF表格。 如需每種物件型別的正確表格和ID欄名稱，請參閱Workfront Data Connect資料字典。

若要將另一個REFERENCE欄位聯結到其他外部記錄，與聯結到REFERENCE_CURRENT和Workfront工作流程檢視的模式相同，將新增到上述查詢。

透過多次聯結至REFERENCE_CURRENT表格並使用適當的聯結模式，可在相同查詢中聯結外部與Planningrecord值。


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
