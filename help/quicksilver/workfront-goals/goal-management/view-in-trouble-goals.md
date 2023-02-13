---
product-previous: workfront-goals
navigation-topic: goal-management
title: 檢閱Adobe Workfront目標中的問題目標
description: 《有麻煩的進展》有不可能實現的危險，以Adobe Workfront目標中的紅色進展條為代表。 您應經常審視您的目標，並了解進度為何落後。
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# 檢閱Adobe Workfront目標中的問題目標

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

《有麻煩進展的目標》有不能實現的危險，Adobe Workfront目標中的紅色進展條是代表。 您應經常審視您的目標，並了解進度為何落後。 如需目標進度的相關資訊，請參閱 [Adobe Workfront目標中的目標進度和條件概覽](../../workfront-goals/goal-management/calculate-goal-progress.md).

## 存取需求

<!--drafted for P&P release: replace the existing requirements with this:

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
   <td> <p>編輯目標或更高版本的存取權</p> <p><b>附註</b><p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱：</p> 
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

## Recommendations：《麻煩中》進展難

在目標達到「遇到麻煩」的進度之前，您可以經常監控這些進度，並在達到「面臨風險」的進度時調整其進度。 面臨風險的目標有陷入麻煩的危險。 如需目標進度的詳細資訊，請參閱 [Adobe Workfront目標中的目標進度和條件概覽](../../workfront-goals/goal-management/calculate-goal-progress.md)

在您的目標達到「麻煩中」進度之前，我們建議：

* 審查經常分配給您的具有「風險」條件的目標，以及分配給您的團隊、組或組織的組織目標，這些目標可能會受目標進度的影響。 風險目標有可能變成麻煩目標。 風險目標以黃色進度列標示。 使用「目標清單」可檢視屬於您、您的團隊、群組或組織的目標。


## 查看目標清單中的故障目標

您可以檢閱Workfront目標任何區段中的目標。 如需「Workfront目標」章節的相關資訊，請參閱 [Adobe Workfront目標章節概覽](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

本文說明如何檢閱目標清單中的目標。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) > **目標** 在右上角。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   這會開啟「Workfront目標」區域，並依預設顯示「目標清單」區段。

1. （建議）調整「目標清單」區域的下列篩選條件，以審核風險目標：

   * 按一下 **公司**，然後 **我的團隊**，然後 **我的群組**，然後 **個人** 目標，以便檢視屬於您的組織、您的團隊、群組，然後是您自己的目標。

      >[!TIP]
      >
      >在Adobe Workfront目標中，公司篩選器會顯示您的組織被選取為擁有者的目標。
      >
      >
      >您無法使用此欄位來搜尋公司。 依預設，僅會選取擁有Workfront執行個體的組織。

   * 針對您在上方選取的每個組織單位，按一下 **新增篩選** > **進度** > **麻煩** >**。**
   * （選用）選取您要檢視目標的時段。

      目標清單中每個目標的進度列指標會以紅色顯示。

      如需使用右側面板中所有其他條件來篩選目標的詳細資訊，請參閱 [篩選Adobe Workfront目標中的資訊](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 將滑鼠指標暫留在進度列指標上，可查看實際進度百分比，以及當天的預期值。

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. （選用）使用篩選器來尋找屬於特定擁有者的目標。

   目標清單中會顯示所選使用者的故障中目標。

1. 按一下目標名稱以開啟目標頁面，然後按一下 **進度指標** 中。 查看哪些進度指標導致目標落後，並更新該指標的進度，位於 **實際進度** 進度指標清單的列。

   如需更新結果和活動的相關資訊，請參閱 [更新Adobe Workfront目標中的目標進度](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >您只能更新進度指標清單中的結果和活動。 您必須通過訪問目標來更新子項目標的進度指標，並且必須更新有關連接項目的任務以更新項目的進度。


