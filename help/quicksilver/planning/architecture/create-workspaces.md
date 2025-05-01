---
title: 建立工作區
description: 工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。 記錄型別會依工作區中的區段組織。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 建立工作區

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中，工作區是團隊規劃工作的集中位置。

工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區。

如需工作區的一般資訊，請參閱[工作區概述](/help/quicksilver/planning/architecture/workspaces-overview.md)。

## 存取需求

+++ 展開以檢視存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 產品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>您會收到您所建立之工作區的「管理」許可權。 </p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>在生產環境中，所有使用者（包括系統管理員）都必須指派給包含Planning的版面配置範本。</p>
<p><span class="preview">在預覽環境中，標準使用者和系統管理員預設啟用Planning。</span></p></td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立工作區

您可以建立工作區並在其中新增記錄型別，以在Workfront Planning中組織您的物件。 如需有關編輯工作區的詳細資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。

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

   系統會指出哪些作業記錄型別、分類法以及與每個範本相關聯的欄位數。

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


