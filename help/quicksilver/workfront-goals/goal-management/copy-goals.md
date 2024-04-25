---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中複製目標
description: 您可以複製Adobe Workfront目標中的目標來建立目標。 部分原始目標資訊會轉移至新目標。
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 4%

---

# 在Adobe Workfront目標中複製目標

您可以複製Adobe Workfront目標中的目標來建立目標。 部分原始目標資訊會轉移至新目標。

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
 <p>新授權：投稿人或以上版本</p>
 或
 <p>目前授權：要求或以上</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>.</p> </td>
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
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  <p>如需關於共用目標的資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 複製目標的考量事項

在複製目標之前，您必須擁有存取層級中「編輯目標」的存取權。 如需授與目標存取權的相關資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

您可能想要複製現有目標的一些原因包括：

* 在時段（季或年）結束時，當您想要為下一個時段重新建立相同的目標時。
* 在時段結束時，當目標無法完成，並且您想要在另一個時段處理它時。
* 當多個團隊成員具有類似目標時，您可能需要為每個團隊成員建立一個目標。

>[!TIP]
>
>您可以複製任何狀態下的目標。 如需目標狀態的詳細資訊，請參閱 [Adobe Workfront目標中的目標狀態概觀](../../workfront-goals/goal-management/goal-status-overview.md).

複製目標時，請考量下列事項：

* 有關目標的所有資訊也會複製到新目標。
* 您可以選擇複製現有目標的結果。 結果名稱會轉移至新目標，但現有目標上的結果目前進度不會複製到新目標。 依預設，複製的結果會指派給相同的擁有者。

  >[!NOTE]
  >
  >如果從Workfront中刪除或停用原始擁有者，則會將新結果指派給登入使用者。

* 當您複製目標時，無法複製目標的活動。

## 複製目標

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. 前往目標並按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **複製目標**.

   ![](assets/copy-goal-box-unshimmed.png)

1. 針對複製的目標更新下列資訊：
   * **目標名稱**：新目標的名稱。 複製目標的預設名稱是「副本」 &lt;original goal=&quot;&quot;>「。
   * **期間**：您要達到目標的時段。 從下拉式功能表中選取時段

     或

     選取 **啟用自訂日期** 若要指定目標的自訂日期 **開始** 和 **結束日期**. 啟用自訂日期設定預設為停用。

     >[!TIP]
     >
     >   取消選取「啟用自訂日期」將還原為原始目標的時段。

      * **目標所有者**：目標的擁有者。 可以是使用者、團隊、群組或公司。 預設為原始目標的所有者。
      * **說明**：目標的其他資訊。
      * **複製結果**：如果您要將目前目標的結果傳輸至複製的目標，請選取此選項。 這樣會複製原始結果，並將它們附加到複製的目標。 所複製目標的結果與原始目標的結果的所有者、名稱和測量值均相同。

        >[!NOTE]
        >
        >* 原始結果的進度不會轉移到複製的目標。
        >* 如果從Workfront中刪除或停用原始擁有者，則會將新結果指派給登入使用者。

1. 按一下 **複製目標**.

   與原始目標類似的目標已建立且處於「草稿」狀態。

   >[!NOTE]
   >
   >如果您尚未從原始目標複製結果，則必須先將新目標與進度指示器建立關聯，然後才能啟動並開始努力實現目標。
   >如需將目標與進度指標建立關聯的資訊，請參閱下列文章：
   >* [在Adobe Workfront目標中新增結果](../results-and-activities/add-results-to-goals.md)
   >* [將活動新增至Adobe Workfront目標中的目標](../results-and-activities/add-activities-to-goals.md)
   >* [透過在Adobe Workfront目標中連線目標來對齊目標](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >如需啟用目標的詳細資訊，請參閱 [啟用目標](../goal-management/activate-goals.md).

