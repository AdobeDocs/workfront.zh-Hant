---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Marketo模組
description: 在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Marketo]，以及將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2062'
ht-degree: 0%

---

# [!DNL Marketo] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Marketo]，以及將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL Marketo] 模組，您必須擁有 [!DNL Marketo] 帳戶。

## Connect [!DNL Marketo] 至Workfront Fusion {#connect-marketo-to-workfront-fusion}

您可以建立與的連線 [!DNL Marketo] 直接從內部帳戶 [!DNL Marketo] 模組。

1. 在任何 [!DNL Marketo] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 輸入您的 [!DNL Marketo] 帳戶或 [!DNL Marketo] [!UICONTROL Munchkin] ID。 這是指派給您帳戶且您用來存取的基礎URL或端點的唯一部分 [!DNL Marketo] 透過其 [!UICONTROL REST] API。 如需尋找此專案的指示，請參閱 [基本URL](https://developers.marketo.com/rest-api/base-url/) 在 [!DNL Marketo] 說明檔案。
1. 輸入您的 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼]. 如需尋找這些專案的指示，請參閱 [驗證](https://developers.marketo.com/rest-api/authentication/) 在 [!DNL Marketo] 說明檔案。
1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

## [!DNL Marketo] 模組及其欄位

當您設定 [!DNL Marketo] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Marketo] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

* [[!UICONTROL 觀看記錄]](#watch-records)
* [[!UICONTROL 觀看活動（即時）]](#watch-events-instant)

#### [!UICONTROL 觀看記錄]

建立或更新記錄時，此觸發模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL活動]</strong> </p> <p>選取您要觀看的活動型別。 </p> <p>模組只會監視新活動。<br></p> </li> 
     <li> <p><strong>[！UICONTROL銷售機會]</strong> </p> <p>選取是否要監視新記錄、更新的記錄、新記錄和更新的記錄，或特定欄位更新。 如果您選取觀看特定欄位更新，請選取您希望模組觀看的欄位。</p> </li> 
     <li> <p><strong>[！UICONTROL程式]</strong> </p> <p>選取您要監視新記錄、更新的記錄，或同時監視新記錄和更新的記錄。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看活動（即時）]

建立或更新記錄時，此觸發模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Webhook]</p> </td> 
   <td> <p>輸入您希望模組使用的webhook。</p> <p>如需Webhook的詳細資訊，請參閱 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 下載檔案]](#download-a-file)
* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 將潛在客戶新增至清單]](#add-leads-to-a-list)
* [[!UICONTROL 從清單中移除銷售機會]](#remove-leads-from-a-list)
* [[!UICONTROL 排程行銷活動]](#schedule-a-campaign)
* [[!UICONTROL 複製計畫]](#copy-a-program)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Marketo] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Marketo] 模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於 <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[！UICONTROL Workfront Fusion]會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期使用的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄]

此動作模組會在中建立新記錄 [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別。</p> 
    <ul> 
     <li> <p>[！UICONTROL公司]</p> </li> 
     <li> <p>[！UICONTROL資料夾]</p> </li> 
     <li> <p>[！UICONTROL銷售機會]</p> </li> 
     <li> <p>[！UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取要對應的欄位]</td> 
   <td>如果您要建立「公司」或「銷售機會」，請在建立新記錄時選取要為其設定值的欄位，然後輸入這些欄位的值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL程式型別]</td> 
   <td>如果您正在建立方案，請選取您要建立的方案型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL計畫頻道] </td> 
   <td>如果您正在建立方案，請選取您要建立方案的方案頻道。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾] / [！UICONTROL程式名稱]</td> 
   <td>如果您要建立資料夾或程式，請輸入或對應新記錄的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td> <p>如果您要建立資料夾或程式，請輸入或對應新記錄的描述。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL父資料夾ID]</td> 
   <td>如果您正在建立資料夾或程式，請輸入或對應您要建立新記錄的父資料夾ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成本]</td> 
   <td>如果您正在建立方案，請新增任何成本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤]</td> 
   <td>如果您正在建立方案，請新增任何標籤</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組使用其ID更新現有記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別。</p> 
    <ul> 
     <li> <p>[！UICONTROL公司]</p> </li> 
     <li> <p>[！UICONTROL銷售機會]</p> </li> 
     <li> <p>[！UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL公司] / [！UICONTROL銷售機會] / [！UICONTROL計畫ID]</td> 
   <td>輸入或對應您要更新的記錄ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取要對應的欄位]</td> 
   <td>如果您要更新「公司」或「銷售機會」，請選取要更新值的欄位，然後輸入這些欄位的值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL程式名稱]</td> 
   <td>如果您要更新方案，請輸入或對應方案的新名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td> <p>如果您要更新程式，請輸入或對應程式的新描述。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始日期]</td> 
   <td>如果您要更新程式，請輸入或對應程式的新開始日期。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結束日期]</td> 
   <td>如果您要更新方案，請輸入或對應方案的新結束日期。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成本]</td> 
   <td>如果您要更新程式，請新增任何成本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤]</td> 
   <td>如果您要更新程式，請新增任何標籤</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會使用檔案ID下載檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td>對應您要下載的檔案ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組會將新檔案上傳至 [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL來源檔案]</td> 
   <td>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾ID]</td> 
   <td>輸入或對應您要放置新檔案的資料夾ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入已上傳檔案的說明。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組使用記錄的ID來讀取記錄的相關資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別。</p> 
    <ul> 
     <li> <p>[！UICONTROL行銷活動]</p> </li> 
     <li> <p>[！UICONTROL公司]</p> </li> 
     <li> <p>[！UICONTROL銷售機會]</p> </li> 
     <li> <p>[！UICONTROL清單]</p> </li> 
     <li> <p>[！UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取要包含在此模組輸出組合中的資訊。 根據您選取的[！UICONTROL記錄型別]可使用欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL &lt;object&gt; ID]</td> 
   <td>輸入或對應您要擷取相關資訊之物件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將潛在客戶新增至清單]

