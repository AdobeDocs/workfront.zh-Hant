---
product-previous: workfront-goals
navigation-topic: goal-management
title: 列印Adobe Workfront目標中的目標清單
description: 您可以從Adobe Workfront目標的目標清單區段列印目標清單。 如果瀏覽器的「打印目標」設定為「另存為PDF」，則打印會將檔案發送到打印機或生成.pdf檔案。
author: Alina
feature: Workfront Goals
exl-id: 66488d2f-ed35-4571-93e3-e0e025da7b33
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# 列印Adobe Workfront目標中的目標清單

>[!IMPORTANT]
>
>自23.1版開始，本文所述的功能已從Workfront中移除。
>
>2023年初，23.1版發行後不久，也將移除本文。 此時，建議您據以更新任何書籤。

您可以從Adobe Workfront目標的目標清單區段列印目標清單。 如果瀏覽器的「打印目標」設定為「另存為PDF」，則打印會將檔案發送到打印機或生成.pdf檔案。

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

您必須具備下列存取權，才能執行本文所述的動作：

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
   <td role="rowheader">存取層級*</td> 
   <td> <p>檢視或更高程度地存取目標</p> <p><b>附註</b><p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> 
    <div> 
     <p>檢視目標的或更高權限</p> 
     <p>如需共用目標的相關資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須具備下列條件，才能開始：

* 一種佈局模板，在主菜單中包括目標區域。

## 打印目標清單

>[!TIP]
>
>* 列印目標清單時，產生的檔案只包含螢幕上顯示的資訊。 篩選目標清單所消除的項目不會顯示在.pdf檔案中。
>* 當您在列印清單之前未展開清單中的目標時，.pdf檔案只會顯示沒有其結果和活動的目標。
>


1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) > **目標** 在右上角。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   這會開啟Workfront目標區域。

   預設會顯示「目標清單」。

1. （選用）將篩選器套用至目標清單，以檢視與您相關的目標。

   如需篩選目標清單中資訊的相關資訊，請參閱 [篩選Adobe Workfront目標中的資訊](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 按一下 **列印**. 打印框隨即顯示。
1. （條件性）根據您使用的瀏覽器和電腦上已安裝的其他應用程式，您可以從下列目的地進行選取：

   * 打印到打印機
   * 打印到PDF
   * 將目標清單儲存到本地或聯機驅動器(例如，Google驅動器)
   * 將目標清單傳送至其他應用程式（例如「一個附註」）

1. （可選）調整打印選項。
1. 按一下 **列印**.

   目標清單會傳送至您選取的目的地。
