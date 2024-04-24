---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 移除Adobe Workfront目標中的目標校準
description: 如果兩個目標之間的連線不再合理，您可以移除它們之間的對齊。
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 1%

---

# 移除Adobe Workfront目標中的目標校準

如果兩個目標之間的連線不再合理，您可以移除它們之間的對齊。

如需對齊目標的資訊，請參閱下列文章：

* [透過在Adobe Workfront目標中連線目標來對齊目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [透過將結果和活動轉換為目標來校準目標](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
   <p>新計畫：選取或更高</p>
   或
   <p>目前計畫：專業或以上版本</p>
   
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
   <p>目前產品需求： Adobe Workfront Goals的Workfront計畫和額外授權。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">存取層級</td>
   <td> <p>編輯目標的存取權</p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">物件許可權</td>
   <td>
    <p>檢視目標或更高許可權以檢視它</p>
     <p>管理目標的許可權以編輯它</p>
     <p>如需關於共用目標的資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p>
    </td>
  </tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
 </tbody>
</table>

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. Click the **gear icon** ![](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. 存取 **目標** Workfront區域，然後按一下目標的名稱以開啟目標的頁面。
1. 從上層目標的目標頁面，按一下 **進度指示器** 在左側面板中。

   ![](assets/remove-goal-alignment-from-list-unshimmed.png)

1. 在 **型別：目標** 分組，選取目標，然後按一下 **中斷連線** 圖示 ![](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) 在清單頂端。

   會顯示[Disconnect]方塊。

1. 按一下 **中斷連線** 以中斷所選目標與其父項的連線。

   目標會變成獨立目標，不再列為原始目標的進度指示器。 已中斷連線目標的進度不再影響原始目標的進度。

   成功訊息會顯示在頁面的右上角，以確認目標已中斷連線。