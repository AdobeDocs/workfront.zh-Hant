---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 在Adobe Workfront目標中將目標連結起來，以協調目標
description: 如果您是具有個人目標的個別貢獻者，您可能會想要將其與團隊的目標一致，以便在組織策略的更大情境中有效顯示您自己目標的進度。
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 在Adobe Workfront目標中將目標連結起來，以協調目標


如果您是具有個人目標的個別貢獻者，您可能會想要將其與團隊的目標一致，以便在組織策略的更大情境中有效顯示您自己目標的進度。

當組織中的每個人的目標都與組織的目標一致時，他們就能清楚了解他們的個人貢獻和團隊努力如何協助推進更大、公司層級的優先事項。 如需協調目標的最佳實務的詳細資訊，請參閱 [Adobe Workfront目標中的目標對齊概觀](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

將Adobe Workfront目標中的目標聯繫起來有兩種方法：

* 您可以將目標彼此連結，以建立目標之間的協調。

* 您可以手動協調兩個目標，或者可以將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。

>[!IMPORTANT]
>
>一個目標可以有1 000個進度指標。

本文說明如何將目標彼此連結，以協調目標。 如需將結果和活動轉換為目標以協調目標的相關資訊，請參閱 [通過將結果和活動轉換為目標來協調目標](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## 存取需求

<!--drfated for the P&P release: 

You must have the following:

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

您必須具備下列條件：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯目標的存取權</p> <p><b>附註</b>

<p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> 
    <div> 
     <p>管理目標的權限</p> 
     <p>如需共用目標的相關資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須具備下列條件，才能開始：

* 一種佈局模板，在主菜單中包括目標區域。

## 通過將目標彼此連接來協調目標

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
1. 建立您要協調的兩個目標。 如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).
1. （選用）啟用您要協調的目標。 您可以協調具有「草稿」、「作用中」或「非作用中」狀態的目標。 如需啟用目標的相關資訊，請參閱 [啟用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/activate-goals.md).
1. 前往您要與其他目標（父目標）對齊的目標，然後按一下其名稱以開啟目標頁面。

   >[!INFO]
   >
   >例如，如果希望目標2影響目標1的進度，則必須轉到目標2。

1. 按一下 **目標詳細資訊** 中。

1. 在 **上層目標資訊** 按一下 **新增** 在 **上層目標** 欄位，

   或

   按一下父目標的名稱以選擇另一個目標。

1. 開始在 **上層目標** 欄位，然後在清單中出現時選取它。 清單中只會顯示來自相同或未來期間的目標。

1. 按一下 **儲存變更**.

   您開始的目標（目標2）現在是您與其對齊的父目標的子目標（目標1）。\
   對齊的目標顯示在「目標對齊」區段中，與目標2連結，作為目標1的次要項目。
子目標的進度會隨著其進度更新父目標的進度，而顯示在父目標的「進度指標」區段中。

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. （可選）若要在「目標對齊」區段中檢視目標，請前往Workfront的「目標」區域，然後按一下 **目標對齊** 區段。 如需「目標對齊」區段的相關資訊，請參閱 [導覽Adobe Workfront目標中的「目標對齊」區段](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. （選用）將活動和結果新增至任一目標，以指出其進度。 如需新增活動和結果的相關資訊，請參閱下列文章：

   * [將活動新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [將結果新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. （選用）當您認為與貴組織的整體策略不再相關時，請移除兩個目標之間的協調。 如需移除目標之間對齊方式的相關資訊，請參閱 [移除Adobe Workfront目標中的目標對齊](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

