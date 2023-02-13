---
product-area: projects
navigation-topic: manage-tasks
title: 刪除任務
description: 您可以刪除可能是重複的或已錯誤建立的任務。
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---

# 刪除任務

您可以刪除可能是重複的或已錯誤建立的任務。

對於具有歷史資訊（更新、計畫更改、狀態或其他欄位）的任務，建議您關閉它們或將其標籤為「已停止」，而不是將其刪除。 這可協助您保留專案的歷史資訊。

## 存取需求

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問權限，並具有刪除權限</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 有關訪問任務的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予任務的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為專案貢獻權限，並提供新增工作或更新版本</p> <p>建立任務時，您會自動獲得該任務的「管理」權限</p> <p> 有關任務權限的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共用任務 </a>. </p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 了解刪除任務的過程

* [刪除任務的限制](#limitations-for-deleting-tasks)
* [刪除任務的影響](#the-impact-of-deleting-tasks)

### 刪除任務的限制  {#limitations-for-deleting-tasks}

* 如果項目的狀態為「完成」，則只有在您的Workfront管理員或組管理員在「項目首選項」區域中允許執行此操作時，才能刪除任務。 有關設定項目首選項的資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果任務已記錄小時，Workfront或組管理員必須允許通過在Workfront實例中配置任務和問題首選項來刪除這些任務。 當您嘗試刪除已登入數小時之任務的專案時，也會套用此方法。

   <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

   有關啟用刪除記錄小時的任務的詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### 刪除任務的影響 {#the-impact-of-deleting-tasks}

刪除任務時，會影響連結到該任務的其他對象。

刪除任務時，也會刪除附加到任務的以下對象：

* 文件

   無法刪除已附加了已簽出文檔的任務。 有關簽出文檔的詳細資訊，請參閱 [簽出文檔](../../../documents/managing-documents/check-out-documents.md).

* 問題
* 子任務
* 附註
* 核准

根據您的Workfront管理員在Workfront實例的「工時單和小時首選項」中配置項目、任務或問題刪除首選項的方式，在刪除任務時，以下列方式之一處理任務記錄的小時數：

* 移至專案，如果稍後還原任務，則不會在任務上還原。
* 如果稍後還原任務，則會刪除並在任務上還原。

   當您嘗試刪除已登入數小時之任務的專案時，也會套用此方法。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

   如需針對記錄問題的數小時設定刪除偏好設定的詳細資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 任務費用將移至項目。

* 分配給任務或任務批准的用戶將保留在項目組中。

   如需專案團隊的詳細資訊，請參閱 [專案團隊概觀](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 刪除任務

* [同時刪除專案中的多個工作](#delete-multiple-tasks-in-a-project-simultaneously)
* [刪除單個任務](#delete-a-single-task)

### 同時刪除專案中的多個工作  {#delete-multiple-tasks-in-a-project-simultaneously}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **專案**.
1. 按一下包含您要刪除之任務的專案名稱。
1. 按一下 **工作** 中。
1. 執行下列任一項作業：

   1. （條件性）若 **自動儲存** 切換為啟用：

      1. 選擇要刪除的任務，然後按一下 **更多**
      1. 按一下 **刪除**，然後 **是，刪除它** 以確認刪除。

         將刪除這些任務。
   1. （條件性）按一下 **計畫模式** 圖示並選取 **手動儲存** 如果要撤消對任務清單所做的更改。

      ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

      執行下列動作：

      1. 選擇要刪除的任務。
      1. 按一下 **刪除**.
      1. （選用）按一下 **還原** 以撤消更改，而不刪除任務。
      1. 按一下 **取消復原** 如果要保留更改並刪除任務。
      1. 按一下 **儲存** 刪除任務。

         只有在保存更改後，才會刪除任務。


### 刪除單個任務 {#delete-a-single-task}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **專案**.
1. 按一下包含您要刪除任務的項目名。
1. 按一下 **工作** 在左邊。
1. 按一下要刪除的任務的名稱。
1. 按一下 **更多** 圖示 ![](assets/qs-more-menu.png)在右上角。

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. 按一下 **刪除任務**.
1. 如果允許刪除，請按一下 **是，刪除它**.

   您的Workfront管理員或群組管理員可能不允許刪除記錄小時的任務。

   有關刪除任務所需的訪問權限和權限的詳細資訊，請參閱部分 [刪除任務的限制](#limitations-for-deleting-tasks) 這篇文章。

## 還原已刪除的任務

Workfront或群組管理員可在任務刪除後30天內還原任務，如 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
