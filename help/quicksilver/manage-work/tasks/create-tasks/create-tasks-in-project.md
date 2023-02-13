---
product-area: projects
navigation-topic: create-tasks
title: 在專案中建立任務
description: 只有在建立專案後，才能在專案中建立工作。
author: Alina
feature: Work Management
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 1%

---

# 在專案中建立任務

只有在建立專案後，才能在專案中建立工作。

例如，建立項目後，您可能需要添加任務並修改任務以組織項目計畫。 如需建立專案的詳細資訊，請參閱 [建立專案](../../../manage-work/projects/create-projects/create-project.md).

如需有關建立不在專案中的個人任務的資訊，請參閱文章中的「建立個人任務」一節 [從「首頁」區域建立工作項](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

本文說明如何從頭建立任務。 您也可以透過下列方式建立工作：

* 複製或複製現有任務。 如需詳細資訊，請參閱 [複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* 將任務從一個項目移動到另一個項目。 如需詳細資訊，請參閱 [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## 存取需求

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td><p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront授權*</p> </td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 有關訪問任務的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予任務的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為專案貢獻權限，並提供新增工作或更新版本</p> <p>建立任務時，您會自動獲得該任務的「管理」權限</p> <p> 有關任務權限的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共用任務 </a>. </p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在專案中建立任務

1. 轉到要建立任務的項目。
1. 按一下 **工作** 中。
1. （條件性）如果您目前是以敏捷檢視檢視來檢視工作清單，請按一下 **清單檢視** 圖示 ![](assets/list-view-in-agile-view-for-tasks.png) 顯示任務清單。
1. （選用）按一下 **計畫模式** 圖示 ![](assets/nwe-plan-mode-icon-task-list.png) 選取 **手動儲存**，然後選取 **標準** 或 **時間表規劃**. 這會停用 **自動儲存** 選項，預設為啟用。

   ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

   >[!TIP]
   >
   >選擇「手動儲存」時，可以撤消更改。

1. 通過執行以下操作之一建立新任務：

   * 按一下 **新任務** 在任務清單的頂部
   * 按一下 **添加更多任務** 在任務清單的底部

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. （條件性）如果您按一下 **新任務** 執行下列動作：

   1. 在 **新任務** 框，然後按一下 **建立任務** 如果要快速建立任務。

      或

      要更新任務的所有欄位，請按一下 **更多選項** 開啟 **建立任務** 框。

      ![](assets/nwe-create-task-small-screen-350x272.png)

      此 **建立任務** 框。

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >根據Workfront管理員設定版面範本的方式，「建立任務」方塊中的欄位可能會在您的環境中顯示不同的欄位。 如需詳細資訊，請參閱 [使用版面範本自訂「詳細資料」檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. 在「建立任務」框的左側面板中指定以下區域的資訊：

      * 任務名稱
      * 總覽
      * 指派
      * 自訂Forms
      * 財務
      * 設定

         有關定義任務上所有與任務相關的欄位的資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
   1. （條件式和選用式）如果您希望重複執行工作，請更新 **週期頻率** 欄位。 有關建立循環任務的詳細資訊，請參閱 [建立循環任務](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. （選用）按一下 **檔案** 在左側面板中，將文檔附加到新任務，然後按一下 **新增或連結檔案** 從電腦、其他服務向任務添加文檔，或從電腦或其他服務連結文檔和資料夾。


1. （條件性）如果您按一下 **添加更多任務** 在步驟5中，開始使用行內編輯輸入任務資訊，然後按Enter鍵。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   建議您使用此選項，尤其是在將多個任務新增至清單時。

   ![](assets/ctp4-350x26.png)

1. （條件性）執行下列其中一項作業：

   * 如果您按一下 **新任務** 在步驟5中，按一下 **建立任務** 保存更改並將新任務添加到項目。

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * 如果您按一下 **添加更多任務** 在步驟5中，執行下列動作：

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. 按一下瀏覽器中的任意位置以提交更改，或按Enter鍵。
      1. （可選）在任務清單中，選擇新建立的任務，然後按一下 **縮進**.

         這會使新任務成為前一個任務的子任務或子任務。

         有關子任務的詳細資訊，請參閱 [任務概述](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. （條件性）如果您停用 **自動儲存** 按下後選項 **添加更多任務**，您可以執行下列動作：

         * 按一下 **還原** 在任何時候撤銷上次變更，或 **取消** 要撤消對任務清單所做的所有更改。
         * 如果您先前曾按一下 **還原**，按一下 **取消復原** 重新應用您取消的最後一次更改。
         * 按一下 **儲存** 保存對任務清單的更改。
