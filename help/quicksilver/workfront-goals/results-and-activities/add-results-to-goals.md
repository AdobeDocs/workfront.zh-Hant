---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 在Adobe Workfront目標中新增結果
description: 結果會衡量目標的進度。 若未將結果、活動或校準的目標與目標建立關聯，您就無法啟動目標，也無法記錄其進度。
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 3%

---

# 在Adobe Workfront目標中新增結果

<!--Audited for P&P only: 10/2025-->

結果會衡量目標的進度。 若未將結果、活動或校準的目標與目標建立關聯，您就無法啟動目標，也無法記錄其進度。

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
<p>要求或更高版本</p></td>
 </tr>
  <tr>
 <td role="rowheader">存取層級設定</td>
 <td> <p>編輯目標的存取權</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  </div> </td>
 </tr>
<tr>
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
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
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
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 先決條件

開始之前，您必須具備下列條件：

* 包含主功能表中目標區域的版面配置範本。
* 現有目標。

  如需建立目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。

>[!IMPORTANT]
>一個目標不能有超過1000個活動、結果、專案或校準的目標。

## 將結果新增到目標中

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

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

1. 按一下主功能表![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。

1. 從&#x200B;**目標清單**，按一下目標的名稱以開啟目標頁面。
1. 按一下左側面板中的&#x200B;**進度指示器**。
1. 展開&#x200B;**新進度指示器**&#x200B;下拉式功能表，然後按一下&#x200B;**建立結果**。

   「新建結果」方塊開啟。

   ![新結果方塊](assets/new-result-box-unshimmed.png)

1. 在&#x200B;**結果名稱**&#x200B;欄位中輸入結果的名稱。 這是必填欄位。
1. （選擇性）如果要將結果指派給其他使用者，請從&#x200B;**結果擁有者**&#x200B;欄位中移除您的名稱。 依預設，您是您建立之活動的擁有者。

   >[!NOTE]
   >
   >您無法將團隊、群組或公司指派為結果擁有者。

1. 在&#x200B;**中，您要如何測量結果？**&#x200B;區域，請指定下列資訊：
   * **值型別**：這表示您要如何測量結果的進度。 您可以使用百分比值或貨幣金額以數值方式測量進度。

     從下表列出的選項中選取值型別：

     | 值類型 | 說明 |
     |---------------------------------------------------------|------------------|
     | 數字 | 數值 |
     | % | 百分比值 |
     | CN¥、DKK、KR、Mex$、R、$、 zl、 £ 、 € 、 ₹、 ฿、 MYR、 ₪、$ | 貨幣值 |

   * **初始值**：結果在記錄任何進度之前的開頭值。
   * **目標值**：結果被視為完成時所要達到的值。
1. 按一下&#x200B;**建立結果**。

   結果會顯示在目標頁面的「進度指示器」區段的「結果」群組下。

   啟動目標後，當您更新結果的進度時，目標的進度會自動更新。 如需啟用目標的相關資訊，請參閱[在Adobe Workfront目標中啟用目標](../goal-management/activate-goals.md)。
