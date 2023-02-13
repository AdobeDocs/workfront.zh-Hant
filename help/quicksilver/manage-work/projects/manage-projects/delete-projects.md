---
title: 刪除專案
product-area: projects
navigation-topic: manage-projects
description: 如果不再需要專案及其資料，您可以刪除專案。
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# 刪除專案

如果不再需要專案及其資料，您可以刪除專案。

除了刪除專案，我們建議您編輯專案，並將狀態變更為「完成」或「已停用」。 這會從用戶的任務清單中刪除與項目相關的所有當前任務，但會保存與項目相關的所有資料。

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
   <td> <p>Edit access to Projects, Tasks,&nbsp;Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列條件才能執行本文所述步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對「項目」、「任務」、「問題」的訪問權，以及刪除項目、任務和問題的功能</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限、工作和專案問題，並能刪除專案、工作和問題。 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。
您可以在專案清單或專案層級刪除專案。

## 了解刪除專案的程式

* [刪除專案的限制](#limitations-for-deleting-projects)
* [刪除專案的影響](#the-impact-of-deleting-projects)

### 刪除專案的限制  {#limitations-for-deleting-projects}

* 已刪除的項目會移至回收筒30天，且只能由Workfront管理員復原。

   有關還原對象的詳細資訊，請參閱文章 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 如果專案有記錄小時的工作或問題，Workfront或群組管理員必須在Workfront例項中設定「任務和問題偏好設定」 ，才能刪除包含工作的專案，以允許刪除這些工作。

   如需有關啟用刪除工作、問題或記錄了小時的專案的詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### 刪除專案的影響 {#the-impact-of-deleting-projects}

* 刪除項目時，會影響連結到項目的其他對象。

   刪除專案時，也會刪除附加至專案的下列物件：

   * 文件

      無法刪除包含已簽出的附加文檔的項目。 有關簽出文檔的詳細資訊，請參閱 [簽出文檔](../../../documents/managing-documents/check-out-documents.md).

   * 任務
   * 子任務
   * 問題
   * 附註
   * 核准
   * 費用

* 根據您的Workfront管理員在Workfront實例的「工時單和小時首選項」中配置項目、任務或問題刪除首選項的方式，在刪除項目時，系統會以以下方式之一處理任務、問題或項目的記錄時數：

   * 小時作為一般時間保留在工時單上。
   * 系統會刪除小時，如果專案已還原，則會還原。

   如需針對記錄問題的數小時設定刪除偏好設定的詳細資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 如果您刪除的項目連結到Workfront方案計畫器中的方案：

   * 該計畫仍在進行中，但與項目的連結被刪除。
   * 如果您刪除的項目連結到計畫中唯一已發佈的計畫，則也會刪除已發佈計畫的指示。
   * 如果恢復已刪除的項目，則將恢復項目，但它與方案的連結不會恢復，方案規劃器區域將不再顯示在項目詳細資訊中。

      方案規劃器僅適用於新的Adobe Workfront體驗，需要額外的許可。 有關Workfront方案計畫器的資訊，請參閱 [方案計畫員概覽](../../../scenario-planner/scenario-planner-overview.md).

      有關在方案計畫器中連結到方案的項目的資訊，請參閱 [通過在方案計畫器中發佈方案來更新或建立項目](../../../scenario-planner/publish-scenarios-update-projects.md).

* 如果專案也是Workfront目標中目標的活動：

   * 項目將從目標中刪除。 項目所指示的目標進度也會被移除。

   * 如果您復原已刪除的專案，專案也會還原為目標的活動。

      這需要額外的授權。 如需Workfront目標的相關資訊，請參閱 [Adobe Workfront目標概覽](../../../workfront-goals/goal-management/wf-goals-overview.md).

      如需將專案與目標關聯的詳細資訊，請參閱 [將專案新增至Adobe Workfront目標中的目標](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## 刪除清單中的專案

您可以從專案清單中刪除專案。

1. 移至專案清單或專案報表。
1. 選取您要刪除的專案，然後按一下 **刪除** 清單頂端。

1. 按一下 **是，刪除它** 以確認刪除。

   項目被刪除並儲存在資源回收筒中30天。 此時，您的Workfront管理員可從資源回收筒還原它。

## 刪除專案層級的專案

1. 前往您要刪除的專案。
1. 按一下 **更多** 圖示 ![](assets/qs-more-menu.png).

1. 按一下 **刪除專案**.

1. 按一下 **是，刪除它**.

   項目被刪除並儲存在資源回收筒中30天。 此時，您的Workfront管理員可從資源回收筒還原它。

## 還原已刪除的專案

系統或組管理員可以在項目刪除後30天內恢復項目，如文章所述 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
