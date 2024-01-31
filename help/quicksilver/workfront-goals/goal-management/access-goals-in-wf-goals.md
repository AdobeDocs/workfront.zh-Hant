---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中存取和開啟目標
description: 本文說明如何在Adobe Workfront中尋找和管理目標。
author: Alina
feature: Workfront Goals
exl-id: a729f334-6ca4-4cf5-a3ef-01a7effb7153
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 在Adobe Workfront目標中存取和開啟目標

本文說明如何在Adobe Workfront中尋找和管理策略目標。


## 存取需求

<!--drafted for P&P: replace the requirements table and the asterisk below it with the following: 


You must have the following to perform the activities described in this article:

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
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
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
  <tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> 
    <div> 
     <p>All users, including Workfront administrators,  must be assigned to a layout template that includes the Goals area in the Main Menu. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
-->

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td> <p>您必須為Adobe Workfront目標購買額外的授權，才能存取本文所述的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯目標的存取權</p> <p><b>附註</b><p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span> </p> </li> 
     </ul> </p> </td> 
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
   <td> 
    <div> 
     <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p> 
    </div> </td> 
  </tr>

</tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 存取Workfront目標

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 按一下「 」 **目標**.

   <!-- drafted for Shell release: Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   目標清單隨即顯示。


   >[!IMPORTANT]
   >
   >   當您擁有Workfront目標的正確存取權時，預設情況下，您可以檢視自己或其他任何人在目標清單中建立的目標。

   <!--   
   (NOTE: This might change when sharing is in place; right now, with sharing in place, they can VIEW all goals in the system but they cannot EDIT the ones others created!)
   -->

1. （選用）按一下目標的名稱以開啟或編輯目標。

   或

   按一下 **新目標** 以新增目標。

   如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).

## 開啟和管理個別目標

您必須存取個別目標，才能在管理目標時執行下列動作：

* 編輯它
* 新增結果或活動到其中
* 編輯與其關聯的結果和活動
* 啟用它
* 停用它
* 刪除它
* 使其與另一個目標一致
* 將結果或活動轉換為其他目標
* 更新它
<!--
Accessing goals differs depending on what environment you use.

To access an individual goal in the Production environment:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Goals** .

     (!--drafted for Shell release: Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List displays by default. 

1. Click the name of a goal in the list 

   Or

   Click one of the options below in the left panel, then click the name of a goal to access it:

   * Goal Alignment
   * Check-in 
   * Pulse 

   >[!NOTE]
   >
   >Depending on what action you want to perform on the individual goal, you might choose to select different sections every time. For information about the differences between the Workfront Goals sections, see [Overview of the Adobe Workfront Goals sections](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

   The Goal Details panel displays on the right. You can update the goal, its results, and activities in the Goal Details panel when you have access to manage it. For information about updating goals using the Goal Details panel, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
-->

若要存取個別目標：

1. 按一下 **主要功能表** Workfront圖示並按一下「 」，接著再按一下「 」。 **目標** .
預設會顯示「目標清單」。
   ![](assets/goal-list-unshimmed.png)
1. 按一下清單中目標的名稱。
目標的頁面隨即顯示。
   ![](assets/goal-page-unshimmed.png)
1. 按一下 **更多** 功能表 ![](assets/more-icon.png) 位於目標名稱的右側，以進一步編輯或共用目標。
1. 按一下 **目標詳細資料** 編輯目標的相關資訊。 如需詳細資訊，請參閱 [更新「Adobe Workfront目標」中「目標詳細資料」區段中的目標](../goal-management/update-goals-in-goal-details-panel.md).


