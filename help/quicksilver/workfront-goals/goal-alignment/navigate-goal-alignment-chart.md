---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 導覽Adobe Workfront目標中的「目標校準」區段
description: 使用「目標校準」區段，在流程圖中顯示整個組織的目標校準整體檢視。 對齊的目標會顯示在階層式樹狀結構中相互連線的卡片上。
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# 導覽Adobe Workfront目標中的「目標校準」區段

<!--Audited P&P only: 4/2025-->

使用「目標校準」區段，在流程圖中顯示整個組織的目標校準整體檢視。 對齊的目標會顯示在階層式樹狀結構中相互連線的卡片上。

如需有關目標對齊方式以及如何達成目標對齊方式的資訊，另請參閱下列文章：

* [Adobe Workfront目標中的目標一致性概觀](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [透過在Adobe Workfront目標中連線目標來對齊目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的活動：

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
  <ul><li>Ultimate計畫 </li></ul>
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
<p>目前授權：要求或以上</p>  </td>
</tr>
<tr>
<td role="rowheader">產品*</td>
<td>
  <p> 新產品需求：Workfront</p>
  或
  <p>目前產品需求：除了Workfront授權之外，您必須購買Adobe Workfront Goals的授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
</tr>
<tr>
<td role="rowheader">存取層級</td>
<td> <p>編輯目標的存取權</p> </td>
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

+++

## 導覽「目標校準」區段

1. 按一下熒幕右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](../goal-alignment/assets/dots-main-menu-icon.png)，然後按一下&#x200B;**目標**。
   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 按一下左側面板中的&#x200B;**目標校準**。
1. 使用對齊圖表右上角的篩選器，僅選取對您而言重要的目標。 如需在Workfront目標中使用篩選器的相關資訊，請參閱[Adobe Workfront目標中的篩選資訊](../../workfront-goals/goal-management/filter-information-wf-goals.md)。

   符合篩選器的目標會顯示在卡片的對齊圖中。

   目標卡片上會顯示下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">時段日期 </td> 
      <td> <p>這是目標開啟的期間。 目標必須在期間的結束日期前達成。 Workfront目標會根據目標期間的持續時間和目前日期計算目標上的進度。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">進度指示器</td> 
      <td>目標的進度指標數目。 進度指標可以是校準的目標、結果或活動。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者名稱</td> 
      <td>指定為目標擁有者的使用者、專案團隊、群組或組織的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目標名稱</td> 
      <td>目標的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目標進度列<span>和進度</span></td> 
      <td> <p>目標進度指出目前已達成的目標程度。 這是根據自目標時段開始以來經過的時間，自動計算目標的所有已校準目標、結果和活動的平均進度。 如需有關計算目標進度的資訊，請參閱<a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目標中的目標進度和條件總覽</a>。 </p> 
       <div> 
        <p>到目前日期的目標實際進度。 下列進度值和顏色表示目標準時達成的可能性： </p> 
        <ul> 
         <li><span>達成目標</span> （綠色指標）：目標準時，將準時達成。</li> 
         <li> <span>有風險</span> （黃色指標）：目標落後，可能無法按時達成。</li> 
         <li> <span>發生問題</span> （紅色指示器）：目標有無法準時實現的危險。 </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td> <p>The date when the goal was last updated</p> <p>(NOTE: drafted because I think this was removed with the alignment chart redesign - 21.1) </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">狀態</td> 
      <td>所有狀態中的<span>目標會顯示在「目標校準」區段中。</span> </td> 
     </tr> 
    </tbody> 
   </table>

   對齊其他目標的目標會在目標卡下顯示對齊的目標數量。

   ![對齊圖表箭頭](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. 按一下目標下方的&#x200B;**向下箭頭**&#x200B;圖示，可進一步展開並檢視子目標。

   ![對齊圖表箭頭](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >將兒童目標對齊的目標會在各自的卡片下顯示對齊的目標數。

1. （條件式）如果目前篩選條件排除參與對齊的某些目標，則會顯示警告訊息，指出並非所有目標都會顯示。

   ![已排除上層目標](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. 按一下&#x200B;**顯示它們**&#x200B;以顯示篩選目前排除的目標。

   在對齊圖中注意下列變更：

   * 之前由篩選器排除的已連線目標現在會顯示在對齊圖表中。
   * 右上角的濾鏡外框為黃色，表示目前未套用濾鏡。

     ![黃色濾鏡反白顯示](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     重新套用篩選器連結會顯示在篩選器名稱的左側。

1. （選擇性）按一下&#x200B;**重新套用篩選器**&#x200B;以返回原始結果並顯示目標階層。
1. （選用）將滑鼠指標暫留在進度指標上，以瞭解當天的目標進度應該位於何處。

   ![將滑鼠移到對齊圖](assets/progress-mouse-over-alignment-chart-350x163.png)上

   下列資訊隨即顯示：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">截至今日</td> 
      <td>進度狀態一律為最新狀態。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>實際</span> </td> 
      <td>根據目前日期計算的目標實際進度（百分比），計算方式為考慮目標上的所有進度指標。 目標進度指標是校準的目標、活動和結果。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預期</td> 
      <td> <p>截至目前日期的目標預期進度（百分比），並假設您將準時達成目標。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下目標卡以開啟目標頁面。 如需有關編輯現有目標的資訊，請參閱[在Adobe Workfront目標中編輯目標](../../workfront-goals/goal-management/edit-goals.md)。 如需有關更新目標進度的資訊，請參閱[在Adobe Workfront目標中更新目標進度](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md)。

1. 按一下目前層級目標的向上箭頭，以返回圖表階層中的上一個層級。

   或

   （選擇性）按一下「**退出目標階層**」以顯示符合目前篩選條件的所有目標卡片，而不會顯示彼此的連線。


