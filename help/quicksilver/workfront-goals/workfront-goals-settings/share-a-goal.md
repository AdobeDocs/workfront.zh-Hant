---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: 在Workfront目標中共用目標
description: 當您共用目標時，您會將目標的「管理」權限授予未建立該目標的人。
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# 在Adobe Workfront目標中共用目標

當您共用目標時，您會將目標的「管理」權限授予未建立該目標的人。

## 存取需求

<!--drafted - replace the table below with this one when P&P releases: 

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
     <p>如需共用目標的相關資訊，請參閱 <a href="#" class="MCXref xref selected">在Workfront目標中共用目標</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須具備下列條件：

* 一種佈局模板，在主菜單中包括目標區域。

## 共用目標的考量事項

* 使用者可擁有目標的下列權限：

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>目標權限</b></p></td> 
      <td>
      <p><b>說明</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>檢視</p></td> 
      <td>
      <p>使用者有檢視目標的權限，但無法編輯目標的資訊、無法新增或編輯結果、活動、更新狀態或刪除目標的資訊。</p>      
      <p>依預設，所有具有目標存取權的使用者都可以檢視系統中的所有目標。 如果使用者在其存取層級中擁有「編輯」目標存取權，則可複製目標。</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>管理</p></td> 
      <td> <p>使用者可以編輯目標的所有資訊，包括結果或活動的資訊，包括刪除這些資訊。</p> 
      <p>只有明確指定目標的管理權限的目標建立者或使用者才能管理目標。</p> 
      只有對目標具有管理權限的使用者才能與其他人共用目標，以授予目標的管理權限。 </p> </td> 
   </tr> 
   </tbody> 
   </table>

* 您可以與其他人共用下列類型的目標：

   * 您建立的目標
   * 您被授予「管理」權限的其他人所建立的目標。

* 如果您有目標的「管理」權限，則可以為目標建立者變更目標的權限。 依預設，他們在建立目標時具有「管理」權限，但您可以將其權限變更為「檢視」。

## 共用目標

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) > **目標** 在右上角。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   目標清單隨即顯示。

1. 按一下清單中目標的名稱。 目標頁面隨即開啟。

1. 按一下 **更多圖示** 在目標名稱旁，按一下 **共用**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   「目標存取」方塊隨即顯示。

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. 執行下列任一項作業：

   * 選取 **管理全系統** 設定，將「管理」權限授予系統中在其存取層級具有「編輯」目標存取權的每個人。 對於所有新目標，預設會取消選取此選項。
   * 開始鍵入要在 **授予管理存取權** 框。 選取名稱出現在清單中時。

      >[!TIP]
      >
      >您只能與其他使用者共用目標。 您無法與群組、團隊或您的公司共用目標。

1. 按一下 **共用**.

   目標會與您指定的使用者共用。 「目標詳細資訊」面板的「存取管理」欄位中會顯示「系統範圍」標籤或具有目標「管理」權限的使用者名稱。

## 目標權限選項

下表列出您在共用目標時可授予的權限。 如需使用者根據其授權所取得存取權限的詳細資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>動作</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>檢視</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>檢視目標</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檢視結果或活動</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>複製目標* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>將結果或活動轉換為其他目標*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>檢視新增為活動的專案** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>編輯目標</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯結果或活動</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>為目標新增結果或活動</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>將專案作為活動與目標建立關聯**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>刪除目標</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>刪除結果或活動</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>斷開項目與目標的連接</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*您必須在存取層級中擁有「編輯目標」存取權，才能將結果和活動轉換為目標。

**您必須擁有已新增或要新增至目標以檢視專案的「檢視專案」和「檢視」權限。

如需專案存取層級的相關資訊，請參閱 [授予專案的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

如需專案權限的相關資訊，請參閱 [在Adobe Workfront中共用專案](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
