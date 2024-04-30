---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 在Adobe Workfront目標中新增結果
description: 結果會衡量目標的進度。 若未將結果、活動或校準的目標與目標建立關聯，您就無法啟動目標，也無法記錄其進度。
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 3%

---

# 在Adobe Workfront目標中新增結果

結果會衡量目標的進度。 若未將結果、活動或校準的目標與目標建立關聯，您就無法啟動目標，也無法記錄其進度。

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
 <td role="rowheader"><p>存取層級</p></td>
 <td> <p>編輯目標的存取權</p>  </td>
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

## 先決條件

開始之前，您必須具備下列條件：

* 包含主功能表中目標區域的版面配置範本。
* 現有目標。

  如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>一個目標不能有超過1000個活動、結果、專案或校準的目標。

## 將結果新增到目標中

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. 按一下主功能表 ![](assets/main-menu-icon.png)，然後 **目標**.

1. 從 **目標清單**，按一下目標的名稱以開啟目標頁面。
1. 按一下 **進度指示器** 在左側面板中。
1. 展開 **新進度指示器** 下拉式功能表，然後按一下 **建立結果**.

   「新建結果」方塊開啟。

   ![](assets/new-result-box-unshimmed.png)

1. 輸入結果的名稱，在 **結果名稱** 欄位。 這是必填欄位。
1. （可選）將您的名稱從 **結果擁有者** 欄位。 依預設，您是您建立之活動的擁有者。

   >[!NOTE]
   >
   >您無法將團隊、群組或公司指派為結果擁有者。

1. 在 **您要如何測量結果？** 區域，指定下列資訊：
   * **值型別**：這會指示您想要如何測量結果的進度。 您可以使用百分比值或貨幣金額以數值方式測量進度。

     從下表列出的選項中選取值型別：

     | 值類型 | 說明 |
     |---------------------------------------------------------|------------------|
     | 數字 | 數值 |
     | % | 百分比值 |
     | CN¥、DKK、KR、Mex$、R、$、 zl、 £ 、 € 、 ₹、 ฿、 MYR、 ₪、$ | 貨幣值 |

   * **初始值**：結果在記錄其任何進度之前在開始時的值。
   * **目標值**：視為完成時結果預計達到的值。
1. 按一下 **建立結果**.

   結果會顯示在目標頁面的「進度指示器」區段的「結果」群組下。

   啟動目標後，當您更新結果的進度時，目標的進度會自動更新。 如需啟用目標的詳細資訊，請參閱 [在Adobe Workfront目標中啟用目標](../goal-management/activate-goals.md).
