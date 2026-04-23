---
title: 建立工作區
description: 工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。 記錄型別會依工作區中的區段組織。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---


# 建立工作區

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。

工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。

For general information about workspaces, see [Workspaces overview](/help/quicksilver/planning/architecture/workspaces-overview.md).

## 存取權要求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>任何Workfront或Workflow套件</p> 
<p>任何Workfront Planning套件</p>
<p>Workfront Planning Prime或更新版本的套件，一次建立多個工作區</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   <p>系統管理員使用最佳實務範本套件一次建立多個工作區</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## 建立工作區

您可以建立工作區並在其中新增記錄型別，以在Workfront Planning中組織您的物件。

如需有關編輯工作區的詳細資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。

您可以使用下列方式建立工作區：

* 從頭開始或從範本建立一個工作區

  For information, see the section [Create a workspace from scratch or from a template](#create-a-workspace-from-scratch-or-from-a-template) in this article.
* Create one workspace using the AI-powered Planning Designer. This feature is currently available only to a limited number of customers in a Beta program.

  如需詳細資訊，請參閱[開始使用Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md)。

* Create multiple workspaces using a best-practice multi-workspace template bundle

  For information, see the section [Create multiple workspaces using a best-practice multi-workspace template bundle](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) in this article

  >[!TIP]
  >
  >只有在使用最佳實務範本組合時，才能一次建立多個工作區。

### 從頭開始或從範本建立工作區

{{step1-to-planning}}

1. 按一下&#x200B;**建立工作區**

   「建立工作區」方塊隨即顯示。 您可以從頭開始建立工作區，或使用其中一個可用的範本建立工作區。

1. （選擇性和條件式）在下列任何預先定義的工作區範本中按一下&#x200B;**預覽**：

   * 基本：行銷管理
   * 進階：行銷管理
   * 企業：行銷管理
   * 銷售管理
   * 產品管理

   範本預覽方塊開啟。

   There is an indication of what operational record types, taxonomies and how many fields are associated with each template.

   ![預覽工作區範本](assets/previewing-a-workspace-template.png)

   如需Workfront Planning工作區範本的相關資訊，請參閱[工作區範本清單](/help/quicksilver/planning/architecture/workspace-templates.md)。

1. 在範本預覽方塊中，按一下&#x200B;**使用範本**&#x200B;以從選取的範本開始建立工作區

   或

   Click **Back**, then click **New workspace** to create a workspace from scratch.

   會建立下列其中一種工作區型別：

   * 名為&#x200B;**無標題Workspace**&#x200B;的空白工作區，當您從頭開始建立工作區時，可以在此處開始手動新增記錄型別。
   * 以您選取的範本命名並填入範例記錄型別的工作區。 您可以進一步自訂記錄型別和工作區。

   若為Workfront管理員，新工作區會顯示在我所在的&#x200B;**工作區中**&#x200B;索引標籤。

   對於可以建立工作區的所有其他使用者，新工作區會顯示在&#x200B;**工作區**&#x200B;區域中。

1. 在新工作區標題的工作區名稱內按一下以重新命名，然後按Enter鍵。

1. （選擇性和條件式）如果您是從範本建立工作區，請在&#x200B;**作業記錄型別**&#x200B;或&#x200B;**分類**&#x200B;區段的名稱內按一下

   或

   將游標暫留在區段名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**重新命名**&#x200B;以重新命名區段。

   >[!TIP]
   >
   >您可以從任何工作區重新命名任何區段，即使您沒有建立該區段亦然。

   For more information about editing workspaces, including editing workspace sections, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. （選擇性）按一下&#x200B;**新增記錄型別**，將記錄型別新增至任何區段中的工作區。

   如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   如需在工作區中編輯和刪除記錄型別的詳細資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。

1. （可選）按一下新工作區左側的返回箭頭，以開啟Planning首頁面。 在我所在的&#x200B;**工作區**&#x200B;索引標籤中為新工作區建立了新工作區卡片。

   The name of the user who created the workspace is saved on the workspace card as the Owner.

   >[!TIP]
   >
   >Workspaces created by Workfront-only users who have not been added to the Adobe Admin Console display as created by the **System**.
   >

### Create multiple workspaces using a best-practice multi-workspace template bundle

>[!IMPORTANT]
>
>Creating multiple workspaces at a time using the best-practice template bundle is available only when the following prerequisites are met:
>
>* Your organization purchased a Workfront Planning Prime or Ultimate package.
>* 您是系統管理員

您只需按一下即可使用多工作區範本套件來建立6個工作區。

套件組合中包含的範本包含工作區、記錄型別、記錄、檢視和欄位，可協助您開始實施Planning。

>[!IMPORTANT]
>
>束中包含的工作區和記錄的名稱只是範例，並非您自己環境的反映。
>
>根據我們的建議，記錄型別和欄位的名稱可用於任何組織，作為任何產業中實施的標準。
>

{{step1-to-planning}}

1. 按一下&#x200B;**建立工作區**

   「建立工作區」方塊隨即顯示。 您可以從頭開始建立工作區，或使用其中一個可用的範本建立工作區。

1. 按一下&#x200B;**從這裡開始（建議）**&#x200B;區域中的&#x200B;**檢閱工作區設定**。
1. （選擇性）在下列任何預先定義的工作區範本中按一下&#x200B;**預覽**，以開啟每個範本的「預覽」方塊：

   * 1.全域分類與分類法

     「全域分類與分類」範本包含我們建議您在您的環境中建立的所有記錄型別和欄位，以便成功實作Workfront Planning。

     You can later link or import the record types in this template in other workspaces you create.
   * 2.Fréscopa全球行銷
   * 3.Fréscopa社交行銷
   * 4.弗雷斯科帕媒體與公關
   * 5.Fréscopa全球活動
   * 6.Fréscopa Executive Company Leadership

1. After opening the **Preview** box for each workspace template, click Back to go back to the **Create workspace** box, or click Use templates to use the templates including in the bundle and create workspaces.

   The workspaces are created and display in the **Workspaces I&#39;m** on and **All Workspaces** tabs for System administrators. All Standard-license users will see the workspaces in their Workspaces area after a System Administrator creates them and shares the new workspaces with them.

1. Start editing the workspaces you created and adding record types, records, views, and fields that are pertinent to your organization.

   For more information about best practices to implement Workfront, see the articles in the [Adobe Workfront Planning best practices: article index](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) section.

   如需有關編輯工作區的資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。



