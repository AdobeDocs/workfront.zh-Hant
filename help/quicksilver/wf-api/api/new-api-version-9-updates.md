---
content-type: api
navigation-topic: api-navigation-topic
title: API第9版的更新
description: 更新的資源
author: Becky
feature: Workfront API
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 47%

---

# API第9版的更新

## 更新的資源

此版本的Adobe Workfront API已更新下列現有資源。 若要檢視第9版的新資源，您可以造訪 [API 9版的新功能](../../wf-api/api/new-api-version-9.md) 和 [API 9版的新功能（續）](../../wf-api/api/new-api-version-9-continue.md). 對資源的變更會以下列方式表示：

* 新增項目會列出
* 移除項目會以字串文字表示
* 表格後面的注釋中會列出更改

### AgileWork

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |  |  |  |  |  |
| `taskID`<sup>2</sup> |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹已移除標幟：可報告\
²已移除標幟：NOT_GROUPABLE

### 核准

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

指派

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  |  |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `assignUserToRoleOnTasks`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnProjects`<sup>1</sup> |  |  |
|  |  |  |  | `swapUsersOnTasks`<sup>1</sup> |  |  |

{style=&quot;table-layout:auto&quot;}

¹新增欄位：lockToRole

### 客戶偏好設定

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹可能值的更改

### 時數

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `days` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 反覆項目

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  |  |  |  | `moveIssues` |  |  |

{style=&quot;table-layout:auto&quot;}

### 版面範本

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 備註

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `html` |  |  |  |  |  |  |
| `json` |  |  |  |  |  |  |
| `richTextNoteID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Op 任務

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |  |  | `convertToProject` |  |  |
| `isReady` |  |  |  | `convertToTask` |  |  |
| `storyBoardOrder` |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### 資源預算

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `ID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹已移除標幟：可報告

### 排程

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 任務

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  | `agileWork` |  |  | `convertToProject` |  |  |
|  |  |  |  | `linkExternalObject` |  |  |
|  |  |  |  | `unlinkExternalObject` |  |  |

{style=&quot;table-layout:auto&quot;}

### 團隊

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `includeIssues` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 時間表配置檔案

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### UIFilter

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `filtersForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### UIView

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  |  |  |  |  | `viewsForObjCode` |  |

{style=&quot;table-layout:auto&quot;}

### 使用者

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `logTimeInDays` |  |  |  |  |  |  |
| `workHoursPerDay` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### 工作

| 欄位 | 參考 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |  |  | `getWFHomeObjects` |  |  |
