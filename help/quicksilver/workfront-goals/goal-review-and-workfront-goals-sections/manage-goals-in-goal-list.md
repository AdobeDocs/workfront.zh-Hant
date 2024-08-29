---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 管理Adobe Workfront目標之目標清單中的目標
description: 在您或其他使用者建立目標後，可以在「目標清單」中檢閱其進度和資訊。 如需建立目標的相關資訊，請參閱在Adobe Workfront目標中建立目標。
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 2%

---

# 管理Adobe Workfront目標之目標清單中的目標

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

在您或其他使用者建立目標後，可以在「目標清單」中檢閱其進度和資訊。 如需建立目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。

## 存取需求

您必須具有下列存取權才能執行本文所述的動作：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> 
   <p>對於新計畫和授權結構：
  <ul><li>終極計畫 </li></ul>
   </p>
<p>對於目前的計畫與授權結構： 
<ul><li> A Pro或更高版本 </li>
  <li>除了Adobe Workfront授權之外，還有Workfront目標授權。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront授權*</td>
 <td>
 <p>新授權：投稿人或以上版本</p>
 或
 <p>目前授權：要求或以上</p> <p>如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
 <p> 新產品需求，下列其中一項： </p>
<ul>
<li>Select或Prime Adobe Workfront計畫以及額外的Adobe Workfront目標授權。</li>
<li>預設包含Workfront目標的Ultimate Workfront計畫。 </li></ul>
 <p>或</p>
 <p>目前產品需求： Adobe Workfront Goals的Workfront計畫和額外授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">存取層級</td>
 <td> <p>編輯目標的存取權</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  <p>如需共用目標的相關資訊，請參閱<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>。 </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 管理目標清單中的目標

您可以在Workfront目標的下列區段中檢視和管理目標：

* 目標清單
* 目標校準

每個區段都會以稍微不同的格式顯示目標。 您使用哪個區段取決於您在使用目標時想要達到的目的。

如需詳細資訊，請參閱[ Adobe Workfront目標區段概觀](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)。

本文說明如何檢閱目標清單中的目標。

檢閱目標清單時，請考量下列事項：

* 您可以檢視您或組織中其他人在目標清單中建立的目標。 您必須擁有目標的管理許可權才能編輯目標。

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

若要管理「目標清單」中的目標：

1. 按一下右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   預設會顯示「目標清單」區段。 依預設，您可以檢視目標，而不論其狀態、期間或擁有者為何。

   目標清單包含以下欄位，其中包含每個目標的相關資訊：

   * **名稱**：目標的名稱。
   * **所有者**：目標所有者的名稱。
   * **期間**：目標排定的期間。
   * **狀態**：目標的狀態可以是下列其中一項：
      * 啟用中
      * 草稿
      * 停用中
      * 已關閉

     如需目標狀態的相關資訊，請參閱Adobe Workfront目標中的[目標狀態總覽](../goal-management/goal-status-overview.md)。

     對齊圖示會出現在與其他目標對齊的目標上。 如需對齊目標的資訊，請參閱[在Adobe Workfront目標中連線來對齊目標](../goal-alignment/align-goals-by-connecting-them.md)。

   * **條件**：目標在配置給目標完成的時段內進度之視覺化表示。

     目標的條件可以是下列其中一項：

      * 新增
      * 達成目標
      * 有風險
      * 陷入困境

     如需目標條件的詳細資訊，請參閱[Adobe Workfront目標中的目標進度和條件概觀](../goal-management/calculate-goal-progress.md)。

   * **進度**：目標的進度指示器百分比值。 進度指示器的顏色符合目標條件的顏色。

     如需詳細資訊，請參閱[在Adobe Workfront目標中計算目標進度](../goal-management/calculate-goal-progress.md)。

1. 按一下目標清單右上角的篩選器圖示![](assets/filter-icon.png)，然後套用篩選器以僅顯示對您重要的目標。

   如需在Workfront目標中使用篩選器的相關資訊，請參閱[Adobe Workfront目標中的篩選資訊](../goal-management/filter-information-wf-goals.md)。

1. 按一下欄標題中的任何欄位，即可依該欄位排序清單。
欄位右側會顯示一個箭頭，清單會依此箭頭排序。

1. （選用）再按一下欄中的欄位，以遞減順序排序相同的欄。
1. 按一下目標的名稱以開啟目標的頁面。
1. 在清單中選取一個目標，然後按一下清單頂端的下列其中一個選項：
   * **編輯**&#x200B;圖示![](assets/edit-icon.png)以編輯目標的相關資訊。 如需詳細資訊，請參閱[在Adobe Workfront目標中編輯目標](../goal-management/edit-goals.md)。
   * **共用**&#x200B;圖示![](assets/share-icon.png)以與其他人共用目標。 如需詳細資訊，請參閱[在Adobe Workfront目標中共用目標](../workfront-goals-settings/share-a-goal.md)。
   * **開啟對齊方式**&#x200B;圖示![](assets/align-icon-unshimmed.png)以開啟目標對齊方式區域。 只有在您選取的目標已對齊另一個目標時，才會顯示此選項。
   * **刪除**&#x200B;圖示![](assets/delete-icon.png)以刪除目標，然後按一下&#x200B;**刪除**&#x200B;以確認。  如需詳細資訊，請參閱[在Adobe Workfront目標中刪除及停用目標](../goal-management/delete-and-deactivate-goals.md)。





