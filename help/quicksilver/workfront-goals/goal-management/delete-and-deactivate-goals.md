---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: 刪除和停用Adobe Workfront目標中的目標
description: 當您開始處理目標，且該目標在您的組織中變得無關時，建議您停用該目標，而非將其刪除。 停用目標可保留其歷史資訊，並讓您有機會稍後重新啟用目標。 不過，有時刪除目標可能有意義，可讓您的目標清單正確無誤。
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 刪除和停用Adobe Workfront目標中的目標

當您開始處理目標，且該目標在您的組織中變得無關時，建議您停用該目標，而非將其刪除。 停用目標可保留其歷史資訊，並讓您有機會稍後重新啟用目標。 不過，有時刪除目標可能有意義，可讓您的目標清單正確無誤。

## 存取需求

<!--drafted for P&P release: 

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

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須具備下列條件，才能開始：

* 一種佈局模板，在主菜單中包括目標區域。

## 停用目標

您可以停用不再相關的目標，且您日後可能想要重新啟用。

* [停用目標時的考量事項](#considerations-when-deactivating-goals)
* [停用目標](#deactivate-goals)

### 停用目標時的考量事項

停用目標時請記住以下事項：

* 您只能停用處於「作用中」狀態的目標。 如需啟動目標的相關資訊，請參閱 [啟用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/activate-goals.md).

   >[!TIP]
   >
   >您無法停用草稿狀態中的目標。

* Workfront停止計算已停用目標的進度。
* Workfront目標的「圖表」區段中不再顯示非作用中目標，也不會將其納入考量。 如需Workfront目標圖表的相關資訊，請參閱 [檢閱圖表以了解Adobe Workfront目標中的目標進度趨勢](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* 您無法再對停用的目標進行更新。
* 您可以編輯目標及其對齊方式的相關資訊。
* 您可以重新啟用先前停用的目標。

### 停用目標

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 按一下右上角的 **目標**.

   目標清單隨即顯示。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. （選用）修改您的篩選條件，僅顯示作用中的目標。

   如需篩選Workfront目標中資訊的詳細資訊，請參閱 [篩選Adobe Workfront目標中的資訊](../goal-management/filter-information-wf-goals.md).

1. 按一下作用中的目標。

   目標頁面隨即開啟。

   ![](assets/goal-page-unshimmed.png)

1. 按一下 **更多** 功能表 ![](assets/more-icon.png) 在目標名稱的右側，然後按一下 **停用**.

1. 目標已停用，其狀態會變成非使用中。

## 刪除目標

您可以刪除不再相關或可能永遠無關的目標。

* [刪除目標時的考量事項](#considerations-when-deleting-goals)
* [刪除目標](#delete-goals)

### 刪除目標時的考量事項 {#considerations-when-deleting-goals}

* 您可以刪除任何狀態的目標，包括已結束的目標。
* 您無法恢復已刪除的目標。
* 也會刪除附加至目標的結果和手動進度欄活動。
* 不會刪除與目標相關聯的專案，但會移除其與目標的關聯。

### 刪除目標

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon.png) 按一下右上角的 **目標**.

   目標清單隨即顯示。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 按一下目標的名稱。 這會開啟目標頁面。
1. 按一下 **更多** 功能表 ![](assets/more-icon.png) 在目標名稱的右側，然後按一下 **刪除目標**，然後 **刪除**.

   目標及其活動和結果也會被刪除，無法復原。 不會刪除與目標或子目標相關聯的項目。


