---
title: 在構思空間建立簡報
description: 本文說明如何在創意空間進行腦力激盪和策略化，以建立簡報。 您可以將完成的創意力摘要匯出至檔案或Workfront Planning，以建立或更新記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
source-git-commit: cf783443d618874e1241d91895bcc78d78db23df
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%
---

# 在構思空間建立簡報

<!--add to TOC and miniTOC-->

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它只能做為&#x200B;**創意空間Beta**&#x200B;程式的一部分。</span>

<span class="preview">如需詳細資訊，請參閱[開始使用Adobe Workfront Planning的構思空間](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。</span>

{{planning-important-intro}}

使用Adobe Workfront Planning的新功能Ideation Space，您可以將簡報轉換為Planning記錄。 匯出的摘要會建立新記錄或更新現有記錄。

本文說明如何在創意空間進行腦力激盪和策略化，以建立簡報。 若要建立或更新記錄，請將完成的創意力摘要匯出至檔案或Workfront Planning。

## 存取權要求

+++ 展開以檢視本文中功能的存取需求。 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
<ul> 
<li><p>具有Planning套件的任何Workfront或工作流程</p></li>
或
<li><p>以獨立產品形式購買時的任何Planning套件</p></li></ul>
   </td> 
<!--
<tr> 
<td role="rowheader"><p>Additional products</p></td> 
<td><ul>
<li><p>Adobe GenStudio for Performance Marketing</p></li>
<li><p>Adobe Customer Journey Analytics</p></li>
</ul>
</td> 
</tr> 
-->
  <tr> 
   <td role="rowheader"><p>Adobe工作流程授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> 
   <ul>
   <li><p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   </li>
   <li><p>必須取消選取存取層級中的停用創意空間設定</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>提供或更高許可權給您要新增記錄的工作區和記錄型別 </p>
      <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
      <p>檢視Workfront物件的許可權，以將它們新增至摘要 <!--not sure if this is available--></p>
      <p>創意力空間的編輯器許可權以建立簡報</p>
   </td> 
  </tr>  
    <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++  

## 建立創意力空間簡報

1. 在Workfront Planning中開始，使用創意空間建立或編輯記錄。

   如需詳細資訊，請參閱[從創意空間摘要建立Planning記錄](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)。
1. 當&#x200B;**創意空間**&#x200B;開啟時，請使用提供的提示來說明您要建立的簡報。

   例如，輸入「為K-12學生建立返校行銷活動，以在美國進行8月份的活動，對象為美國的家長和教師」。  為了儘可能提供簡短，請儘可能指明可用於何種行銷活動、時間表、利害關係人和其他詳細資訊的資訊。

1. 按一下&#x200B;**開始構思**。

   開啟後，創意空間代理程式將進行以下步驟：

   1. **資料擷取與合成**：從連線的來源提取相關資訊。 例如：

      * 現有記錄型別或您開始使用的現有記錄型別。
      * 您可能在創意力空間上傳的最近檔案。
      * 符合提示條件的網頁資訊。

        >[!TIP]
        >
        >必須開啟網頁搜尋設定，AI才能在網頁上尋找資訊。\
        >如需詳細資訊，請參閱本文中的[設定創意空間](#configure-the-ideation-space)一節。
        >
   1. **對象定義**：根據歷史模式識別或建議目標對象引數
   1. **策略框架**：建構行銷活動的策略敘述
   1. **傳訊與概念構想**：產生初始訊息選項與創意概念方向
   1. **簡短的產生與規劃移交**：產生結構化的簡報，並回饋至Workfront規劃工作區

      當創意力代理程式完成收集所有資訊的流程時，會發生下列情況：

      * 系統隨即建立5張卡片，並根據相關和類似資訊加以整理。

        這些卡片的標題在建立要求的記錄時使用了各種步驟，以便於辨識。

        例如，它們可以命名為：

        * 規劃
        * 時間軸
        * 區段
        * 力學
        * 傳送訊息

      卡片標題是根據每張卡片在構思上的自訂內容。

      * 卡片會放置在相同的框架中，表示這是單一創意的結果。

      * 系統會建立簡報，並顯示在創意力空間左下角的預覽影像中。<!--add screen shot??-->

      摘要包含系統認為與您探索的想法相關的建議欄位。

1. （選擇性）按一下右上角的&#x200B;**說明**&#x200B;圖示![](assets/more-information-icon.png)，取得鍵盤快速鍵清單，協助您瀏覽創意空間。

1. （選擇性）按一下每張卡片底部的&#x200B;**來源**，瞭解資訊的收集來源。

   您可從Workfront Planning或網頁匯入資訊。
1. （選擇性）使用卡片上的向上或向下縮圖示提供意見反應。<!--is this still available??-->
1. 按一下卡片或按一下包含所有卡片的框架，然後按一下&#x200B;**新增至簡報**，將其資訊新增至簡報。

   Workfront會將其找到的每個資訊與最可能儲存它的欄位進行比對。

   例如，時間表會新增到日期型別欄位，說明會新增到段落型別欄位。
   1. （視條件而定）按一下卡片，然後按一下&#x200B;**詢問AI至……**&#x200B;以取得下一個步驟的想法，然後再將資訊新增至簡報。 答案取決於每張卡片資訊的內容。
   1. 按一下創意力空間左上角的&#x200B;**新增檔案**&#x200B;圖示![新增檔案圖示](assets/add-documents-in-ideation-space.png)，將檔案上傳至該空間。 您可以新增先前已新增至空間的新檔案或檔案。

      >[!TIP]
      >
      >必須開啟檔案設定，才能存取檔案並將檔案上傳至空間。
      >如需詳細資訊，請參閱本文中的[設定創意空間](#configure-the-ideation-space)一節。
      > 
   1. 按一下&#x200B;**新增WF分類卡**&#x200B;圖示![從Workfront Planning新增](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised-->，並選取連線的記錄型別，然後選取每個型別的記錄，將該記錄的資訊新增至您選取的記錄型別。

      系統會為您選取要新增至空間的記錄建立卡片。 記錄型別會顯示在記錄卡片的左上角。
   1. （選擇性）按一下&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**在Workfront中檢視**。

      記錄的詳細資訊頁面會在Workfront Planning的另一個瀏覽器標籤中開啟。
   1. （可選）選取創意力框架或卡片，按一下「刪除」圖示，然後按一下「刪除」以進行確認。 卡片會從創意力空間移除。

      當您刪除與儲存檔案或記錄相對應的卡片時，專案會從創意空間移除，但會保留在各自的應用程式中。

1. （選擇性）隨時使用右下角的&#x200B;**詢問任何事項**&#x200B;方塊來調整您的構思。

   例如，針對特定卡片輸入`regenerate`，讓AI使用更新的內容重做該卡片。 創意空間會重新執行其推理步驟（搜尋、合成、引證）並更新受影響的卡片。

1. （選擇性）在&#x200B;**詢問任何事項**&#x200B;方塊中，詢問新問題以開始新構思。

   空間重新執行其推理步驟後，會產生一組新的卡片。

1. （選擇性）按一下任何構思卡片組中的其中一個紫色聯結器，然後按一下&#x200B;**複製以提示列**&#x200B;圖示以重新執行構思推理。

   ![複製到提示列圖示](assets/copy-to-prompt-bar-icon-highlighted.png)

1. （選擇性）按一下頁面頂端的&#x200B;**還原**&#x200B;或&#x200B;**重做**&#x200B;圖示![還原和重做圖示](assets/undo-redo-icons.png)以取消或反轉動作。
1. 縮小範圍以檢視完整圖片：您的原始行銷活動目標、所有AI產生的概念卡和引文、其他檔案，以及您拉入的實際Workfront Planning記錄（產品、角色等）。 左下角的&#x200B;**簡介**&#x200B;摘要卡片會將其拉在一起。

1. 按一下左下角的簡介預覽影像並檢閱簡介，然後按一下下列其中一個選項：

   * **匯出至檔案**。 您可以將簡介匯出為下列檔案型別：

     * PDF
     * 字詞
     * PowerPoint （使用或不使用範本）
   * **匯出至Workfront Planning**。 匯出會覆寫Workfront Planning中記錄的所有現有欄位資料。

   這樣會使用其他資訊完成記錄的建立，並將其新增到您最初選取的記錄型別。

   如需有關使用摘要更新Planning記錄的詳細資訊，請參閱文章[從創意空間摘要建立Planning記錄](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)中的「關於使用創意空間建立記錄的考量事項」一節。


## 設定創意力空間

創意力空間有控制項，可設定您在畫面上看到的內容，並幫助您導覽該空間。

1. 按一下&#x200B;**設定**&#x200B;圖示![設定](assets/setting-icon.png)以控制AI從何處提取資訊，然後從下列&#x200B;**Source型別**&#x200B;中選擇：

   * **檔案** — 檔案已上傳至選取的空間
   * **網頁搜尋** — 外部網頁搜尋
   * **CJA** — Adobe Customer Journey Analytics

1. 按一下「**儲存**」。

1. 按一下&#x200B;**說明**&#x200B;圖示![說明圖示](assets/more-information-icon.png)以檢閱您可用來瀏覽創意空間或選取其他縮放值的鍵盤快速鍵。

   從下列縮放等級中選擇：

   * 縮放至100%
   * 縮放至200%
   * 縮放以符合

   或使用下列捷徑之一在頁面上導覽：

   | 動作 | 快速鍵 |
   |---|---|
   | 放大/縮小 | Ctrl/⌘ + / − |
   | 縮放以符合/符合選取範圍 | — |
   | 縮放至游標 | Ctrl/⌘ +捲動 |
   | 平移畫布 | 空格鍵+拖曳 |
   | 顯示/隱藏點格線 | G |

1. 按一下「搜尋」圖示以搜尋創意空間中的專案，然後按一下顯示在清單中的專案以導覽至該專案。








