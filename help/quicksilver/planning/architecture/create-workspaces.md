---
title: 建立工作區
description: 工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。 記錄型別會依工作區中的區段組織。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LtHxTws4o0FI964-qOtFE-sbKaLGRQroBQvMD5fOUvY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 1311
ht-degree: 1%

---

# 建立工作區

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。

工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。

如需工作區的一般資訊，請參閱[工作區概述](/help/quicksilver/planning/architecture/workspaces-overview.md)。

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

  如需詳細資訊，請參閱本文中的[從頭開始或從範本建立工作區](#create-a-workspace-from-scratch-or-from-a-template)一節。
* 使用AI支援的Planning Designer建立一個工作區。 此功能目前僅適用於Beta計畫中的有限數量客戶。

  如需詳細資訊，請參閱[開始使用Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md)。

* 使用最佳實務多工作區範本套件組合建立多個工作區

  如需詳細資訊，請參閱本文章的[使用最佳實務多工作區範本組合](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle)建立多個工作區

  >[!TIP]
  >
  >只有在使用最佳實務範本組合時，才能一次建立多個工作區。

### 從頭開始或從範本建立工作區

{{step1-to-planning}}

1. 按一下&#x200B;**建立工作區**

   「建立工作區」方塊隨即顯示。 您可以從頭開始建立工作區，或使用其中一個可用的範本建立工作區。

1. （選擇性和條件式）在下列任何預先定義的工作區範本中按一下&#x200B;**預覽**：

   * Operations Initiative Studio
   * Communications Planning Studio
   * 基本：行銷管理
   * 進階：行銷管理
   * 企業：行銷管理
   * 銷售管理
   * 產品管理

   範本預覽方塊開啟。

   這會指出哪些記錄型別、區段以及與每個範本相關聯的欄位數。

   ![預覽工作區範本](assets/previewing-a-workspace-template.png)

   如需Workfront Planning工作區範本的相關資訊，請參閱[工作區範本清單](/help/quicksilver/planning/architecture/workspace-templates.md)。

1. 在範本預覽方塊中，按一下&#x200B;**使用範本**&#x200B;以從選取的範本開始建立工作區

   或

   按一下[上一步]****，然後按一下[新工作區]****&#x200B;從頭開始建立工作區。

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

   如需有關編輯工作區的詳細資訊，包括編輯工作區區段，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。

1. （選擇性）按一下&#x200B;**新增記錄型別**，將記錄型別新增至任何區段中的工作區。

   如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   如需在工作區中編輯和刪除記錄型別的詳細資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。

1. （可選）按一下新工作區左側的返回箭頭，以開啟Planning首頁面。 在我所在的&#x200B;**工作區**&#x200B;索引標籤中為新工作區建立了新工作區卡片。

   建立工作區的使用者名稱會以擁有者的身分儲存在工作區卡片上。

   >[!TIP]
   >
   >僅Workfront使用者建立且尚未新增至Adobe Admin Console的工作區，會顯示為&#x200B;**系統**&#x200B;所建立。
   >

### 使用最佳實務多工作區範本套件組合建立多個工作區

>[!IMPORTANT]
>
>只有在符合下列先決條件時，才能使用最佳實務範本套件組合一次建立多個工作區：
>
>* 貴組織已購買Workfront或工作流程計畫Prime或Ultimate套件
>* 您是系統管理員

您只需按一下即可使用多工作區範本組合來建立6個工作區。

套件組合中包含的範本包含工作區、記錄型別、記錄、檢視和欄位，可協助您開始實施Planning。 如需詳細資訊，請參閱[工作區範本清單](/help/quicksilver/planning/architecture/workspace-templates.md)。

>[!IMPORTANT]
>
>束中包含的工作區和記錄的名稱只是範例，並非您自己環境的反映。
>
>根據我們的建議，記錄型別和欄位的名稱可用於任何組織，作為任何產業中實施的標準。
>

{{step1-to-planning}}

1. 執行下列其中一項：

   * 按一下「**建立工作區**」，然後依照下列步驟進行：

      1. 「建立工作區」方塊隨即顯示。 您可以從頭開始建立工作區，或使用其中一個可用的範本建立工作區。

      1. 按一下&#x200B;**從這裡開始（建議）**&#x200B;區域中的&#x200B;**檢閱工作區設定**。
      1. （選擇性）在下列任何預先定義的工作區範本中按一下&#x200B;**預覽**，以開啟每個範本的「預覽」方塊：

         * 1.全域分類與分類法

           「全域分類與分類」範本包含我們建議您在您的環境中建立的所有記錄型別和欄位，以便成功實作Workfront Planning。

           您稍後可以在您建立的其他工作區中連結或匯入此範本中的記錄型別。
         * 2.Fréscopa全球行銷
         * 3.Fréscopa社交行銷
         * 4.弗雷斯科帕媒體與公關
         * 5.Fréscopa全球活動
         * 6.Fréscopa執行公司領導力

      1. 開啟每個工作區範本的&#x200B;**預覽**&#x200B;方塊後，按一下&#x200B;**上一步**&#x200B;以返回&#x200B;**建立工作區**&#x200B;方塊，或按一下&#x200B;**使用範本**&#x200B;以使用套件組合中包含的範本並建立工作區。

   <div class="preview">

   * 按一下&#x200B;**範例工作區**&#x200B;索引標籤，然後依照下列步驟進行：

      1. 按一下標籤上的其中一個工作區範本，即可檢閱每個範本中的記錄型別和欄位。 **範例工作區**&#x200B;索引標籤中的範本是唯讀的。
      1. 按一下範本右上角的&#x200B;**從範本建立**。
      1. （選擇性）按一下任何範本上的&#x200B;**預覽**&#x200B;以檢視記錄型別及其欄位。

         >[!TIP]
         >
         >按一下範本中的記錄型別卡片，即可在右側面板中顯示記錄型別的欄位。
      1. 按一下&#x200B;**使用範本**。

   </div>

   這6個工作區已建立並顯示在我所在的&#x200B;**工作區**&#x200B;以及系統管理員的&#x200B;**所有工作區**&#x200B;標籤中。 系統管理員建立所有標準授權使用者並與其共用新工作區後，這些使用者都會在其「工作區」區域中看見工作區。

1. 開始編輯您建立的工作區，並新增與組織相關的記錄型別、記錄、檢視和欄位。

   如需有關實作Workfront的最佳實務的詳細資訊，請參閱[Adobe Workfront規劃最佳實務：文章索引](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md)區段中的文章。

   如需有關編輯工作區的資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。



