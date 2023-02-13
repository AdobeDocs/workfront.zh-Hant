---
product-area: resource-management
navigation-topic: resource-planning
title: 查找資源計畫員
description: 「(這篇文章的內容是：當文章上線時，請起草該內容：/Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)`
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 查找資源計畫員

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

您可以使用資源計畫員來管理資源分配給項目。 您可以從項目的「業務案例」區域同時訪問多個項目或一個項目的資源計畫器。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>在全局區域中定位資源計畫員的計畫或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看對資源管理的訪問權限或更高版本</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案和使用者的權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

在開始使用資源規劃器之前，請確保滿足訪問和使用資源規劃器的所有先決條件。 這樣，在開始對資源進行預算之前，您可以確保資源計畫員顯示正確的資訊。

有關資源規劃器必備條件的資訊，請參閱 [開始使用資源規劃](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## 查找資源計畫員

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

您可以在Workfront的兩個區域中查找資源計畫器，具體取決於您要為多個項目或僅一個項目預算資源。

* [對多個項目使用資源計畫器](#use-the-resource-planner-for-multiple-projects)
* [將資源計畫器用於一個項目](#use-the-resource-planner-for-one-project)

### 對多個項目使用資源計畫器 {#use-the-resource-planner-for-multiple-projects}

對多個項目使用資源計畫器時，資源的分配編號表示多個項目中的編號。

要訪問「資源」區域中的「計畫員」部分，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **資源**. 預設情況下，計畫員將顯示。  有關資源計畫員中預算資源的資訊，請參閱本文 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 將滑鼠指標暫留在左側面板上，然後按一下 **資源池**.\
   有關建立資源池的資訊，請參見 [建立資源池](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### 將資源計畫器用於一個項目 {#use-the-resource-planner-for-one-project}

對一個項目使用資源計畫器時，資源的分配編號表示所選項目的編號。

1. 轉到要為資源預算的項目。
1. 按一下 **業務案例** 中。
1. 捲動至 **資源預算** 部分。
1. 按一下 **編輯資源預算** 向項目添加資源池並開始為資源編製預算。

   >[!TIP]
   >
   >只有在項目沒有與其關聯的資源池時，才可以在Business Case的「資源預算」區域中添加資源池。 當項目已有資源池時，預設情況下，池中的用戶及其任務角色將顯示在「資源預算」區域中。

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   有關一個項目的預算資源的資訊，請參閱文章 [業務案例中的預算資源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
