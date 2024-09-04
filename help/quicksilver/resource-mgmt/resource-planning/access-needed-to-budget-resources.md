---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 在Workfront中預算資源所需的存取權
description: 當您擁有工作專案、使用者、工作角色和團隊的特定存取層級設定和許可權時，您可以針對您有權檢視的專案檢視和管理有關資源計畫的資訊。
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# 在Workfront中預算資源所需的存取權

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

當貴公司購買包含資源規劃的Adobe Workfront授權時，您可以檢視您有權檢視之專案的資源預算資訊。 您可以在資源規劃工具中檢視預算資訊。

如需有關在Workfront中使用預算工具之先決條件的詳細資訊，請參閱[開始使用資源規劃](../../resource-mgmt/resource-planning/get-started-resource-planning.md)。

若要預算資源、管理「資源集區」，並在資源計畫工具中檢視「成本」資訊，您的公司與您必須具有下列存取權： 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td><p>新增：任何</p>
       <p>或</p>
       <p>目前：Pro或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> 
    <ul> 
     <li> <p>編輯存取層級中「資源管理」的存取權，包括：</p> 
      <ul> 
       <li> <p>存取以編輯專案優先順序和預算時數。 </p> </li> 
       <li> <p>存取以管理資源集區（如果您需要管理資源集區）。</p> </li> 
      </ul> <p>如需有關資源管理存取層級的資訊，請參閱文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">授予資源管理的存取權</a>。</p> </li> 
     <li> <p>編輯專案和使用者的存取權。 </p> </li> 
     <li> <p> 如果您需要依成本檢視或管理資訊，請在存取層級中編輯財務資料的存取權。</p> <p>如需財務資料存取層級的詳細資訊，請參閱文章<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予財務資料的存取權</a>。</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權，包括管理財務許可權。</p> <p>如需有關專案許可權的資訊，請參閱文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>。</p> <p>如需有關專案財務許可權的資訊，請參閱文章<a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共用物件的財務許可權</a></a>。</p>

<p><b>附註</b>

在「角色」檢視中編列資源預算時，如果角色下列出的至少一個專案少於「管理」許可權，則無法為角色編列時數、FTE或成本的預算。 您只能為您擁有管理許可權的專案編列預算。</p> </td>
</tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
