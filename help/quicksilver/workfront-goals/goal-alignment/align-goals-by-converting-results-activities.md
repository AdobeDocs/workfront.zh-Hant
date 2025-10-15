---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 透過將結果和活動轉換為目標來校準目標
description: 您可以手動對齊兩個目標，也可以將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。 如需有關手動對齊兩個目標的資訊，請參閱在Adobe Workfront目標中透過連線來對齊目標。
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 17%

---

# 透過將結果和活動轉換為目標來校準目標

<!--Audited P&P only: 4/2025-->

您可以手動對齊兩個目標，也可以將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。
如需有關手動對齊兩個目標的資訊，請參閱[在Adobe Workfront目標中連線來對齊目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)。

## 存取需求

>[!NOTE]
>
>如果貴公司過去曾購買此套件，他們可能會選擇繼續使用Adobe Workfront目標。 如需詳細資訊，請洽詢客戶代表。
>
>Adobe Workfront目標不再提供購買。

+++展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>Adobe Workfront套件</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront授權</p> </td> 
   <td> <p>投稿人或以上</p> 
     <p>要求者或以上</p> </td> 
  </tr>

<td><p>存取層級設定</p> </td> 
   <td> <p>編輯目標的存取權</p> </td> 
  </tr> 
  <tr> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p>管理目標的許可權</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者（包括系統管理員）指派一個版面配置範本，該範本包括主功能表中的「目標」區域。 </p>  
</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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