此動作模組會使用銷售機會ID將一個或多個銷售機會新增到清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL清單ID]</td> 
   <td>輸入或對映您要新增潛在客戶的清單ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL銷售機會ID]</td> 
   <td> <p>針對您想要新增至清單的每個銷售機會，按一下 <b>[！UICONTROL新增]</b>，然後輸入或對應您要新增的潛在客戶ID。 您可以新增最多300個銷售機會，以便模組新增至清單。</p> <p>按一下地圖切換來對應您想要新增至清單的現有銷售機會集合。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從清單中移除銷售機會]

此動作模組會使用銷售機會ID從清單中移除一或多個銷售機會。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL清單ID]</td> 
   <td>輸入或對映您要移除潛在客戶的清單ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL銷售機會ID]</td> 
   <td> <p>針對您要從清單中移除的每個銷售機會，按一下 <b>[！UICONTROL新增]</b>，然後輸入或對映您要移除的潛在客戶ID。 您最多可以新增300個銷售機會，讓模組從清單中移除。 </p> <p>按一下地圖切換來對應您要從清單中移除的現有銷售機會集合。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 排程行銷活動]

此動作模組會為特定日期排程現有行銷活動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL促銷活動ID]</td> 
   <td>輸入或對應您要排程之行銷活動的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL日期排程]</p> </td> 
   <td>選取您要執行行銷活動的日期。 如果此欄位留空，行銷活動會在案例開始後5分鐘執行。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製計畫]

此動作模組會使用現有程式ID製作程式的副本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL現有計畫ID]</td> 
   <td>輸入或對應您要複製的程式ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL新計畫名稱]</p> </td> 
   <td> <p>輸入或對應新方案的名稱</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾ID]</td> 
   <td>輸入或對映您想要新程式所在的資料夾的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 清單記錄]](#list-records)
* [[!UICONTROL 搜尋記錄]](#update-a-record)

#### [!UICONTROL 清單記錄]

此動作模組會擷取特定型別的所有記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要列出的記錄型別。</p> 
    <ul> 
     <li> <p>[！UICONTROL讀取所有行銷活動]</p> </li> 
     <li> <p>[！UICONTROL讀取所有程式]</p> </li> 
     <li> <p>[！UICONTROL讀取所有銷售機會] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位]</td> 
   <td>如果您已選取要擷取銷售機會，請選取您要從清單還是從方案中擷取銷售機會。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取要包含在此模組輸出組合中的資訊。 根據您選取的[！UICONTROL記錄型別]可使用欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋記錄]

此搜尋模組會擷取符合特定搜尋條件的記錄清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Marketo] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要搜尋的記錄型別。</p> 
    <ul> 
     <li> <p>[！UICONTROL行銷活動]</p> </li> 
     <li> <p>[！UICONTROL銷售機會]</p> </li> 
     <li> <p>[！UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL欄位]</p> </td> 
   <td> <p>選取您要依名稱、方案名稱或工作區名稱搜尋。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td>針對您要搜尋的每個值，按一下 <b>[！UICONTROL新增專案]</b> 並輸入值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>
