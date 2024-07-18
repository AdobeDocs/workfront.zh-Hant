---
content-type: api
navigation-topic: api-navigation-topic
title: API第8版的更新
description: 檢視API 8版的更新。
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 31%

---

# API第8版的更新

## 已更新的資源

此版本的Adobe Workfront API已更新下列現有資源。 若要檢視版本8的新資源，請參閱[API版本8](../../wf-api/api/new-api-version-8.md)的新增功能。 對資源所做的變更會以下列方式表示：

* 新增內容只會列出
* 移除以刪除線文字表示
* 變更會記在表格後面的註記中

### AccessRequest

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| 動作<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### AccessRule<sup>1</sup> 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>旗標已移除：可報告\
<sup>2</sup>可能值的變更

### 核准

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 敏捷工作  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更\
<sup>2</sup>標幟已新增：動態、LAZY_READ和NOT_GROUPABLE

### 指派

|   |   |   |   | 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOntasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### 客戶

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | Getpackagingoptionvalue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 客戶喜好設定

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| 名稱<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 檔案核准

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| 識別碼<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>標幟已新增： NOT_FILTERABLE

### 檔案版本

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### 群組

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   | 擁有者 |   |   |   |   |

{style="table-layout:auto"}

### Hourtype

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>標幟已新增： NOT_FILTERABLE

### 反覆項目

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   | 移動劇本 |   |   |

{style="table-layout:auto"}

### 喜歡

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### 備註

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### Op 任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 敏捷工作  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | 反複專案 |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| 預估 |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 專案組合

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 方案

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 專案

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | resourcePools |   |   | defaultShowTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### ProofApproval

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| approverID | 核准者 |   |   |   |   |   |
| documentVersionID | documentversion |   |   |   |   |   |
| 識別碼<sup>1</sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>標幟已新增： NOT_FILTERABLE

### QueueDef

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestorForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 費率

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| 名稱 |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### 保留時間

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| extRefId |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| 專案優先順序 |   |   |   |   |   |   |

{style="table-layout:auto"}

### 任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 敏捷工作  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 團隊

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| 敏捷方法 |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### 範本

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### 範本任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

更新

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 使用者

|   |   | 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | 使用者群組 |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### 使用者附註

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 工作

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | 敏捷工作  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更\
<sup>2</sup>標幟已新增：動態、LAZY_READ和NOT_GROUPABLE
