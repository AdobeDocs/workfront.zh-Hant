---
product-area: projects
navigation-topic: manage-tasks
title: 刪除任務
description: 您可以刪除重複或建立有誤的任務。
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 5%

---

# 刪除任務

您可以刪除重複或建立有誤的任務。

對於具有歷史資訊（更新、排程變更、狀態或其他欄位）的任務，我們建議您關閉或將它們標籤為無效，而不是刪除它們。 這可協助您保留專案的歷史資訊。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p> 
   <p>工作或更高層級</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對具有刪除存取權的任務和專案的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>為專案貢獻許可權，並可新增任務或以上專案</p> <p>建立任務時，您會自動收到該任務的「管理」許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects with access to&nbsp;Delete</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 瞭解刪除任務的程式

* [刪除任務的限制](#limitations-for-deleting-tasks)
* [刪除任務的影響](#the-impact-of-deleting-tasks)

### 刪除任務的限制  {#limitations-for-deleting-tasks}

* 當專案狀態為「完成」時，您必須是您的Workfront管理員或群組管理員在您的「專案偏好設定」區域中允許此動作，才能刪除任務。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 如果任務已記錄時數，Workfront或群組管理員必須透過在您的Workfront執行個體中設定任務和問題偏好設定，以允許刪除這些任務。 當您嘗試刪除擁有已記錄時數任務的專案時，這也適用。

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  如需有關啟用刪除記錄時數之任務的詳細資訊，請參閱[設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)中的「刪除」一節。

### 刪除任務的影響 {#the-impact-of-deleting-tasks}

當您刪除任務時，會影響連結到該任務的其他物件。

請考量下列事項：

* 當您刪除任務時，也會刪除附加至任務的下列物件：

   * 文件

  您不能刪除附加了已出庫檔案的任務。 如需簽出檔案的詳細資訊，請參閱[簽出檔案](../../../documents/managing-documents/check-out-documents.md)。

   * 問題
   * 子任務
   * 附註
   * 核准

* 根據您的Workfront管理員如何在Workfront執行個體的時程表和小時偏好設定中設定專案、任務或問題刪除偏好設定，任務記錄的小時在刪除任務時以下列方式之一處理：

   * 移至專案，如果稍後還原任務，則不會在任務上還原。
   * 會被刪除，並將在任務上還原（如果稍後還原任務）。

  當您嘗試刪除擁有已記錄時數任務的專案時，這也適用。

  如需有關為登入問題時數設定刪除偏好設定的詳細資訊，請參閱[設定時程表和時數偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。
   * 任務的費用將移至專案。

   * 指派給任務或任務核准的使用者仍保留在專案團隊中。

  如需專案團隊的詳細資訊，請參閱[專案團隊概述](../../../manage-work/projects/planning-a-project/project-team-overview.md)。

* 當您刪除子項任務並將其父項移動到另一個專案中，然後恢復已刪除的子項任務時，該任務會新增回原始專案作為主要任務。

<!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

## 刪除任務

* [同時刪除專案中的多個任務](#delete-multiple-tasks-in-a-project-simultaneously)
* [刪除單一任務](#delete-a-single-task)

### 同時刪除專案中的多個任務  {#delete-multiple-tasks-in-a-project-simultaneously}

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**專案**。
1. 按一下包含您要刪除之任務的專案名稱。
1. 按一下左側面板中的&#x200B;**工作**。
1. 執行下列其中一項：

   1. （視條件而定）啟用&#x200B;**自動儲存**&#x200B;切換功能時：

      1. 選取您要刪除的工作，然後按一下&#x200B;**更多**
      1. 按一下&#x200B;**刪除**，然後按一下&#x200B;**刪除**&#x200B;以確認刪除。

         任務即被刪除。

   1. （視條件而定）如果要回覆對工作清單所做的變更，請按一下&#x200B;**計畫模式**&#x200B;圖示，並選取&#x200B;**手動儲存**。

      ![選取手動儲存](assets/manual-save-option.png)

      請執行下列動作：

      1. 選取您要刪除的任務。
      1. 按一下&#x200B;**刪除**。
      1. （選擇性）按一下[復原] **&#x200B;**&#x200B;以復原您的變更，並且不刪除工作。
      1. 如果要保留變更並刪除工作，請按一下[重做] **&#x200B;**。
      1. 按一下[儲存]刪除工作。**&#x200B;**

         只有在您儲存變更後，才會刪除任務。

### 刪除單一任務 {#delete-a-single-task}

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**專案**。
1. 按一下包含您要刪除之任務的專案名稱。
1. 按一下左側面板中的&#x200B;**工作**。
1. 按一下要刪除的工作名稱。
1. 按一下右上角的&#x200B;**更多**&#x200B;圖示![](assets/qs-more-menu.png)。

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. 按一下&#x200B;**刪除工作**。
1. 如果允許刪除，請按一下&#x200B;**刪除**。

   您的Workfront管理員或群組管理員可能不允許刪除記錄時數的任務。

   如需有關刪除任務所需存取權和許可權的詳細資訊，請參閱本文中[刪除任務的限制](#limitations-for-deleting-tasks)一節。

## 還原已刪除的任務

Workfront或群組管理員可以在刪除工作後30天內還原工作，如[還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)中所述。
