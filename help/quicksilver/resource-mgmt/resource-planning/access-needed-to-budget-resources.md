---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 獲得Adobe Workfront預算資源所需資源
description: 當您具有特定訪問級別設定和工作項、用戶、作業角色和團隊的權限時，可以查看和管理有權查看的項目的資源規劃資訊。
author: Alina
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 獲得Adobe Workfront預算資源所需資源

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

當您的公司購買了包含Oracle Resource Planning的Adobe Workfront許可證時，您可以查看您有權查看的項目的資源預算資訊。 您可以在資源計畫員中查看預算資訊。

如需在Workfront中使用預算工具的必要條件的詳細資訊，請參閱 [開始使用資源規劃](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

要對資源進行預算，請管理資源池，並查看資源規劃工具中的成本資訊，您的公司和您必須具有以下訪問權限： 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> 
    <ul> 
     <li> <p>在訪問級別中編輯對資源管理的訪問，包括：</p> 
      <ul> 
       <li> <p>存取編輯專案優先順序和預算小時數。 </p> </li> 
       <li> <p>如果需要管理資源池，可訪問管理資源池。</p> </li> 
      </ul> <p>有關資源管理訪問級別的資訊，請參見文章 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予資源管理的訪問權限</a>.</p> </li> 
     <li> <p>編輯「專案」和「使用者」的存取權。 </p> </li> 
     <li> <p> 如果需要按成本查看或管理資訊，請在訪問級別中編輯對財務資料的訪問。</p> <p>有關財務資料訪問級別的詳細資訊，請參閱文章 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予金融資料的存取權</a>.</p> </li> 
    </ul>

<p><b>附註</b> </p>

<p> 如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理包含「管理財務」權限之專案的權限。</p> <p>如需專案權限的相關資訊，請參閱文章 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>如需專案的財務權限相關資訊，請參閱文章 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共用物件的財務權限</a></a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">請求對對象的訪問 </a>.</p>

<p><b>附註</b>

在「職責」視圖中編製預算資源時，如果職責下列出的至少一個項目的「管理」權限少於「管理」權限，則不能為職責預算小時數、FTE或成本。 您只能對您擁有「管理」權限的專案進行預算。</p> </td>
</tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。
