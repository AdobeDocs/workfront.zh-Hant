---
content-type: api
navigation-topic: api-navigation-topic
title: API 6版的新增功能
description: API 6版的新增功能
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 34%

---

# API 6版的新增功能

## 新物件

### 資源管理員

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| ID | 客戶 |   |   |   |   | 新增 |
| customerID | 專案 |   |   |   |   | 計數 |
| projectID | resourceManager |   |   |   |   | 刪除 |
| resourceManagerID | 範本 |   |   |   |   | Get |
| templateID |   |   |   |   |   | 報告  |
|   |   |   |   |   |   | 搜尋  |


### Ews

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| 檔案名稱 |   |   |   |   | 上傳 |   |
| 控點 |   |   |   |   |   |   |
| 物件代碼 |   |   |   |   |   |   |


### 自訂標籤

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabel | 新增 |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabel | 計數 |
|   |   |   |   | removeCustomLabs |   | 刪除 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | 搜尋 |


## 更新的物件

對現有物件的變更：新增物件只是簡單的列出、移除具有刪除線、對現有物件的變更在表格後面具有附加註記

### 更新

 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

<sup>2</sup> hasFilters屬性已變更為true

 

### 核准

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>日期驗證已新增

<sup>2</sup> NOT_FILTERABLE旗標已新增

 

### 核准流程

|   | 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### 核准步驟

 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

 

### 核准路徑<sup>1</sup>

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| approvedstatus |   |   |   |   |   | 新增 |
| approvedStatusLabs |   |   |   |   |   | 計數 |
| 評論 |   |   |   |   |   | 刪除 |
| enteredById |   |   |   |   |   | 編輯 |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | 報告 |
| isPrivate |   |   |   |   |   | 搜尋 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| 名稱<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已變更為可報告

<sup>2</sup>已新增長度上限驗證器

 

### 工作服務物件

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workitemstatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup>日期驗證已新增

<sup>2</sup> Not_Filterable旗標已新增

 

### 指派

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProject |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignuserfromprojects |   |   |

{style="table-layout:auto"}

 

### 基線 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable旗標已新增

 

### 基準線任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable旗標已新增

 

### 計費記錄

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已新增NO_TIME欄位旗標

### 待執行工作事件 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### 類別 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

自訂列舉 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatures |   |
|   |   |   |   |   | taskGroupStatures |   |

{style="table-layout:auto"}

 

檔案 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

匯率 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| 速率<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已將8的PRECISION驗證器變更為9

 

### 整合

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 日誌輸入項目

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

 

### Optask （問題）<sup>1</sup> 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已標示為可還原

<sup>2</sup> Not_Filterable旗標已新增

 

### 專案<sup>1</sup> 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 工作 |   |   |   |   |   |   |
| 所需工作 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>標示為可還原且資源可管理

<sup>2</sup> Not_Filterable旗標已新增

 

### 工作<sup>1</sup>

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已標示為可還原

<sup>2</sup> AT_DATE_YEAR_BEFORE驗證器已新增

<sup>3</sup> Not_Filterable旗標已新增

 

### 團隊

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### 範本<sup>1</sup> 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>標示為可還原且資源可管理

### 範本任務<sup>1</sup> 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>已標示為可還原

<sup>2</sup> Not_Filterable旗標已新增

 

### 使用者

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH違規者

 

### 使用者附註

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup>可能的值已變更

<sup>2</sup>的篩選器已變更為`[true]`

 

### 宣告

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
