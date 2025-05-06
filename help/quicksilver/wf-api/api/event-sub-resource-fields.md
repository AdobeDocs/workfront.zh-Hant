---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱資源欄位
description: 事件訂閱資源欄位
author: Becky
feature: Workfront API
role: Developer
exl-id: 54859930-7619-4b93-8dff-29b10e43d6d5
source-git-commit: 50878d9799025f35101cc267d26f2f6330750357
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 9%

---

# 事件訂閱資源欄位

事件訂閱資源欄位代表事件的觸發器，該事件會導致事件訂閱傳送傳出訊息至已設定的端點。 編輯資源欄位時會觸發UPDATE事件。

請注意，資料可使用巢狀篩選進行篩選。 如需詳細資訊，請參閱文章事件訂閱API中的[使用巢狀篩選器](/help/quicksilver/wf-api/general/event-subs-api.md#using-nested-filters)。

下表列出事件訂閱資源可用的欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>資源</th> 
   <th>物件代碼</th> 
   <th>欄位</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>指派</td> 
   <td>指派</td> 
   <td>actualWorkCompleted</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>actualWorkPerDayStartDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> assignmentPercent </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> avgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> categoryID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 分類器ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> financeLastUpdateDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isPrimary</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isTeamAssignment </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdateDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 物件代碼 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 物件類別 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opTaskId </td> 
  </tr>
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> parametervalues </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedAvgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedUserAllocationPercentage </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> securityRootID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>工作</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDate <p>[！BADGE已移除]{type=negative tooltip="此欄位已於2023年10月26日移除。"}</span></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDayList</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>所需工作</td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>CMPY</td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> extRefId </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> groupID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 物件代碼 </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> parametervalues </td> 
  </tr> 
  <tr> 
  <tr> 
   <td>儀表板</td> 
   <td>PTLTAB</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>docID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>lastUpdateDate</p> <p>注意： LastUpdateDate只會在每天首次更新時觸發事件。 </p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Portalprofileid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>檔案</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customer：isAdvancedDocMgmtEnabled</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Documentrequestid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>群組<p><b>注意</b>：此欄位無法篩選。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>附註ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parametervalues</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>referenceNumber</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>releaseVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>範本任務ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Topobjid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>DocumentVersion</span> </td> 
   <td><span>DOCV</span> </td> 
   <td><span>accessorIDs</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>activeProofStages</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Documentproviderid</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>docSize</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>enteredByID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>分機</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalIntegrationType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalStorageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>檔案名稱</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>識別碼</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>位置</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>物件代碼</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofApprovalStatusID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofedByUserID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDeadlineDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>校訂決定</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>校訂ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>校訂名稱</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofOwnerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>校訂頁面</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofProgress</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofStageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>版本</span> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>費用</td> 
   <td> actualAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> actualUnitAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> billingRecordID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> categoryID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customFormsIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>effectiondate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>費用型別ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isBillable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 是可償還 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isRefelsed </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件類別</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedUnitAmou</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjectName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>範本任務ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Topobjid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjID</td> 
  </tr> 
  <tr> 
   <td>欄位</td> 
   <td>欄位</td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> createdBy </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerId </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> dateOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 說明 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 顯示名稱 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> formulanoptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> hasError </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> linkedField </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lookupOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> numberoptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 物件代碼 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 選項 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> referenceOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 類型 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 更新時間 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 更新者 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> userOptions </td> 
  </tr> 
  <tr> 
   <td>時數</td> 
   <td>HOUR</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 實際成本 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedOnDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalTimesheetID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>小時</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>專案管理費用ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetID</td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>OPTASK</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>佇列主題ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionissedid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveOpTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveProjectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolvetaskid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolvingObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>來源物件ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>附註</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachDocumentId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Attactionobjid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachOpTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Attactionworkuserid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>auditRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>檔案ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalServiceID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>附註文字</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentInventationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentJournalEntryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentnotedid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>proofactionid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rtfNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>主旨</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>範本任務ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>threadid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Topobjid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>連線埠</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignmentScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>PRGM</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>專案</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignmentScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachedRateCardID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>貨幣</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverablescorecardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
    <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowautomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
<tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>里程碑路徑ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>popaccountid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionissedid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>subscriptorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>校訂核准</span> </td> 
   <td><span>PRFAPL</span> </td> 
   <td><span>accessorIDs</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>customerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentVersionID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>識別碼</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>isWaitingDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>物件代碼</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofCreationDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>請求者ID</span> </td> 
  </tr> 
  <tr> 
   <td>記錄</td> 
   <td>記錄</td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdBy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>資料<p><b>注意</b>：此欄位無法篩選。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordExternalOptions</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordTypeId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新時間</td> 
  </tr> 
  <tr> 
   <td>記錄類型 </td> 
   <td>RECORD_TYPE </td> 
   <td>顏色</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdBy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>資料<p><b>注意</b>：此欄位無法篩選。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>顯示名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalOptions</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>欄位<p><b>注意</b>：此欄位無法篩選。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>圖示</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isExternal</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isTaxonomy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>許可權</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>primaryFieldId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordscount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新時間</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新者</td> 
  </tr> 
  <tr> 
   <td>報告</td> 
   <td>PTLSEC</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>appGlobalID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>filterId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastViewedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>preferenceID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>publicRunAsUserId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>reportfolderid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>runAsUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>排程報告識別碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>viewID</td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>任務</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>里程碑ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recurrenceRuleId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionissedid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>範本任務ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>範本</td> 
   <td>存取子IDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverablescorecardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowautomationID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>里程碑路徑ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>subscriptorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>表格</td> 
   <td>approverID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approversListString</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>顯示名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>endDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hasnotes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursDuration</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>可編輯</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>overftimeHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>regularHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>startDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>totalhours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>使用者</td> 
   <td>accessLevelId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>defaultHourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>delegationToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Eauthuserid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>emailAddr</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Hometeamid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isActive</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastEnteredNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastLoginDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>latestUpdateNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Layouttemplateid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>logTimeInDays</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>managerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>引數值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Portalprofileid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>標題</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiTemplateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Uuuserid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workHoursPerDay </td> 
  </tr> 
  <tr> 
   <td>工作區</td> 
   <td>Workspace</td> 
   <td>顏色</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdAt</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdBy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>圖示 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>物件代碼</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>許可權</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordTypes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新時間</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新者</td> 
  </tr> 
 </tbody> 
</table>

&#42;parameterValue是與各種Workfront資源（或物件）相關聯的自訂欄位值。 事件訂閱傳出訊息包含填入的parameterValues （自訂欄位）的完整清單。
