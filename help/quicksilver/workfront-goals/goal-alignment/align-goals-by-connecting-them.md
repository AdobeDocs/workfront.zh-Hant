---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 透過在Adobe Workfront目標中連線目標來對齊目標
description: 如果您是有個人目標的個人投稿人，您可能希望將其與團隊的目標一致，以便在組織策略的大背景中有效顯示您自己目標的進度。
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# 透過在Adobe Workfront目標中連線目標來對齊目標

如果您是有個人目標的個人投稿人，您可能希望將其與團隊的目標一致，以便在組織策略的大背景中有效顯示您自己目標的進度。

當貴組織中的每個人都將目標與貴組織的目標一致時，他們可以清楚瞭解其個人貢獻和團隊努力如何有助於推動大型公司層級優先順序的進展。 如需調整目標之最佳實務的詳細資訊，請參閱 [Adobe Workfront目標中的目標對齊方式概觀](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

在Adobe Workfront目標中連結目標的方法有兩種：

* 您可以藉由將目標相互連線來建立目標之間的對齊方式。

* 您可以手動對齊兩個目標，也可以將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。

>[!IMPORTANT]
>
>一個目標總共可以有1000個進度指示器。

本文說明如何藉由將目標相互連線來對齊目標。 如需有關透過將結果和活動轉換為目標來調整目標的資訊，請參閱 [透過將結果和活動轉換為目標來校準目標](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront計畫</td>
 <td>
 <p>任何</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront授權*</td>
 <td>
 <p>目前授權：投稿人或以上版本</p>
 或
 <p>舊版授權：要求或更高版本</p> </td>
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
 <tr>
 <td role="rowheader">物件許可權</td>
 <td>

<p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  <p>如需關於共用目標的資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 藉由將目標相互連線來對齊目標

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. 建立您要對齊的兩個目標。 如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).
1. （可選）啟動您要對齊的目標。 您可以對齊狀態為「草稿」、「作用中」或「非作用中」的目標。 如需啟用目標的詳細資訊，請參閱 [在Adobe Workfront目標中啟用目標](../../workfront-goals/goal-management/activate-goals.md).
1. 移至您要對齊（子系目標）至其他目標（父系目標）的目標，然後按一下其名稱以開啟目標頁面。

   >[!INFO]
   >
   >例如，如果您希望目標2影響目標1的進度，則必須前往目標2。

1. 按一下 **目標詳細資料** 在左側面板中。

1. 在 **上層目標資訊** 區域，按一下 **新增** 在 **上層目標** 欄位若沒有上層目標，

   或

   按一下上層目標的名稱以選擇其他目標。

1. 開始在「 」中輸入現有目標的名稱 **上層目標** 欄位，然後在其出現在清單中時選取它。 清單中只會顯示相同或未來期間的目標。

1. 按一下「**儲存變更**」。

   您一開始的目標（目標2）現在是將它與（目標1）對齊之父目標的子目標。\
   校準的目標會顯示在「目標校準」區段中，以目標2作為目標1的次要。
當子目標的進度更新父目標的進度時，其進度會顯示在父目標的進度指示器區段中。

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. （可選）若要檢視「目標校準」區段中的目標，請前往Workfront的目標區域，然後按一下 **目標校準** 區段。 如需「目標校準」區段的詳細資訊，請參閱 [導覽Adobe Workfront目標中的「目標校準」區段](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. （選用）將活動和結果新增至任一目標以指出其進度。 如需新增活動和結果的資訊，請參閱下列文章：

   * [將活動新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [在Adobe Workfront目標中新增結果](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. （可選）當您認為與您組織的整體策略不再相關時，請移除兩個目標之間的對齊方式。 如需有關移除目標間對齊方式的資訊，請參閱 [移除Adobe Workfront目標中的目標校準](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

