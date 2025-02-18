---
title: 從Workfront Planning建立Workfront物件
description: 當您從Workfront Planning中的其他記錄連線物件時，可以建立Workfront物件型別。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 597d8db034269e673dbe46e8c0f4934bf9509e2f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 從Workfront Planning <!--as you connect them to records-->建立Workfront物件

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">本頁標示的資訊是指尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

<!--
You can create Adobe Workfront objects from Workfront Planning in the following ways: 

* As you try to connect Workfront objects from Planning records

    This article describes how to create Workfront objects from Workfront Planning as you try to connect them from Planning records. 
* <span class="preview">When you use automations from a record's page.</span> 

    For information about creating Workfront objects using automations, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). 
-->

當您連線Workfront記錄與下列Workfront物件型別時，可以從Workfront Planning建立下列Workfront物件型別：

* 專案
* 專案組合
  <!--* <span class="preview">Programs</span>-->

>[!IMPORTANT]
>
>* 從記錄連線專案和投資組合時，您只能在Workfront中建立專案和投資組合。
>
>* 從Workfront Planning中的記錄連線方案、群組或公司時，您無法建立它們。
>

<!--replace the IMPORTANT above with this when we release programs: 

>[!IMPORTANT]
>
>* You can create only projects, portfolios, and <span class="preview">programs</span> in Workfront when connecting them from a record. 
>
>* You cannot create groups or companies when connecting them from a record in Workfront Planning. 
>
-->

您可以從連線欄位在Workfront規劃的下列區域中連線專案與投資組合<!--<span class="preview"> and programs </span>-->：

* 記錄型別的表格檢視
* 記錄的詳細資訊頁面或預覽方塊

如需有關連線Planning記錄與Workfront物件的資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

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
   <td> 標準
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p> 
   <p>將記錄連線至要建立的物件型別（專案與投資組合）時，可在Workfront中編輯其存取權。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>管理您要新增記錄的工作區的許可權。 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
   <p>管理Workfront物件（專案組合）的許可權以新增子物件（專案）。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從Workfront Planning連線物件與記錄時，建立Workfront物件的先決條件

您必須具備下列條件，才能透過從現有記錄連線來新增專案或投資組合：

* 記錄型別已連線至Workfront專案或投資組合<!--or <span class="preview">programs</span>-->。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
* 記錄。 如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。
* Workfront Planning和Workfront中的正確存取和許可權，如本文中[存取需求](#access-requirements)一節所述。

## 當您從Workfront Planning將專案與記錄連線時，建立專案

若要在從其他記錄連線專案時建立專案：

1. 移至記錄的詳細資訊頁面或記錄型別的表格，並開始將Workfront Planning記錄與Workfront專案連線，如文章[連線記錄](/help/quicksilver/planning/records/connect-records.md)中所述。

1. （條件式） <!--<span class="preview">Click **Add project**</span> Or Start typing the name of a project, then click **Add project** if you cannot find it.-->如果您嘗試從其他記錄的已連線記錄欄位新增專案時找不到專案，請新增名稱，然後按一下&#x200B;**新增專案**。 「新增」按鈕後面接著您輸入的專案名稱。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![從連線欄位連線時新增專案](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview"> **建立專案**&#x200B;方塊開啟。</span>

1. <span class="preview">（選擇性）更新&#x200B;**專案名稱**。 根據預設，專案會以您從記錄連線時新增為搜尋專案的名稱命名。</span>
1. <span class="preview"> （選擇性）選取&#x200B;**專案範本**。 如果您未選取範本，Workfront會建立不含任務的空白專案。</span>
1. <span class="preview">按一下&#x200B;**建立**。</span>
1. <span class="preview">（條件式）如果您選取從範本建立專案，請依照文章[使用範本](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)建立專案中的步驟完成新增專案。</span>

   新專案已建立並新增至所選記錄的已連線欄位。

1. （可選）從Workfront計畫按一下新專案的名稱，以在Workfront中開啟專案頁面，並對專案進行其他更新。

## 在連結投資組合與Workfront Planning的記錄時建立投資組合

若要在從Planning記錄連線投資組合時建立投資組合：

1. 移至記錄的詳細資訊頁面或記錄型別的表格，然後開始將Workfront Planning記錄與Workfront投資組合連線，如文章[連線記錄](/help/quicksilver/planning/records/connect-records.md)中所述。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. （條件式） <!--<span class="preview">Click **Add portfolio**</span> Or Start typing the name of a portfolio, then click **Add portfolio** if you cannot find it.-->如果您嘗試從其他記錄的已連線記錄欄位新增投資組合時找不到投資組合，請新增名稱，然後按一下&#x200B;**新增投資組合**。 「新增」按鈕後面也會跟著您輸入的投資組合名稱。

   ![從連線欄位連線時新增投資組合](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   投資組合隨即建立並新增至您所選記錄的連線欄位。

1. （選用）從Workfront Planning按一下新投資組合的名稱，即可在Workfront中開啟投資組合頁面，並對投資組合進行其他更新。

<!--

<div class="preview">

## Create programs as you connect them with records from Workfront Planning

To create programs as you are connecting them from Planning records: 

1. Go to a record's details page or to the record type's table and start connecting Workfront Planning records with Workfront portfolios, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    ******** at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed." ***********
    
1. Click **Add program** 

    Or 
    
    Start typing the name of a program, then click **Add program** if you cannot find it. The Add button is followed by the program name you typed. 

    ![Add Workfront program when connecting it from connection field](assets/add-wf-program-when-connecting-it-from-connection-field.png)

    The **Create program** box opens.

1. Update the **Program name**. This is a required field.
1. Choose a **Portfolio** from the drop-down, or start typing the name of a portfolio, then select it when it displays in the list. This is a required field. 
1. Click **Create**.

    The program is created and added to the connection field of the record you selected. 

1. (Optional) Click the name of the new program from Workfront Planning to open the program's page in Workfront and make additional updates to it. 

</div>

-->