---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱資源欄位
description: 事件訂閱資源欄位
author: Becky
feature: Workfront API
exl-id: 54859930-7619-4b93-8dff-29b10e43d6d5
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 11%

---

# 事件訂閱資源欄位

事件訂閱資源欄位表示導致事件訂閱傳送傳出訊息至已設定端點的事件觸發器。 編輯資源欄位時，會觸發UPDATE事件。

下表列出可用於事件訂閱資源的欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>資源</th> 
   <th>objCode</th> 
   <th>欄位</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>指派</td> 
   <td>ASSGN</td> 
   <td>actualWorkCompleted</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>actualWorkPerDayStartDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> assignmentPercent </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> avgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isPrimary</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isTeamAssignment </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opTaskID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedAvgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedUserAllocationPercentage </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>工作</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDayList</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workRequired</td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>CMPY</td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td>儀表板</td> 
   <td>PTLTAB</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>lastUpdateDate</p> <p>注意：LastUpdateDate只會在每天第一次更新時觸發事件。 </p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>DOCU</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customer:isAdvancedDocMgmtEnabled</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>群組</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>referenceNumber</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>DocumentVersion</span> </td> 
   <td><span>DOCV</span> </td> 
   <td><span>activeProofStages</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>docSize</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>enteredByID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>分機</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalIntegrationType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalStorageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>位置</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>presolidByUserID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDeadlineDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofOwnerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofPages</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofProgress</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofApprovalStatusID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>版本</span> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>EXPNS</td> 
   <td> actualAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> actualUnitAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> billingRecordID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> categoryID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customFormsIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>effectiveDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expenseTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isBillable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 是可報銷的 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isRevacted </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>masterTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objectCategories</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>planedAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>planedDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>planedUnitAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjectName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjID</td> 
  </tr> 
  <tr> 
   <td>時數</td> 
   <td>HOUR</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> actualCost </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedOnDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>小時</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>時間表ID</td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>OPTASK</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>planedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>附註</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>noteText</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>主旨</td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>埠</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>PRGM</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>PROJ</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>貨幣</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>planedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ponsorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>ProofApproval</span> </td> 
   <td><span>PRFAPL</span> </td> 
   <td><span>documentVersionID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>isAwaitingDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofCreationDate</span> </td> 
  </tr> 
  <tr> 
   <td>報告</td> 
   <td>PTLSEC</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiObjCode</td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>任務</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>planedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>TMPL</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>說明</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>優先順序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ponsorID</td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>TSHET</td> 
   <td>approversListString</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>displayName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>endDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hasNotes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursDuration</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isEditable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>atterimedHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>runelHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>startDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>狀態</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>totalHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>使用者</td> 
   <td>accessLevelID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeTeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isActive</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastLoginDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>managerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>名稱</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>title</td> 
  </tr> 
 </tbody> 
</table>

&#42;parameterValue是與各種Workfront資源（或物件）相關聯的自訂欄位值。 事件訂閱傳出訊息包含填入的parameterValues（自訂欄位）的完整清單。
