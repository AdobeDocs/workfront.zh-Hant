---
content-type: api
navigation-topic: api-navigation-topic
title: API 10版的新增功能
description: 已更新的資源
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
TQID: https://experienceleague.adobe.com/7paMh3l4zsoBaafv6U6pp1M-SQjk-kdmSho9GYa15SU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 484
ht-degree: 55%

---

# API 10版的新增功能

* [新資源](#new-resources)
* [已更新資源](#updated-resources)
* [已移除的資源](#removed-resources)

## 新資源 {#new-resources}

### 活動記錄

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | 新增 |
|   |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 行事曆專案

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
|   |   |   |   |   |   | 計數  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 編輯  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 報告  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 報告  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### ExternalAuthToken

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
|   |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | 編輯  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | 報告  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| customerID | 客戶 |   |   |   |   |   |
| groupID | 群組 |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| 工作限制 |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| customerID | 客戶 |   |   |   |   | 新增 |
| edTime | 使用者 |   |   |   |   | 計數 |
| firstDayOfWeek |   |   |   |   |   | DELETE |
| ID |   |   |   |   |   | 編輯 |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | 報告 |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**已更新資源**

此版本的Workfront API已更新下列現有資源。 對資源所做的變更如下：

* 新增內容只會列出
* 移除以刪除線文字表示
* 變更會列在表格後面的註記中

### 核准

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| 優先色彩  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| 專案淨值  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### 指派

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`新增的驗證器LESS_THAN_EQUAL

### BudgetedHour

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 客戶喜好設定

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| 名稱`<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### DocMetadataLinkGroup

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### 文件

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### 檔案請求

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

檔案版本

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

費用

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 群組

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### Op 任務

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| 優先色彩 |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>型別從Null變更為布林值

### PortalSection

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### 專案組合

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### 專案

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| 專案淨值 |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### ProofApproval

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### 費率

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>已新增驗證器貨幣

### 任務

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| 優先色彩  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 團隊

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已新增驗證器LESS_THAN

### 團隊指派

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 團隊任務

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 時程表

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### 更新

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup>變更為possibleValues

### 使用者

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### 使用者附註

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>變更為possibleValues

### 工作

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| 優先色彩  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>型別從Null變更為布林值

## 已移除的資源 {#removed-resources}

### ResourceBudgetedHour

| 欄位 | 參考資料 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 新增  |
| budgetedHours |   |   |   |   |   | 計數  |
| ID |   |   |   |   |   | DELETE  |
| plannedBudgetedHours |   |   |   |   |   | 編輯  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | 報告  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
