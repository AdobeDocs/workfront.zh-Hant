---
content-type: api
navigation-topic: api-navigation-topic
title: API 6版的新功能
description: API 6版的新功能
author: Becky
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 42%

---

# API 6版的新功能

## 新對象

### 資源管理員

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID | 客戶 |   |   |   |   | 新增 |
| customerID | 專案 |   |   |   |   | 計數 |
| projectID | resourceManager |   |   |   |   | 刪除 |
| resourceManagerID | 範本 |   |   |   |   | 取得 |
| templateID |   |   |   |   |   | 報告  |
|   |   |   |   |   |   | 搜尋  |


### Ews

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | 上傳 |   |
| 手柄 |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### 自訂標籤

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | 新增 |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | 計數 |
|   |   |   |   | removeCustomLabel |   | 刪除 |
|   |   |   |   |   |   | 取得 |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | 搜尋 |


## 更新的物件

對現有對象的更改：「添加」(additions)僅列出，「移除」(removes)為「刪除」(striketh)，「現有」(existing)的更改在表格後面附加一個附註

### 更新

 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹可能值的變更

² hasFilters屬性已變更為true

 

### 核准

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹新增日期驗證

²已添加NOT_FILTERABLE標誌

 

### 核准流程

|   | 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 核准步驟

 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹可能值的變更

 

### 批准路徑¹

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 新增 |
| approvedStatusLabel |   |   |   |   |   | 計數 |
| 註解 |   |   |   |   |   | 刪除 |
| enteredByID |   |   |   |   |   | 編輯 |
| entryDate |   |   |   |   |   | 取得 |
| globalPathID |   |   |   |   |   | 報告 |
| isPrivate |   |   |   |   |   | 搜尋 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| 名稱² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹變更為可報告

²新增最大長度驗證器

 

### 工作服務對象

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

¹新增日期驗證

²已添加不可篩選標籤(_F)

 

### 指派

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 基準線 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹已添加不可篩選標籤(_F)

 

### 基準線任務

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹已添加不可篩選標籤(_F)

 

### 付費記錄

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹新增NO_TIME欄位標幟

### 燃耗事件 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### 類別 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

自訂枚舉 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style=&quot;table-layout:auto&quot;}

 

文件 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

匯率 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| 速率¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹將8版的PRECISION驗證器更改為9版

 

### 整合

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 日誌輸入項目

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹可能值的變更

 

### Optask（問題）¹ 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹標籤為可還原

²已添加不可篩選標籤(_F)

 

### 專案¹ 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 工作 |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹標籤為可還原和資源可管理

²已添加不可篩選標籤(_F)

 

### 任務¹

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹標籤為可還原

²新增AT_DATE_YEAR_BEFORE驗證器

³已添加不可篩選標籤(_F)

 

### 團隊

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### 範本¹ 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹標籤為可還原和資源可管理

### 範本任務¹ 

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹標籤為可還原

²已添加不可篩選標籤(_F)

 

### 使用者

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ MAX_LENGTH違規者

 

### 用戶注釋

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹可能的值已更改

²已將篩選器變更為 `[true]`

 

### 宣告

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
