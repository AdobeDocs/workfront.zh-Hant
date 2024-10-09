---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查詢範例
description: 您可以使用查詢範例來熟悉特定型別查詢的語法和結構。
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Workfront Data Connect查詢範例

為協助您更妥善運用Workfront Data Connect資料，本頁包含基本範例查詢，讓您熟悉特定型別查詢的語法和結構。

## 自訂資料查詢

此範例示範如何撰寫查詢以傳回Workfront中的自訂資料，例如自訂表單和自訂欄位。

### 案例：

您的組織使用名為Finance Integration的自訂表單。 此表單會附加至每個專案，並包含下列欄位：

* **業務單位** — 包含字串的自訂欄位。
* **ProjectID** — 包含數字字串的自訂欄位。
* **展開的專案名稱** — 將商業單位、專案ID和原生Workfront專案名稱的值串連為單一字串的計算自訂資料欄位。

您需要將此資訊包含在針對Data Connect的查詢的回應中。 資料湖中記錄的自訂資料值包含在標題為`parametervalues`的欄中。 此欄會儲存為JSON物件。

### 查詢：

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

### 回應：

上述查詢會傳回下列資料：

* `projectid` — 原生Workfront專案ID
* `parametervalues` — 儲存JSON物件的欄
* `name` — 原生Workfront專案名稱
* `Business Unit` - `parametervalues`物件中包含的自訂資料值
* `Project ID` - `parametervalues`物件中包含的自訂資料值
* `Expanded Project Name` - `parametervalues`物件中包含的自訂資料值

### 說明：

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

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
