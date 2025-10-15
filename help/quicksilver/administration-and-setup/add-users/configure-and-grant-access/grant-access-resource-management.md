---
title: 授與資源管理的存取權
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中資源管理的存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 5%

---

# 授與資源管理的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對資源管理的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用自訂存取層級設定使用者對資源管理工具的存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下資源管理右側![](assets/gear-icon-settings.png)檢視&#x200B;**或**&#x200B;編輯&#x200B;**按鈕上的齒輪圖示**，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在規劃工具中編輯優先順序和預算</td> 
      <td> <p>允許擁有此授權的使用者執行下列動作：</p> <p>排定資源規劃工具中專案的優先順序。</p> <p>資源計畫工具中資源的預算分配（專案的「業務案例」中的「資源規劃工具」與「資源預算」區段）。</p> <p>此選項預設為啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理資源集區</td> 
      <td> <p>允許擁有此授權的使用者建立、編輯和刪除資源集區。 此選項預設為停用。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>更新工作負載平衡器中的計畫時數</span> </td> 
      <td> <p>允許擁有此授權的使用者在更新工作負載平衡器中的使用者指派時更新規劃時數工作專案。 分配時數總計會變成工作專案的計畫時數。</p> <p>此選項預設為停用。</p> <p> 如需詳細資訊，請參閱<a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器</a>中管理使用者配置。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 依授權型別存取資源管理

如需有關每個存取層級中的使用者可以執行哪些資源管理的資訊，請參閱每個物件型別[可用的文章](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource)功能中的[資源管理](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)小節。

## 存取共用問題

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

當您與其他使用者共用物件時，收件者對其編列預算或檢視資源配置的許可權是由下列三項的組合所決定：

* 收件者資源管理的存取層級設定
* 使用者對財務資料的存取權，如[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)中所述
* 共用者授予物件的任何財務資料許可權

如需使用者在共用物件時可授與物件財務資料之許可權的資訊，請參閱[共用物件的財務許可權](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)。
