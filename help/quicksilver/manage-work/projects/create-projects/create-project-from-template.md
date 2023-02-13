---
product-area: projects;templates
navigation-topic: create-projects
title: 使用範本建立專案
description: 您可以使用範本作為架構來建立新專案。 如果您的專案經常重複，則在新專案的一般時間軸中使用範本，可省去重複建立相同專案的繁瑣工作。
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 1%

---

# 使用範本建立專案

您可以使用範本作為架構來建立新專案。 如果您的專案經常重複，則在新專案的一般時間軸中使用範本，可省去重複建立相同專案的繁瑣工作。

範本可讓您擷取與專案相關聯的所有可重複的程式、資訊和設定。 與模板關聯的所有資訊都將傳輸到項目。 這包括任務、分配、持續時間、文檔、財務詳細資訊、風險和自定義表單。

>[!TIP]
>
>從模板建立的新項目的狀態與主「項目首選項」區域中的Workfront管理員或組的「項目首選項」區域中的組管理員(或Workfront管理員)所定義的狀態相對應。 如需設定專案偏好設定的相關資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 或 [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

從範本建立專案時，您有下列選項：

* 從「項目」區域中的模板建立項目
* 從範本層級的範本建立專案
* 將範本附加至現有專案

   如需詳細資訊，請參閱 [將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* 從「組」區域中的模板建立項目

## 存取需求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront授權概述*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯專案和範本的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取專案的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予專案的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視範本的權限</p> <p>建立專案時，您會自動收到專案的「管理」權限 </p> <p> 如需專案權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從「項目」區域中的模板建立項目

您可以從主菜單中的「項目」區域，或從產品組合或方案的「項目」區域建立項目。

1. 執行下列任一項作業：

   * 按一下 **主菜單** ![](assets/main-menu-icon.png)，按一下 **專案**，然後展開 **新增專案**.
   * 前往產品組合，然後展開 **新增專案**.

      >[!TIP]
      >
      >當您使用產品組合中的範本建立專案時，新專案的「Portfolio」欄位會更新，以顯示您選擇建立專案的產品組合。 如果已指定，則會覆寫範本上的Portfolio欄位。

   * 前往程式，然後展開 **新增專案**.

      >[!TIP]
      >
      >使用方案的模板建立項目時，新項目的「方案」欄位將更新，以顯示您選擇建立項目的方案。 範本的「Portfolio」欄位會更新，以顯示您選擇建立專案的方案組合。 這會覆寫範本上的程式和Portfolio欄位（如果已指定）。

   * 如果您是群組管理員，也可以在您管理之群組的「專案」區段中建立專案。 如需詳細資訊，請參閱 [建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >使用組中的模板建立項目時，僅當未指定模板的「組」欄位時，才會在新項目的「組」欄位中顯示從中建立項目的組。 如果指定了模板組欄位，則新項目的組欄位為模板的組欄位。
   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 在 **最喜愛的範本** 清單

   ![](assets/new-project-from-template-dropdown-with-template-favorites-nwe-350x235.png)

   或

   執行下列動作：

   1. 選擇 **從範本新增專案**.
   1. 在 **搜尋範本** 欄位中，開始鍵入模板的名稱，然後在該名稱顯示在清單中時按一下。
   1. 檢閱右側的範本詳細資訊。

      範本詳細資訊包括：

      * 範本持續時間
      * 範本擁有者
      * 包括前三個任務名稱的頂層任務數
      * 模板中所有任務的數量
      * 範本自訂表單的名稱
   1. （選用）將滑鼠指標暫留在範本名稱上，然後按一下 **我的最愛** **圖示** ![](assets/favorites-icon-small.png) 將其標示為收藏供將來使用。

      或

      展開 **最喜愛的範本** 清單，然後從下拉式清單中選取範本。

      >[!TIP]
      >
      >您最多可以有40個Workfront項目標示為我的最愛。 這包括範本和其他項目。

   1. 按一下 **使用範本** 當您已選取範本時。

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!NOTE]
   >
   >如果已將「里程碑視圖」(Milestone View)應用到項目清單，請按一下 **從範本新增區段**.
   >
   >
   >![](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)   >

1. 此 **新增專案** 框。

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

1. 如果範本中已填入欄位，則會在 **新增專案** 框。 您可以編輯預先填入的值，以更符合您的專案。 如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).
1. 按一下 **建立專案**.

   如果您未在上一步驟中變更，則模板中定義的所有詳細資訊都會自動與新建立的項目關聯。

## 從「模板」區域的模板建立項目

您可以從範本開始，從範本開始建立專案，而不是從「專案」區域開始。

 

1. 從 **主菜單**，按一下 **範本**.

1. 按一下您要使用的範本名稱。
1. 按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **建立專案。**

   ![從範本建立專案](assets/project-sharing-on-template-nwe-2022-350x172.png)

   此 **新增專案** 框。

1. 指定專案的名稱，然後檢閱每個區段並進行任何必要的變更。

   ![](assets/new-project-from-template-box-with-all-sections-on-left-panel-nwe-350x282.png)

   如果範本中已填入欄位，則會在 **新增專案** 框。 您可以編輯預先填入的值，以更符合您的專案。 如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 按一下 **建立專案。**

   如果您未在上一步驟中變更，則模板中定義的所有詳細資訊都會自動與新建立的項目關聯。
