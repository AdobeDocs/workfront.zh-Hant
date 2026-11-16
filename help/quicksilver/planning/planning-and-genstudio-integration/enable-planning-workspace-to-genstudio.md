---
title: 在GenStudio for Performance Marketing中啟用Workfront規劃Workspace
description: 您可將Adobe Workfront Planning工作區設定為GenStudio for Performance Marketing中同時存取這兩個應用程式時的可用工作區。
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 3%
---
# 啟用Workfront規劃工作區至GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

當貴公司同時購買Adobe GenStudio for Performance Marketing並且您是Adobe Workfront Planning客戶時，Workfront Planning中也可使用GenStudio工作區。

如果您在Workfront Planning中已有Planning工作區，您可以為GenStudio for Performance Marketing啟用它，而不是在GenStudio中重新建立相同的資料。

啟用工作區可將其連結至Adobe Could Storage專案，並將其記錄型別和欄位對應至GenStudio工作區。 完成設定後，您可以在GenStudio中開啟工作區的記錄。

您必須具備下列條件：

* 存取Workfront Planning和GenStudio for Performance Marketing。
* 要連結至工作區的Adobe雲端儲存空間專案。 組織管理員可以在Adobe Admin Console中建立一個。

  如需詳細資訊，請參閱[管理Adobe儲存空間](https://helpx.adobe.com/tw/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)。<!--ensure this site still works-->

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
<p>任何Workfront或工作流程以及任何Planning套件</p> 
或
<p>以獨立產品形式購買時的任何Planning套件</p>

</td> 
   <tr> 
<td> 
   <p> 其他產品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Adobe Admin Console設定</p> </td> 
   <td> 
   <p> 您必須在Adobe Admin Console中建立Adobe儲存雲端專案 </p>

<p>如需詳細資訊，請參閱<a href="https://helpx.adobe.com/tw/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies">管理專案</a>

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>規劃標準</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Adobe Workfront存取層級設定</p></td> 
   <td> <p>當您同時具有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到Workfront存取層級</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing使用者角色</p></td> 
   <td><p><ul><li>任何GenStudio使用者角色（如果您需要存取行銷活動、產品和角色）</li>
   <li>GenSudio System Manager （如果您需要存取「啟用」） <!--and Events--></li></ul>
   如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">使用者角色和許可權</a>。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>  
   <p>在Workfront規劃中： </p>
   <ul>
   <li><p>管理工作區的許可權 <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> 在Adobe GenStudio for Performance Marketing中建立許可權以建立專案</p></li></ul>
   </td>  
</tbody> 
</table>

如需Adobe Workfront Planning存取權的相關資訊，請參閱[Adobe Workfront Planning存取權概觀](/help/quicksilver/planning/access/access-overview.md)。

如需Adobe GenStudio for Performance Marketing的詳細資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home)。

+++ 

## 啟用Workfront規劃工作區至GenStudio

1. 在Workfront Planning中，開啟您要啟用的工作區。
1. 按一下工作區名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**啟用GenStudio**。

   **讓工作區GenStudio**&#x200B;啟用方塊開啟，包括以下步驟：

   1. **ACPC專案**：選取您要與此工作區同步的&#x200B;**ACPC專案** （Adobe雲端儲存空間專案），然後按一下[下一步]&#x200B;**。**&#x200B;使用者可透過此專案存取GenStudio中的工作區。

      ![啟用工作區GenStudio - ACPC專案步驟](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **記錄型別**：將工作區的記錄型別對應到GenStudio所需的六種記錄型別：

      * 行銷活動
      * 產品
      * 人物誌
      * 管道
      * 區域
      * 啟用

      請針對每個專案，開啟清單並選取相符的Planning記錄型別，或選取&#x200B;**新增**&#x200B;以建立它，然後按一下&#x200B;**下一步**。

      ![啟用工作區GenStudio — 記錄型別步驟](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **欄位**：對應每個記錄型別的欄位。 使用對話方塊頂端的索引標籤，在記錄型別之間移動。 針對每個欄位，選取相符的Planning欄位，或選取&#x200B;**新增**&#x200B;以建立欄位。

      對所有記錄型別重複欄位設定。

      ![啟用工作區GenStudio — 欄位步驟](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. 檢閱並解決任何警告。

      例如，新欄位可以成為記錄型別的主要欄位，或者已使用的欄位別名已重新命名（如果您已經有名為「Regions」的欄位，則匯入的欄位可能會變成「Regions 2」）。

      對應&#x200B;**狀態**&#x200B;欄位會新增必要選項。

   1. 點擊&#x200B;**發佈**。

      工作區啟用時會顯示確認訊息。 對應記錄型別會在工作區中標示。

      對應為可從GenStudio存取的記錄型別卡片上有新的&#x200B;**Adobe**&#x200B;圖示。

      ![具有Adobe圖示的行銷活動記錄型別](assets/campaigns-record-type-card-with-adobe-icon.png)

1. 開啟GenStudio，選取&#x200B;**行銷活動**，然後按一下畫面左下角您為此設定所原始設定的&#x200B;**ACPC專案**。 檢閱匯入的記錄型別和欄位。

   >[!TIP]
   >
   >您只會看到Adobe Cloud Storage專案成員資格允許的記錄。
