---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Workfront主機板模組
description: 您可以使用Adobe Workfront面板聯結器在Workfront面板中自動化您的流程，並將其連線到第三方應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
source-git-commit: 074bcf15c61f9c0c75cebf774b15baf7fe383f35
workflow-type: tm+mt
source-wordcount: '2118'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 主機板模組

>[!NOTE]
>
>此聯結器目前處於Beta版。

Adobe Workfront展示板是彈性的工具，可讓團隊透過提供對包含欄和卡片的共用展示板的存取權進行共同作業。

您可以使用Adobe Workfront面板模組來讀取或更新記錄、對Workfront面板API進行API呼叫，或當面板上發生動作時觸發情境。

如需Workfront面板的一般資訊，請參閱 [展示板概述](/help/quicksilver/agile/boards-overview.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td>
  <td> <p>任何</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td>
   <td> <p>新增：標準</p><p>或</p><p>目前： [！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 工作自動化與整合]，請參閱[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).
Adobe Workfront面板模組及其欄位

## 先決條件

您必須先在Adobe Workfront中設定主機板，才能連線至該主機板。

## 建立與Workfront展示板的連線

>[!NOTE]
>
>您可以使用Workfront連線來連線至Workfront面板，或是建立個別的Workfront面板連線。

若要建立Workfront面板連線：

1. 在任何 [!DNL Adobe Workfront Boards] 模組，按一下 **[!UICONTROL 新增]** ，位於「連線」方塊旁。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[！UICONTROL連線名稱]</td>
          <td>
            <p>輸入此連線的名稱。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL環境]</td>
          <td>選取您要連線到生產或非生產環境。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL型別]</td>
          <td>選取您是要連線到服務帳戶還是個人帳戶。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者端ID]<p>（可選）</p></td>
          <td>輸入您的 [!DNL Adobe] [！UICONTROL使用者端識別碼]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者端密碼]<p>（可選）</p></td>
          <td>輸入您的 [!DNL Adobe] [！UICONTROL使用者端密碼]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL驗證URL]<p>（可選）</p></td>
          <td>輸入您的Workfront執行個體將用來驗證此連線的URL。 <p>預設值為 <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL主機前置詞]</td>
          <td>輸入您的主機前置詞。<p>預設值為 <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## Adobe Workfront面板模組及其欄位

當您設定Workfront面板模組時， [!DNL Workfront Fusion] 顯示下列欄位。 除此之外，可能還會顯示其他Workfront面板欄位，視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [卡片](#cards)
* [展示板](#boards)
* [欄](#columns)
* [標記](#tags)
* [其他](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### 卡片

* [新增檢查清單項目](#add-checklist-item)
* [新增子任務](#add-subtask)
* [建立卡片](#create-a-card)
* [移動卡片](#move-a-card)
* [讀取卡片](#read-a-card)
* [更新卡片](#update-a-card)

#### 新增檢查清單項目

此動作模組會將檢查清單專案新增至指定的卡片。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡片ID]</td> 
   <td>輸入或對應您要新增檢查清單專案的卡片ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檢查清單專案]</td> 
   <td>針對您要新增的每個檢查清單專案，按一下「新增專案」，輸入檢查清單專案的名稱，然後選取該專案是否已完成。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 新增子任務

此動作模組會將子任務新增到展示板中的卡片。 此卡片必須是已連線的卡片。 子任務也會新增至卡片所代表的Workfront任務。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL父卡片ID]</td> 
   <td>輸入或對應您要新增子任務的卡片ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應包含您要新增子任務之卡片之展示板的ID。<p>在Workfront中檢視展示板時，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL名稱]</td> 
   <td>輸入或對應新子工作的名稱。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 建立卡片

此動作模組會在Workfront展示板上建立新卡片。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應您要新增卡片之主機板的ID。<p>在Workfront中檢視展示板時，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料行ID]</td> 
   <td>輸入或對應您要新增子工作的資料行ID。<p>您可以從讀取展示板模組傳回的資訊中找到標籤ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL名稱]</td> 
   <td>輸入或對應新卡片的名稱。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 移動卡片

此動作模組會將卡片移至相同展示板上的不同欄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡片ID]</td> 
   <td>輸入或對應您要移動之卡片的ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應包含您要移動之卡片的主機板ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目的地資料行ID]</td> 
   <td>輸入或對應您要移動卡片的目標欄ID。<p>您可以從讀取展示板模組傳回的資訊中找到標籤ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL至索引]</td> 
   <td>輸入或對應您要卡片在新欄中的位置。<p>索引0中資料行的頂端位置。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 讀取卡片

此動作模組會擷取特定卡片的相關資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡片ID]</td> 
   <td>輸入或對應您要讀取的卡片ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 更新卡片

此動作模組會更新您指定之卡片的資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡片ID]</td> 
   <td>輸入或對應您要更新的卡片ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應包含要更新卡片之展示板的ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL名稱]</td> 
   <td>輸入或對映卡片的新名稱。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡片ID]</td> 
   <td>輸入或對應卡片/\的新說明。</p></td> 
  </tr> 
 </tbody> 
