---
content-type: api
navigation-topic: api-navigation-topic
title: API 9版的新功能
description: 這是API 9版最新的資源清單，若要查看9版資源的更新清單，請造訪API 9版的更新
author: Becky
feature: Workfront API
exl-id: 29d922f4-f4c6-45e5-b9fa-43e2068ec66d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 25%

---

# API 9版的新功能

## 新資源

這是API 9版最新的資源清單，若要查看9版資源已進行的更新清單，請造訪 [API第9版的更新](../../wf-api/api/new-api-version-9-updates.md)

### AccessLevel

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `accessRestrictions` | `customer` | `accessLevelPermissions` |  |  |  | `ADD` |
| `customerID` | `lastUpdatedBy` | `accessRulePreferences` |  |  |  | `COPY` |
| `description` |  |  |  |  |  | `COUNT` |
| `descriptionKey` |  |  |  |  |  | `DELETE` |
| `entryDate` |  |  |  |  |  | `EDIT` |
| `extRefID` |  |  |  |  |  | `GET` |
| `fieldAccessPrivileges` |  |  |  |  |  | `REPLACE` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isAdmin` |  |  |  |  |  | `SEARCH` |
| `isUnsupportedWorkerLicense` |  |  |  |  |  |   |
| `lastUpdatedByID` |  |  |  |  |  |   |
| `lastUpdatedDate` |  |  |  |  |  |  |
| `licenseType` |  |  |  |  |  |  |
| `name` |  |  |  |  |  |  |
| `nameKey` |  |  |  |  |  |  |
| `securityModelType` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessLevelPermissions

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `coreAction` |  |  |  |  |  |   |
| `forbiddenActions` |  |  |  |  |  |   |
| `ID` |  |  |  |  |  |   |
| `isAdmin` |  |  |  |  |  |   |
| `objObjCode` |  |  |  |  |  |  |
| `secondaryActions` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessRulePreference

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### DekededHour

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `allocationDate` |  |  |  |  |  | `ADD` |
| `budgetedHours` |  |  |  |  |  | `DELETE` |
| `GUID` |  |  |  |  |  | `GET` |
| `plannedBudgetedHours` |  |  |  |  |  | `SEARCH` |
| `projectID` |   |   |   |   |   |   |
| `roleID`  |   |   |   |   |   |   |
| `userID`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 日曆門戶節

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `calendarInfoID` | `customer` |  | `displayDescription` |  |  | `ADD` |
| `customerID` | `enteredBy` |  | `displayName` |  |  | `COPY` |
| `enteredByID` |  |  |  |  |  | `COUNT` |
| `entryDate` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `name` |  |  |  |  |  | `SEARCH` |
| `objID`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### 日曆節

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `calendarID` | `customer` | `filters` |  | `getConcatenatedExpressionForm` |  | `ADD` |
| `calEvents` |  |  |  | `getPrettyExpressionForm` |  | `COUNT` |
| `color` |  |  |  |  |  | `DELETE` |
| `customerID` |  |  |  |  |  | `EDIT` |
| `duration` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `milestone` |  |  |  |  |  | `SEARCH` |
| `name`  |   |   |   |   |   |   |
| `plannedDate` |   |   |   |   |   |   |
| `startDate` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ExternalSection

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `appGlobalID` | `customer` |  | `displayDescription` | `calculateURL` |  | `ADD` |
| `calculatedURL` | `enteredBy` |  | `displayName` | `calculateURLS` |  | `COPY` |
| `customerID` | `view` |  | `linkedCustomersMM` |  |  | `COUNT` |
| `description` |  |  | `linkedUsersMM` |  |  | `DELETE` |
| `descriptionKey` |  |  |  |  |  | `EDIT` |
| `enteredByID` |  |  |  |  |  | `GET` |
| `entryDate` |  |  |  |  |  | `REPORT` |
| `extRefID` |  |  |  |  |  | `SEARCH` |
| `frame`  |   |   |   |   |   |   |
| `friendlyURL`  |   |   |   |   |   |   |
| `globalUIKey`  |   |   |   |   |   |   |
| `height`  |   |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| `name`  |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `objID`  |   |   |   |   |   |   |
| `objInterface`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |
| `scrolling` |   |   |   |   |   |   |
| `url` |   |   |   |   |   |   |
| `viewID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

這份清單分成兩半。 要查看下半部分，請參閱 [API 9版的新功能（續）](../../wf-api/api/new-api-version-9-continue.md). 若要檢視第9版更新的清單，請造訪 [API第9版的更新](../../wf-api/api/new-api-version-9-updates.md)
