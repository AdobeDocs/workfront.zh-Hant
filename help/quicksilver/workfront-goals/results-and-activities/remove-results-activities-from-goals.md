---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 從Adobe Workfront目標中的目標移除進度指示器
description: 當結果、活動和專案不再相關時，您可以從Adobe Workfront目標中的目標中將其移除。
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# 從Adobe Workfront目標中的目標移除進度指示器

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

如果結果、活動和專案不再相關，您可以從目標中將其移除。

如需建立目標及將結果和活動新增至目標的相關資訊，請參閱下列文章：

* [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)
* [在Adobe Workfront目標中新增活動](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [將結果新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [在Adobe Workfront目標中編輯結果和活動](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

目標也可以與父目標校準，成為子目標。 子目標也是父目標的進度指示器。

您可以透過移除目標之間的連線來移除目標之間的對齊方式。 如需詳細資訊，請參閱[移除Adobe Workfront目標中的目標校準](../goal-alignment/remove-goal-alignment.md)。

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

## 先決條件

您必須擁有與結果、活動或專案相關聯的目標。

## 移除結果、活動和從目標中斷專案連線的考量事項

* 您只能從作用中的目標移除結果和活動。
* 您可以刪除結果和活動，以將其從目標中移除。 已刪除的結果和活動無法復原。
* 當您從目標中移除結果或活動時，移除結果或活動的進度會影響目標的整體進度。
* 您無法從目標刪除專案，但可以從目標中斷專案的連線。 透過從目標中斷專案連線，專案的完成百分比不再影響目標的進度。

  如需有關專案如何影響目標進度的資訊，請參閱[在Adobe Workfront目標中新增專案](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)。

* 您無法從目標移除結果或活動，也無法中斷子目標或專案的連線（如果子目標或專案是目標的最後一個進度指示器）。
* 如果專案從「專案」區域刪除，且它是目標的最後一個進度指示器，則目標會變為「非使用中」。

## 從目標中刪除結果和活動

您可以透過刪除來從目標中移除結果和活動。 從目標中刪除結果和活動是相同的。

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. 按一下右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   如此將可開啟Workfront目標區域，且預設會顯示目標清單。

1. 按一下您要從中移除結果和活動的目標名稱。

   如此將可開啟目標頁面。

1. 按一下左側面板中的&#x200B;**進度指示器**。

1. 選取結果或活動，然後按一下清單頂端的&#x200B;**刪除**&#x200B;圖示![](assets/delete-icon.png)。

1. 按一下&#x200B;**刪除**&#x200B;以確認刪除。 結果或活動已刪除且無法復原。 目標的完成百分比會更新，以排除已刪除的活動或結果。


## 從目標中移除專案

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. 按一下右上角的&#x200B;**主要功能表**&#x200B;圖示，然後按一下&#x200B;**目標**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   如此將可開啟Workfront目標區域，且預設會顯示目標清單。

1. 按一下您要從中移除結果和活動的目標名稱。

   如此將可開啟目標頁面。
1. 按一下左側面板中的&#x200B;**進度指示器**。
1. 選取專案，然後按一下清單頂端的&#x200B;**中斷連線**&#x200B;圖示![](assets/disconnect-icon.png)。
1. 按一下&#x200B;**中斷連線**&#x200B;以確認。

   專案不再連線至目標。 目標更新的完成百分比會排除已中斷連線的專案。

