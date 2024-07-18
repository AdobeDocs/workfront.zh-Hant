---
content-type: api
navigation-topic: api-navigation-topic
title: API 8版的新增功能
description: 這是API版本9的新資源清單。 如需第8版資源的更新清單，請造訪API第8版的更新
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 27%

---

# API 8版的新增功能

## 新資源

這是API版本9的新資源清單。 如需版本8的資源更新清單，請造訪[API版本8](../../wf-api/api/new-api-version-8-updates.md)的更新

**敏捷工作**

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| backlogOrder | 客戶 |   |   | bulkcopy  |   | 複製 |
| 顏色 | 反複專案  |   |   |   |   | 計數 |
| customerID | lastUpdatedBy |   |   |   |   | DELETE |
| 預估 | op任務 |   |   |   |   | 編輯 |
| ID | 專案 |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | 報告 |
| iterationID | 任務 |   |   |   |   | SEARCH |
| lastUpdateDate | 團隊 |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| 名稱 |   |   |   |   |   |   |
| opTaskId |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| 類型 |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | 計數  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
| 名稱 |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 編輯 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| documentVersionID | documentversion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| 檔案名稱 |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 新增 |
| budgetedHours |   |   |   |   |   | 計數 |
| plannedBudgetedHours |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | 編輯 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
| 名稱 |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 編輯 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 訂閱

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 訂閱者 | 新增 |
|   |   |   |   | removeSubscribers |   | 計數  |
|   |   |   |   | 訂閱次數 |   | DELETE |
|   |   |   |   | 取消訂閱 |   | GET |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 使用者角色

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| roleID | 角色 |   |   |   |   |   |
| timePercentage | 使用者 |   |   |   |   |   |
| userID |   |   |   |   |   |   |