</table>

### 展示板

* [建立展示板](#create-a-board)
* [讀取展示板](#read-a-board)

#### 建立展示板

此動作模組會在Workfront中建立展示板。 您可以指定要建立的電路板型別。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板名稱]</td> 
   <td>輸入或對映新展示板的名稱。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL型別]</td> 
   <td>選取您要建立的電路板型別。</td> 
  </tr> 
 </tbody> 
</table>

#### 讀取展示板

此動作模組會傳回單一展示板的資訊，例如展示板的卡片、欄、標籤和成員。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應您要擷取資訊之展示板的ID。<p>在Workfront中檢視展示板時，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
 </tbody> 
</table>

### 欄

#### 建立欄

此動作模組會在指定的展示板上建立新欄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應您要新增欄的展示板ID。<p>在Workfront中檢視展示板時，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄名稱]</td> 
   <td>輸入或對應新欄的名稱。</td> 
  </tr> 
 </tbody> 
</table>

### 標記

* [新增標籤至卡片](#add-card-tag)
* [建立標籤](#create-a-tag)

#### 新增標籤至卡片

此動作模組會將標籤新增至卡片。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL卡片ID]</td> 
   <td>輸入或對應您要新增標籤的卡片ID。<p>在Workfront中檢視卡片時，您可以在URL中找到卡片ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應包含您要新增標籤之卡片的主機板ID。<p>在Workfront中檢視展示板時，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標籤ID]</td> 
   <td>輸入或對應您要新增之標籤的ID。<p>您可以從讀取展示板模組傳回的資訊中找到標籤ID。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 建立標籤

此動作模組會建立新標籤並為其指派顏色。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL展示板ID]</td> 
   <td>輸入或對應您要建立標籤之展示板的ID。<p>在Workfront中檢視展示板時，您可以在URL中找到展示板ID。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標籤名稱]</td> 
   <td>輸入或對映新標籤的名稱。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標籤顏色]</td> 
   <td>選取此標籤的顏色。</td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### 進行自訂API呼叫

此動作模組會對Workfront看板API進行自訂呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
      <td> <p>您可以使用現有的Workfront連線來連線至Workfront面板，或使用特定的Workfront面板連線。 </p><p>如需有關連線您的電腦的指示 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">建立與Workfront展示板的連線</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>輸入相對於<code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p><p>對於大多數展示板呼叫，方法是POST的。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。 這會決定請求的內容型別。</p> <p>例如，<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>若為Workfront面板，此區段通常會保留空白。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以JSON內嵌Graphql的形式，新增API呼叫的內文內容 </p> <p>範例：</p><p>此範例會更新欄名稱。 您可以包含 <code>boardId</code> 和 <code>columnId</code> 作為GUID，以硬式編碼或對映自先前的模組。<p><pre>{

  &quot;query&quot;： &quot;mutation { updateColumn(boardId： \&quot;\&quot;， columnId： \&quot;\&quot;， updateColumnInput： { name： \&quot;\&quot; }) { id name }}&quot;

}</pre><p>注意：  <p>使用條件陳述式時，例如 <code>如果</code> 在JSON中，將引號放在條件陳述式之外。</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
