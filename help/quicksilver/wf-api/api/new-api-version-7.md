---
content-type: api
navigation-topic: api-navigation-topic
title: API 7版的新增功能
description: 集合
author: Becky
feature: Workfront API
role: Developer
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 47%

---

# API 7版的新增功能

## 新物件

### 校訂Bean

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 搜尋 |
| 行尾 |   |   |   |   |   |   |
| 名稱 |   |   |   |   |   |   |

{style="table-layout:auto"}

### DocMetadataLink

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>欄位</th> 
   <th>引用</th> 
   <th> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">集合</p> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">+++++++++++ </p> </th> 
   <th>搜尋</th> 
   <th>動作</th> 
   <th>查詢</th> 
   <th>作業</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>新增</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>計數 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>刪除 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Get  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>報告 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>搜尋 </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
|   |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | 刪除 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | 搜尋 |

{style="table-layout:auto"}

### ProofApproval

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | 搜尋 |

{style="table-layout:auto"}

 

### 資源輪廓

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 新增 |
|   |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | 刪除 |
|   |   |   |   |   |   | 編輯 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | 搜尋 |

{style="table-layout:auto"}

 

### 使用者群組

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| groupID | 群組 |   |   |   |   |   |
| isOwner  | 使用者  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 週期性時程表

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |  hourType |   |   |   | 新增 |
| 名稱 |   |   |   |   |   | 複製 |
|   |   |   |   |   |   | 計數 |
|   |   |   |   |   |   | 刪除 |
|   |   |   |   |   |   | 編輯 |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | 報告 |
|   |   |   |   |   |   | 搜尋 |
|   |   |   |   |   |   | 取代 |

{style="table-layout:auto"}

 

### RsrcPool

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID | 客戶 | 使用者 |   |   |   | 新增 |
| customerID  | 輸入者  |   |   |   |   | 計數 |
| 說明  | lastUpdatedBy  |   |   |   |   | 刪除 |
| enteredById  |   |   |   |   |   | 編輯 |
| entryDate  |   |   |   |   |   | Get |
| extRefId  |   |   |   |   |   | 報告 |
| lastUpdateDate |   |   |   |   |   | 搜尋 |
| lastUpdateByID |   |   |   |   |   |   |
| 名稱 |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### DocMetadataLinkGroup

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 計數 |
| 文章名稱  |   |   |   |   |   | Get |
| pageID  |   |   |   |   |   | 報告 |
| url  |   |   |   |   |   | 搜尋 |

{style="table-layout:auto"}

 

 

 

## 更新的物件

對現有物件的變更：新增物件只是簡單的列出、移除具有刪除線、對現有物件的變更在表格後面具有附加註記

### UpdateBean

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能值的變更 

 

### ApprovalServiceObject

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate<sup>1</sup> |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style="table-layout:auto"}

 

### 存取規則<sup>1</sup>

<sup>1</sup> 標示為可報告

 

### 核准流程

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style="table-layout:auto"}

  

### 核准路徑<sup>1</sup>

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style="table-layout:auto"}

<sup>1</sup> 已移除可報告旗標

 

### 工作服務物件

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 日期驗證已新增

<sup>2</sup> 已新增Not_Filterable旗標

 

### 指派

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProject<sup>1</sup> |   |   |
|   |   |   |   | swapUsersOnProjects<sup>1</sup> |   |   |
|   |   |   |   | unassignuserfromprojects<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> 新增欄位includeIssues

 

### 客戶 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能值的變更 

 

### 自訂枚舉 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 文件 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style="table-layout:auto"}

 

### 檔案版本 

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style="table-layout:auto"}

 

### 群組

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | 使用者群組  |   |   |   |   |
| Layouttemplateid |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 將PRECISION驗證器從8變更為9

 

### Hourtype

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style="table-layout:auto"}

 

### 日誌輸入項目

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能值的變更

 

### Optask （問題）

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### 專案

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### QueueDef

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style="table-layout:auto"}

 

### 佇列主題

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  佇列主題ID |   |

{style="table-layout:auto"}

 

### 最新

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style="table-layout:auto"}

 

### 任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### 範本任務

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| 所需工作<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 型別從Int變更為Double 

 

### 使用者

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>欄位</th> 
   <th>引用</th> 
   <th>集合</th> 
   <th>搜尋</th> 
   <th>動作</th> 
   <th>查詢</th> 
   <th>作業</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>
    <code>lastWhatsNew</code> </td> 
   <td> </td> 
   <td>
    <code>roles</code> </td> 
   <td> 角色</td> 
   <td>addMobileDevice</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDeactivationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timesheetProfileHourTypes</span> </td> 
   <td> </td> 
   <td>getAvailableActions</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>hasanyaccess</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>isUserTerminalsActive</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>removeMobileDevice</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>showShouldProofHQNavButton</td> 
   <td> </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

### 使用者附註

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackknowledgeMany |   |   |
| ackDate |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### CustomerPrefObject

| 欄位 | 引用 | 集合 | 搜尋 | 動作 | 查詢 | 作業 |
|---|---|---|---|---|---|---|
|  名稱 |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能值的變更
