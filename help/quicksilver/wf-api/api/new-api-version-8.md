---
content-type: api
navigation-topic: api-navigation-topic
title: API 8版的新功能
description: 這是API 9版新增的資源清單。 如需已對第8版之資源進行更新的清單，請造訪第8版的更新
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 31%

---

# API 8版的新功能

## 新資源

這是API 9版新增的資源清單。 如需已對第8版資源進行更新的清單，請造訪 [API第8版的更新](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| backlogOrder | 客戶 |   |   | bulkCopy  |   | 複製 |
| 色彩 | 迭代  |   |   |   |   | 計數 |
| customerID | lastUpdatedBy |   |   |   |   | DELETE |
| 估計 | opTask |   |   |   |   | 編輯 |
| ID | 專案 |   |   |   |   | GET  |
| isReady | 情節提要父級 |   |   |   |   | 報表 |
| iterationID | 任務 |   |   |   |   | SEARCH |
| lastUpdateDate | 團隊 |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| 名稱 |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| 類型 |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | 計數  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | 報表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**看板板**

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
| 名稱 |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 編輯 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 報表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ProofApprovalStatus

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceDekededHour**

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 新增 |
| 預算小時數 |   |   |   |   |   | 計數 |
| planedDekededHours |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | 編輯 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | 報表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
| 名稱 |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | 編輯 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 報表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**RtfTextNote**

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 報表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### 訂閱

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 訂閱 | 新增 |
|   |   |   |   | removeSubscribers |   | 計數  |
|   |   |   |   | 訂閱數 |   | DELETE |
|   |   |   |   | 取消訂閱 |   | GET |
|   |   |   |   |   |   | 報表 |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### 用戶角色

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| roleID | 角色 |   |   |   |   |   |
| timePercentage | 使用者 |   |   |   |   |   |
| userID |   |   |   |   |   |   |
