---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect查詢範例
description: 您可以使用查詢範例來熟悉特定型別查詢的語法和結構。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Workfront Data Connect查詢範例

為協助您更妥善運用Workfront Data Connect資料，本頁包含基本範例查詢，讓您熟悉特定型別查詢的語法和結構。

## 自訂資料查詢

此範例示範如何撰寫查詢以傳回Workfront中的自訂資料，例如自訂表單和自訂欄位。

### 案例：

您的組織PeopleSoft會使用名為Finance Integration的自訂表單。 此表單會附加至每個專案，並包含下列欄位：

* **PeopleSoft業務單位** — 包含字串的自訂欄位。
* **PeopleSoft ProjectID** — 包含數字字串的自訂欄位。
* **展開的專案名稱** — 將PeopleSoft Business Unit、PeopleSoft ProjectID的值及原生Workfront專案名稱串連為單一字串的計算自訂資料欄位。

您需要將此資訊包含在針對Data Connect的查詢的回應中。 資料湖中記錄的自訂資料值包含在標題為`parameterValues`的欄中。 此欄會儲存為JSON物件。

### 查詢：

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:PeopleSoft Business Unit" :: int as PeopleSoftBusinessUnit,
    parametervalues:"DE:PeopleSoft Project ID" :: int as PeopleSoftProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 回應

上述查詢會傳回下列資料：

* `projectid` — 原生Workfront專案ID
* `parametervalues` — 儲存JSON物件的欄
* `name` — 原生Workfront專案名稱
* `PeopleSoft Business Unit` - `parametervalues`物件中包含的自訂資料值
* `PeopleSoft Project ID` - `parametervalues`物件中包含的自訂資料值
* `Expanded Project Name` - `parametervalues`物件中包含的自訂資料值

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
