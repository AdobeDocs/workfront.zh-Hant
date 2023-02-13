---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 通過將結果和活動轉換為目標來協調目標
description: 您可以手動協調兩個目標，或將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。 如需手動協調兩個目標的詳細資訊，請參閱在Adobe Workfront目標中連結以協調目標。
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# 通過將結果和活動轉換為目標來協調目標

您可以手動協調兩個目標，或將現有目標的結果和活動轉換為另一個目標。 轉換的結果或活動會成為原始目標的子目標。
如需手動協調兩個目標的相關資訊，請參閱 [在Adobe Workfront目標中將目標連結起來，以協調目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## 存取需求


<!--drafted for P&P release: 

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
   <td> <p>編輯目標或更高版本的存取權</p> <p><b>附註</b> 
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
* 具有現有結果和活動的現有目標。

   如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>一個目標最多可以有1 000個進度指標。

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## 將結果和活動轉換為目標時的考量事項

有時，結果或活動的範圍可能比預期更廣，而且更合理的是，它們將成為目標。 您可以將現有目標的結果和活動轉換為新目標。 這是一種自下而上的方法來協調目標。

將結果和活動轉換為目標時，請考慮下列事項：

* 轉換的結果或活動會成為原始目標的子目標，且兩個目標會對齊。
* 如果原始目標上沒有其他結果或活動，則新建立的目標將成為原始目標的單一進度指標。 您必須將結果和活動新增至子目標，才能追蹤進度。
* 將結果或活動轉換為目標是不可逆的。 轉換後，新的子目標將永遠無法再成為父目標的結果或活動。

## 將結果或活動轉換為目標

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. 前往具有結果或您要轉換為目標的活動的目標。
1. 在目標頁面中，按一下 **進度指標** 中。
1. 在進度指標清單中選取結果或活動，然後按一下 **轉換為目標** 圖示 ![](assets/convert-to-goal-icon-unshimmed.png) 在進度指標清單的頂部。 「轉換為目標」(Convert to goal)框開啟。

   ![](assets/convert-to-goal-box-unshimmed.png)
1. 更新下列資訊：
   * **目標名稱**:依預設，新目標的名稱與原始結果或活動相同。
   * **時段**:依預設，新目標的期間為目前的季度。 您可以選取 **啟用自訂日期** 設定以定義新目標的自訂時段。
   * **目標所有者**:依預設，新目標擁有者是原始結果或活動的擁有者。
   * **說明**:新增新目標的詳細資訊。
1. 按一下 **儲存**

   結果或活動現在會轉換為原始目標的子目標。 它被列為原始目標的進度指標清單中的目標。



