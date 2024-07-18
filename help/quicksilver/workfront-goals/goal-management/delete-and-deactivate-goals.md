---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: 刪除和停用Adobe Workfront目標中的目標
description: 當您開始處理目標且它在您的組織中變得無關時，我們建議您將其停用，而非刪除。 停用目標會保留其歷史資訊，並讓您有機會稍後重新啟用。 但是，有時候刪除目標可能很合理，為了保持您的目標清單準確。
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# 刪除和停用Adobe Workfront目標中的目標

當您開始處理目標且它在您的組織中變得無關時，我們建議您將其停用，而非刪除。 停用目標會保留其歷史資訊，並讓您有機會稍後重新啟用。 但是，有時候刪除目標可能很合理，為了保持您的目標清單準確。

## 存取需求

您必須具備下列條件：

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
  <ul><li>終極計畫 </li>
  或
  <li>適用於Prime或選取Adobe Workfront計畫的Adobe Workfront目標的其他授權。 </li></ul> </p>
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
 <p>目前授權：要求或以上</p> </td>
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
 <td role="rowheader"><p>存取層級</p></td>
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

## 停用目標

您可以停用不再相關且將來可能想要重新啟用的目標。

* [停用目標時的考量事項](#considerations-when-deactivating-goals)
* [停用目標](#deactivate-goals)

### 停用目標時的注意事項

停用目標時，請記住下列事項：

* 您只能停用處於作用中狀態的目標。 如需啟用目標的相關資訊，請參閱[在Adobe Workfront目標中啟用目標](../../workfront-goals/goal-management/activate-goals.md)。

  >[!TIP]
  >
  >您無法停用「草稿」狀態下的目標。

* Workfront停止計算已停用目標的進度。
* 非作用中目標不再顯示於，或在Workfront目標的「圖表」區段中予以考慮。 如需Workfront目標圖表的相關資訊，請參閱[檢閱圖表以瞭解Adobe Workfront目標中的目標進度趨勢](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md)。

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* 您無法再對停用的目標進行更新。
* 您可以編輯有關目標及其對齊方式的資訊。
* 您可以重新啟用先前已停用的目標。

### 停用目標

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. 按一下右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。

   目標清單隨即顯示。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. （可選）修改您的篩選器以僅顯示作用中的目標。

   如需在Workfront目標中篩選資訊的詳細資訊，請參閱[在Adobe Workfront目標中篩選資訊](../goal-management/filter-information-wf-goals.md)。

1. 按一下作用中的目標。

   目標頁面隨即開啟。

   ![](assets/goal-page-unshimmed.png)

1. 按一下目標名稱右邊的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**停用**。

1. 目標已停用，其狀態變為非使用中。

## 刪除目標

您可以刪除不再相關或可能永遠不會相關的目標。

* [刪除目標時的考量事項](#considerations-when-deleting-goals)
* [刪除目標](#delete-goals)

### 刪除目標時的注意事項 {#considerations-when-deleting-goals}

* 您可以刪除任何狀態下的目標，包括已關閉的目標。
* 您無法復原已刪除的目標。
* 附加至目標的結果和手動進度列活動也會被刪除。
* 不會刪除與目標相關聯的專案，但會移除其與目標的關聯。

### 刪除目標

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. 按一下右上角的「主要功能表」圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。

   目標清單隨即顯示。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 按一下目標的名稱。 如此將可開啟目標頁面。
1. 按一下目標名稱右邊的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**刪除目標**，再按一下&#x200B;**刪除**。

   目標及其活動和結果也會遭到刪除且無法復原。 不會刪除與一個或多個子目標相關聯的專案。


