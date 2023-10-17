---
title: 刪除專案
product-area: projects
navigation-topic: manage-projects
description: 如果不再需要專案及其資料，您可以刪除該專案。
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 1%

---

# 刪除專案

如果不再需要專案及其資料，您可以刪除該專案。

建議您編輯專案並將狀態變更為「完成」或「廢棄」，作為刪除專案的替代方法。 這會從使用者的任務清單中移除與專案相關的所有目前任務，但儲存與專案相關的所有資料。

## 存取需求

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對專案、任務、問題的存取權，並具備刪除專案、任務和問題的能力</p> <p><b>附註</b></p>

<p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權、專案上的任務和問題，並可刪除專案、任務和問題。 </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。
您可以刪除專案清單中的專案或專案層級的專案。

## 瞭解刪除專案的程式

* [刪除專案的限制](#limitations-for-deleting-projects)
* [刪除專案的影響](#the-impact-of-deleting-projects)

### 刪除專案的限制  {#limitations-for-deleting-projects}

* 刪除的專案會移至資源回收筒並保留30天，且只有Workfront管理員才能復原。

  如需有關還原物件的詳細資訊，請參閱文章 [還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 如果專案具有任務或問題，記錄時數，Workfront或群組管理員必須透過在您的Workfront執行個體中設定任務和問題偏好設定，以允許刪除這些任務，您才能刪除包含任務的專案。

  如需有關啟用刪除記錄時數的任務、問題或專案的詳細資訊，請參閱以下的「刪除」一節： [設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### 刪除專案的影響 {#the-impact-of-deleting-projects}

* 刪除專案時，會影響連結至專案的其他物件。

  當您刪除專案時，也會刪除附加至專案的下列物件：

   * 文件

     您無法刪除具有已出庫之附加檔案的專案。 如需出庫檔案的詳細資訊，請參閱 [簽出檔案](../../../documents/managing-documents/check-out-documents.md).

   * 任務
   * 子任務
   * 問題
   * 更新
   * 核准
   * 費用
   * 風險
   * 基準線
   * 業務案例資訊
   * 佇列詳細資訊
   * 收費率
   * 付費記錄

     您無法刪除記帳記錄狀態為「已記帳」的專案。 如需詳細資訊，請參閱 [建立付費記錄](../../projects/project-finances/create-billing-records.md).

* 根據Workfront管理員在Workfront執行個體的時程表和小時偏好設定中設定專案、任務或問題刪除偏好設定的方式，任務、問題或專案的記錄小時會在刪除專案時以下列方式之一處理：

   * 小時會作為一般時間保留在時程表中。
   * 時數會遭到刪除，如果專案已還原，則會還原時數。

  如需針對登入問題時數設定刪除偏好設定的詳細資訊，請參閱 [設定時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 如果您刪除的專案連結至「Workfront情境規劃工具」中的方案：

   * 方案會保留在計畫上，但專案的連結會被移除。
   * 如果您刪除的專案連結至計畫中唯一發佈的方案，則也會移除已發佈計畫的指示。
   * 如果您復原已刪除的專案，專案將會復原，但其方案連結並未復原，且「情境規劃工具」區域不再顯示在「專案詳細資料」中。

     Scenario Planner僅在新的Adobe Workfront體驗中可用，並且需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱 [情境規劃工具概觀](../../../scenario-planner/scenario-planner-overview.md).

     如需「情境規劃工具」中連結至方案的專案相關資訊，請參閱 [透過在情境規劃工具中發佈行動方案來更新或建立專案](../../../scenario-planner/publish-scenarios-update-projects.md).

* 如果專案也是Workfront目標中的目標活動：

   * 專案會從目標中刪除。 專案在目標上指出的進度也會被移除。

   * 如果您復原已刪除的專案，該專案也會還原為目標活動。

     這需要額外的授權。 如需Workfront目標的相關資訊，請參閱 [Adobe Workfront目標總覽](../../../workfront-goals/goal-management/wf-goals-overview.md).

     如需將專案與目標建立關聯的資訊，請參閱 [在Adobe Workfront目標中新增專案](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## 刪除清單中的專案

您可以從專案清單中刪除專案。

1. 前往專案清單或專案報告。
1. 選取您要刪除的一或多個專案，然後按一下 **刪除** 圖示 ![](assets/delete-icon.png) 在清單頂端。

1. 按一下 **是的，刪除** 以確認刪除。

   專案會刪除並儲存在資源回收筒中30天。 在此期間，您的Workfront管理員可以從資源回收筒還原已刪除的專案。

## 刪除專案層級的專案

1. 前往您要刪除的專案。
1. 按一下 **更多** 圖示 ![](assets/qs-more-menu.png)，然後按一下 **刪除專案**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. 按一下 **是的，刪除**.

   專案會刪除並儲存在資源回收筒中30天。 在這段期間，您的Workfront管理員可以從資源回收筒將其還原。

## 還原已刪除的專案

系統或群組管理員可在刪除專案後30天內還原專案，如文章所述 [還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
