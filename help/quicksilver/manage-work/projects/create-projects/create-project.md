---
product-area: projects
navigation-topic: create-projects
title: 建立專案
description: 專案是Adobe Workfront中的大型工作單位。 您可以從頭開始建立專案、使用範本，或將問題或任務轉換為專案。
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1390'
ht-degree: 1%

---

# 建立專案

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

專案代表在Adobe Workfront中需要完成的大量工作。

## 存取需求

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準</p>
        <p>或</p>
        <p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>建立專案時，您會自動收到專案的管理許可權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立專案的方式

您可以使用下列其中一種方法，在Workfront中建立專案：

* 從頭開始建立專案，而不使用範本。 本文會介紹如何從頭開始建立專案。

* 複製現有專案。\
  如需有關複製專案的詳細資訊，請參閱[複製專案](../../../manage-work/projects/manage-projects/copy-project.md)。

* 使用範本。\
  如需使用範本建立新專案的詳細資訊，請參閱[使用範本建立專案](../../../manage-work/projects/create-projects/create-project-from-template.md)。

* 從Microsoft專案匯入專案。\
  如需有關從MS Project匯入專案的詳細資訊，請參閱[從Microsoft專案匯入專案](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)。

* 使用kick-start匯入專案。

  身為Workfront管理員，您可以使用kick-start匯入專案。

  如需有關在Workfront中使用Kick-Start匯入資料的資訊，請參閱[使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

  如需有關使用Kick-Start匯入專案的資訊，請參閱[Kick-Start情境：簡單專案和任務匯入準備](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md)。

* 從Adobe Workfront情境規劃工具中的情境發佈方案。

  「情境規劃工具」需要下列其中一項：

   * 目前Workfront授權結構的額外授權。
   * 適用於新Ultimate授權結構的Workfront授權。

  如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../../scenario-planner/scenario-planner-overview.md)。 如需有關透過發佈行動方案建立專案的資訊，請參閱[在Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md)中發佈行動方案以更新或建立專案。

* 當您從Workfront Planning中的記錄型別連結專案時，請新增專案。 在生產環境中，您只能從Workfront Planning建立沒有範本的專案。 <span class="preview">您可以在預覽環境中使用範本建立專案。</span>

  您必須擁有新的Workfront授權和適用於Workfront的額外Workfront規劃授權。

  如需有關存取Workfront Planning的資訊，請參閱[存取總覽](/help/quicksilver/planning/access/access-overview.md)。

  如需透過將專案新增至記錄來建立專案的資訊，請參閱文章[當您連線至記錄時，從Workfront Planning建立Workfront物件](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)中的「連線至Workfront Planning的記錄時建立專案」一節

## 先決條件

開始之前，您必須確定：

* 您的系統或群組管理員在設定區域中啟用了「允許使用者在不使用範本的情況下建立專案」偏好設定。

  如需詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 新專案預設設定

建立專案時，Workfront會套用一組預設設定至專案。 例如，當您建立專案時，會預設「狀態」、「群組」和「排程模式」。

請考量下列事項：

* 身為Workfront管理員或群組管理員，您可以在為整個Workfront執行個體或群組設定專案偏好設定時，為新專案設定預設設定。
* Workfront會先套用群組的設定（如果有的話），再套用Workfront管理員設定的設定。
* 新專案的預設狀態與您在主「專案偏好設定」區域中由Workfront管理員定義的狀態相對應，或與群組管理員(或Workfront管理員)在群組「專案偏好設定」區域中定義的狀態相對應。

  >[!NOTE]
  >
  >我們建議新專案的預設狀態為「計畫」。 當您變更新專案時，這可以確保不會將通知傳送給指派給專案的使用者。
  >
  >如需有關設定新專案的預設狀態和其他預設設定的詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)或[設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)。

* 以下是Workfront定義新專案之群組和狀態的方式案例：

   * 如果您從頭開始建立專案，專案群組就是您的主群組。

     專案狀態是主群組（如果有）或Workfront執行個體之專案偏好設定中的預設狀態。 建立專案時，您可以將預設狀態變更為專案群組可用的任何狀態。

   * 如果您使用範本建立專案，範本的設定優先於Workfront或群組管理員建立的設定。

     新專案的群組是範本的群組。 如果範本未與「群組」相關聯，則專案的「群組」是建立專案之使用者的「主群組」 。

     從範本建立的新專案的預設狀態與您在主「專案偏好設定」區域中由Workfront管理員定義的狀態相對應，或與群組的「專案偏好設定」區域中的群組管理員(或Workfront管理員)相對應。 從範本建立專案時，您可以將預設狀態變更為專案群組（範本群組）或建立專案之使用者的「主群組」)的任何狀態。

   * 如果您透過轉換問題來建立專案，則新專案的群組為問題現有專案的群組。 如果轉換問題的使用者無權存取問題的專案，或問題的專案沒有群組，則新專案的群組是轉換問題的使用者的主群組。

     新專案的狀態與專案相關群組的群組狀態相符，這是原始專案的群組或轉換問題的使用者的主群組。

     如果您透過轉換問題來建立專案時使用範本，請參閱上述第二個情境，以瞭解哪一個群組以及哪個Workfront狀態套用至新專案。

## 從頭開始建立專案

>[!NOTE]
>
>如果您使用範本建立專案，建議您也看到文章[使用範本建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)。


1. 執行下列其中一項：

   * 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果可用）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)。 按一下&#x200B;**專案**，然後展開&#x200B;**新增專案**。
   * 移至投資組合，然後展開&#x200B;**新專案**。
   * 前往方案，然後展開&#x200B;**新專案**。
   * 如果您是群組管理員，您也可以在您管理之群組的專案區段中建立專案。 如需詳細資訊，請參閱[建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

   ![新專案功能表](assets/new-project-dropdown-nwe-350x358.png)

1. 按一下功能表中的[新增專案]&#x200B;**&#x200B;**，從頭開始建立專案。
1. 輸入專案名稱。 按下Enter以儲存名稱。

   ![輸入專案名稱](assets/rename-untitled-project.png)

   專案頁面的標題會顯示專案目前健康狀況和進度的快速概覽。 專案資訊更新時，專案標題中的資訊會變更。

1. 按一下&#x200B;**開始新增工作**。

   或

   按一下&#x200B;**新增任務**，將任務新增至專案並指派資源給它們。

   如需將任務新增至專案的詳細資訊，請參閱[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

1. 按一下專案名稱旁的&#x200B;**更多**&#x200B;功能表，然後&#x200B;**編輯** ![編輯圖示](assets/qs-edit-icon.png)，即可編輯專案詳細資料。

   **編輯專案**&#x200B;對話方塊開啟。

   如需有關編輯專案的詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

1. （選擇性）在設定專案設定並新增任務後，您可以將專案狀態變更為&#x200B;**目前**。

   這表示專案現在已準備好開始，並且指派給任務的使用者現在可以開始處理它們。

   如需有關專案狀態的詳細資訊，請參閱[存取系統專案狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)。
