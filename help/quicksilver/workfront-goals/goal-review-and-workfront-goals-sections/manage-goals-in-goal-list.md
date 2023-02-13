---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 管理Adobe Workfront目標目標清單中的目標
description: 在您或其他使用者建立目標後，您可以在目標清單中檢閱其進度和資訊。 如需建立目標的相關資訊，請參閱在Adobe Workfront目標中建立目標。
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 2%

---

# 管理Adobe Workfront目標目標清單中的目標

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

在您或其他使用者建立目標後，您可以在目標清單中檢閱其進度和資訊。 如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).

## 存取需求

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

您必須具備下列存取權，才能執行本文所述的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td> <p>您必須購買額外的Adobe Workfront目標授權才能存取本文所述的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>檢視或更高程度地存取目標</p> <p><b>附註</b><p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> 
    <div> 
     <p>檢視目標的或更高權限</p> 
     <p>如需共用目標的相關資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須具備下列條件，才能開始：

* 一種佈局模板，在主菜單中包括目標區域。

## 管理目標清單中的目標

您可以在下列Workfront目標章節中檢視及管理目標：

* 目標清單
* 目標校準

每個區段會以稍微不同的格式顯示目標。 您使用哪個區段取決於您處理目標時所要達到的目的。

如需詳細資訊，請參閱 [Adobe Workfront目標章節概覽](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

本文說明如何檢閱目標清單中的目標。

檢閱目標清單時，請考量下列事項：

* 您可以檢視您或組織中其他任何人在目標清單中建立的目標。 您必須擁有目標的「管理」權限，才能編輯目標。

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

要管理目標清單中的目標：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)  在右上角，按一下 **目標**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   預設會顯示「目標清單」區段。 依預設，您可以檢視目標，而不論其狀態、期間或擁有者為何。

   目標清單包含下列欄位，其中包含每個目標的相關資訊：

   * **名稱**:目標的名稱。
   * **擁有者**:目標所有者的名稱。
   * **時段**:排程目標的時段。
   * **狀態**:目標的狀態可以是下列其中一項：
      * 使用中
      * 草稿
      * 非使用中
      * 已關閉

      如需目標狀態的相關資訊，請參閱 [Adobe Workfront目標中的目標狀態概觀](../goal-management/goal-status-overview.md).

      對齊圖示會顯示在與其他目標對齊的目標上。 如需協調目標的相關資訊，請參閱 [在Adobe Workfront目標中將目標連結起來，以協調目標](../goal-alignment/align-goals-by-connecting-them.md).

   * **條件**:目標在分配給目標完成的時段內如何前進的視覺表示。

      目標的條件可能是下列其中一項：

      * 新增
      * 達成目標
      * 有風險
      * 陷入困境

      如需目標條件的相關資訊，請參閱 [Adobe Workfront目標中的目標進度和條件概覽](../goal-management/calculate-goal-progress.md).

   * **進度**:目標的進度指標，以百分比值表示。 進度指標的顏色與目標條件的顏色匹配。

      如需詳細資訊，請參閱 [計算Adobe Workfront目標中的目標進度](../goal-management/calculate-goal-progress.md).



1. 按一下篩選圖示 ![](assets/filter-icon.png) 在目標清單的右上角，並套用篩選器以僅顯示對您而言重要的目標。

   如需在Workfront目標中使用篩選器的相關資訊，請參閱 [篩選Adobe Workfront目標中的資訊](../goal-management/filter-information-wf-goals.md).

1. 按一下欄標題中的任何欄位，依該欄位排序清單。
欄位右側會顯示一個箭頭，依此箭頭排序清單。

1. （選用）再按一下欄中的欄位，以降序排序相同的欄。
1. 按一下目標名稱以開啟目標的頁面。
1. 在清單中選取一個目標，然後按一下清單頂端的下列其中一個選項：
   * **編輯** 圖示 ![](assets/edit-icon.png) 編輯目標的相關資訊。 如需詳細資訊，請參閱 [編輯Adobe Workfront目標](../goal-management/edit-goals.md).
   * **共用** 圖示 ![](assets/share-icon.png) 與他人分享目標。 如需詳細資訊，請參閱 [在Adobe Workfront目標中共用目標](../workfront-goals-settings/share-a-goal.md).
   * **開放對齊** 圖示 ![](assets/align-icon-unshimmed.png) 以開啟「目標對齊」區域。 只有當您選取的目標對齊至其他目標時，才會顯示此選項。
   * **刪除** 圖示 ![](assets/delete-icon.png) 若要刪除目標，請按一下 **刪除** 確認。  如需詳細資訊，請參閱 [刪除和停用Adobe Workfront目標中的目標](../goal-management/delete-and-deactivate-goals.md).





