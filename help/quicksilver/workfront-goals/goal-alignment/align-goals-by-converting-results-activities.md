---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 透過將結果和活動轉換為目標來校準目標
description: 您可以手動對齊兩個目標，也可以將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。 如需有關手動對齊兩個目標的資訊，請參閱在Adobe Workfront目標中透過連線來對齊目標。
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 15%

---

# 透過將結果和活動轉換為目標來校準目標

您可以手動對齊兩個目標，也可以將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。
如需有關手動對齊兩個目標的資訊，請參閱[在Adobe Workfront目標中連線來對齊目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)。

## 存取需求


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
 <p>目前授權：要求或以上</p> <p>如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
 <p> 新產品需求，下列其中一項： </p>
<ul>
<li>Select或Prime Adobe Workfront計畫以及額外的Adobe Workfront目標授權。</li>
<li>Ultimate Workfront計畫，預設包含Workfront目標。 </li></ul>
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

開始之前，您必須具備下列條件：

* 具有現有結果和活動的現有目標。

  如需建立目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。

>[!IMPORTANT]
>
>一個目標最多可以有1000個進度指示器。

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## 將結果和活動轉換為目標時的注意事項

有時候，結果或活動的範圍可能比預期的要大，並且更合理的做法是它們會成為目標。 您可以將現有目標的結果和活動轉換為新目標。 這是自下而上的方法來調整目標。

將結果和活動轉換為目標時，請考量下列事項：

* 轉換後的結果或活動成為原始目標的子目標，並且兩個目標保持一致。
* 如果原始目標沒有其他結果或活動，則新建立的目標將成為原始目標的單一進度指標。您必須將結果和活動新增到子目標中才能追蹤其進度。
* 將結果或活動轉換成目標是不可逆的。一經轉換，新的子目標將永遠不會再次成為父系目標的結果或活動。

## 將結果或活動轉換為目標

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. 移至具有結果或您要轉換為目標的活動的目標。
1. 從目標的頁面，按一下左側面板中的&#x200B;**進度指示器**。
1. 在進度指標清單中選取結果或活動，然後按一下進度指標清單頂端的&#x200B;**轉換為目標**&#x200B;圖示![轉換為目標](assets/convert-to-goal-icon-unshimmed.png)。 「轉換為目標」方塊開啟。

   ![轉換為目標方塊](assets/convert-to-goal-box-unshimmed.png)
1. 更新下列資訊：
   * **目標名稱**：依預設，新目標的名稱與原始結果或活動相同。
   * **期間**：依預設，新目標的期間為目前季度。 您可以選取&#x200B;**啟用自訂日期**&#x200B;設定，以定義新目標的自訂時段。
   * **目標擁有者**：依預設，新的目標擁有者是原始結果或活動的擁有者。
   * **描述**：新增新目標的詳細資訊。
1. 按一下&#x200B;**儲存**

   結果或活動現在轉換為原始目標的子目標。 它會在原始目標的進度指標清單中列為目標。



