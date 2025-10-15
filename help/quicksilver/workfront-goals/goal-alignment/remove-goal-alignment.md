---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 移除Adobe Workfront目標中的目標校準
description: 如果兩個目標之間的連線不再合理，您可以移除它們之間的對齊。
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 1%

---

# 移除Adobe Workfront目標中的目標校準

<!--Audited P&P only: 4/2025-->

如果兩個目標之間的連線不再合理，您可以移除它們之間的對齊。

如需對齊目標的資訊，請參閱下列文章：

* [在Adobe Workfront目標中連線目標以對齊目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [透過將結果和活動轉換為目標來校準目標](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## 存取需求

>[!NOTE]
>
>如果貴公司過去曾購買此套件，他們可能會選擇繼續使用Adobe Workfront目標。 如需詳細資訊，請洽詢客戶代表。
>
>Adobe Workfront目標不再提供購買。

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront套件</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <td role="rowheader">Adobe Workfront授權</td>
 <td>
 <p>投稿人或以上</p>
 <p>要求或更高版本</p> </td>
 </tr>
  <tr>
 <td role="rowheader">存取層級</td>
 <td> <p>編輯目標的存取權</p> </td>
 </tr>
 <tr>
 <td role="rowheader">物件許可權</td>
 <td>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>

</td>
 </tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者（包括系統管理員）指派一個版面配置範本，該範本包括主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++
<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront plan*</td>
 <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
   Or
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 先決條件

開始之前，您必須具備下列條件：

* 至少有一個相關聯子目標的父目標。 子目標是目標的進度指示器。

## 移除目標對齊的相關考量事項

移除兩個目標之間的對齊方式時，請考量下列事項：

* 上層目標必須具有與其相關的其他目標、活動或結果，才能保持作用中。
* 如果校準的子目標是父目標的唯一進度指示器，則無法從父目標中移除校準的子目標。
* 當您移除與上層目標的對齊方式時，子目標會成為獨立目標。

## 移除目標一致性

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. 存取Workfront中的&#x200B;**目標**&#x200B;區域，然後按一下目標的名稱以開啟目標的頁面。
1. 從上層目標的目標頁面，按一下左側面板中的&#x200B;**進度指示器**。

   ![重新移動目標校準](assets/remove-goal-alignment-from-list-unshimmed.png)

1. 在&#x200B;**型別：目標**&#x200B;群組中，選取目標，然後按一下清單頂端的&#x200B;**中斷連線**&#x200B;圖示![中斷連線圖示](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png)。

   會顯示[Disconnect]方塊。

1. 按一下&#x200B;**中斷連線**，將選取的目標與其父系中斷連線。

   目標會變成獨立目標，不再列為原始目標的進度指示器。 已中斷連線目標的進度不再影響原始目標的進度。

   成功訊息會顯示在頁面的右上角，以確認目標已中斷連線。
