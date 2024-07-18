---
content-type: api
navigation-topic: api-navigation-topic
title: API第9版的更新
description: 已更新的資源
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 39%

---

# API第9版的更新

## 已更新的資源

此版本的Adobe Workfront API已更新下列現有資源。 若要檢視版本9的新資源，您可以造訪[API版本9](../../wf-api/api/new-api-version-9.md)的新增功能[API版本9的新增功能（續）](../../wf-api/api/new-api-version-9-continue.md)。 對資源所做的變更會以下列方式表示：

* 新增內容只會列出
* 移除以刪除線文字表示
* 變更會記在表格後面的註記中

### 敏捷工作

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup> |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup>1</sup>旗標已移除：可報告\
<sup>2</sup>旗標已移除： NOT_GROUPABLE

### 核准

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

指派

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup>已新增欄位： lockToRole

### 客戶喜好設定

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能值的變更

### 小時

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `days` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 反覆項目

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues` |   |   |

{style="table-layout:auto"}

### 版面配置範本

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### 備註

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `html` |   |   |   |   |   |   |
| `json` |   |   |   |   |   |   |
| `richTextNoteID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Op 任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |   |   | `convertToProject` |   |   |
| `isReady` |   |   |   | `convertToTask` |   |   |
| `storyBoardOrder` |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### 資源預算

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>旗標已移除：可報告

### 排程

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |   |   |   |   |   |

{style="table-layout:auto"}

### 任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   | `agileWork` |   |   | `convertToProject` |   |   |
|   |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### 團隊

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `includeIssues` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 週期性時程表

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode` |   |

{style="table-layout:auto"}

### 使用者介面

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode` |   |

{style="table-layout:auto"}

### 使用者

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `logTimeInDays` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 工作

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 營運 |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   | `getWFHomeObjects` |   |   |
