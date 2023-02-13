---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Marketo模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Marketo]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2014'
ht-degree: 0%

---

# [!DNL Marketo] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Marketo]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL Marketo] 模組，您必須 [!DNL Marketo] 帳戶。

## Connect [!DNL Marketo] 到Workfront Fusion {#connect-marketo-to-workfront-fusion}

您可以建立與 [!DNL Marketo] 直接從內部 [!DNL Marketo] 模組。

1. 在任何 [!DNL Marketo] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 輸入 [!DNL Marketo] 帳戶或 [!DNL Marketo] [!UICONTROL 蒙奇金] ID. 這是指派給您帳戶的基本URL或端點的唯一部分，您可使用這些URL或端點來存取 [!DNL Marketo] 透過 [!UICONTROL REST] API。 有關查找此資訊的說明，請參閱 [基本URL](https://developers.marketo.com/rest-api/base-url/) 在 [!DNL Marketo] 檔案。
1. 輸入 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼]. 有關查找這些內容的說明，請參閱 [驗證](https://developers.marketo.com/rest-api/authentication/) 在 [!DNL Marketo] 檔案。
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Marketo] 模組及其欄位

設定時 [!DNL Marketo] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Marketo] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

* [[!UICONTROL 監看記錄]](#watch-records)
* [[!UICONTROL 監看事件（即時）]](#watch-events-instant)

#### [!UICONTROL 監看記錄]

此觸發模組會在建立或更新記錄時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要建立的記錄類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL活動]</strong> </p> <p>選取您要監看的活動類型。 </p> <p>模組只會監視新活動。<br></p> </li> 
     <li> <p><strong>[!UICONTROL銷售機會]</strong> </p> <p>選擇您要監視新記錄、更新記錄、新記錄和更新記錄，還是特定欄位更新。 如果您選取觀看特定欄位更新，請選取您要讓模組觀看的欄位。</p> </li> 
     <li> <p><strong>[!UICONTROL程式]</strong> </p> <p>選擇您要監視新記錄、更新記錄，還是新記錄和更新記錄。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監看事件（即時）]

此觸發模組會在建立或更新記錄時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>輸入要模組使用的網頁連結。</p> <p>如需Webhook的詳細資訊，請參閱 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
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
* [[!UICONTROL 將銷售機會添加到清單]](#add-leads-to-a-list)
* [[!UICONTROL 從清單中刪除銷售機會]](#remove-leads-from-a-list)
* [[!UICONTROL 排程促銷活動]](#schedule-a-campaign)
* [[!UICONTROL 複製方案]](#copy-a-program)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Marketo] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Marketo] 模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑 <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion]為您添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射在每個方案執行週期中希望模組使用的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄]

此動作模組會在 [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要建立的記錄類型。</p> 
    <ul> 
     <li> <p>[!UICONTROL公司]</p> </li> 
     <li> <p>[!UICONTROL資料夾]</p> </li> 
     <li> <p>[!UICONTROL銷售機會]</p> </li> 
     <li> <p>[!UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇要映射的欄位]</td> 
   <td>如果要建立公司或銷售機會，請選擇要在建立新記錄時設定值的欄位，然後為這些欄位輸入值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL程式類型]</td> 
   <td>如果要建立方案，請選擇要建立的方案類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL程式通道] </td> 
   <td>如果要建立方案，請選擇要建立方案的方案渠道。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾] / [!UICONTROL程式名]</td> 
   <td>如果要建立資料夾或程式，請輸入或映射新記錄的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td> <p>如果要建立資料夾或程式，請輸入或映射新記錄的說明。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL父資料夾ID]</td> 
   <td>如果要建立資料夾或程式，請輸入或映射要建立新記錄的父資料夾的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL成本]</td> 
   <td>如果要建立方案，請添加任何成本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td>如果要建立程式，請新增任何標籤</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會使用其ID更新現有記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要建立的記錄類型。</p> 
    <ul> 
     <li> <p>[!UICONTROL公司]</p> </li> 
     <li> <p>[!UICONTROL銷售機會]</p> </li> 
     <li> <p>[!UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL公司] / [!UICONTROL銷售機會] / [!UICONTROL計畫ID]</td> 
   <td>輸入或映射要更新的記錄ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇要映射的欄位]</td> 
   <td>如果要更新公司或銷售機會，請選擇要更新其值的欄位，然後為這些欄位輸入值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL程式名]</td> 
   <td>如果要更新方案，請輸入或映射方案的新名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td> <p>如果要更新方案，請輸入或映射方案的新說明。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL開始日期]</td> 
   <td>如果要更新方案，請輸入或映射方案的新起始日期。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結束日期]</td> 
   <td>如果要更新方案，請輸入或映射方案的新終止日期。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL成本]</td> 
   <td>如果要更新程式，請添加任何成本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td>如果要更新程式，請新增任何標籤</td> 
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
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案ID]</td> 
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
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID]</td> 
   <td>輸入或映射要新檔案所在的資料夾的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td>輸入已上傳檔案的說明。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會使用記錄的ID來讀取記錄的相關資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要建立的記錄類型。</p> 
    <ul> 
     <li> <p>[!UICONTROL促銷活動]</p> </li> 
     <li> <p>[!UICONTROL公司]</p> </li> 
     <li> <p>[!UICONTROL銷售機會]</p> </li> 
     <li> <p>[!UICONTROL清單]</p> </li> 
     <li> <p>[!UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選擇要包含在此模組的輸出包中的資訊。 欄位根據您選取的[!UICONTROL記錄類型]而可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; ID]</td> 
   <td>輸入或映射要檢索相關資訊的對象的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將銷售機會添加到清單]

此動作模組會使用銷售機會ID，將一或多個銷售機會新增至清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單ID]</td> 
   <td>輸入或映射要添加銷售機會的清單的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL潛在客戶ID]</td> 
   <td> <p>對於您要新增至清單的每個銷售機會，按一下 <b>[!UICONTROL添加]</b>，然後輸入或對應您要新增的銷售機會ID。 您最多可以新增300個銷售機會，讓模組新增至清單。</p> <p>按一下對應切換按鈕，對應您要新增至清單的現有銷售機會集合。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從清單中刪除銷售機會]

此動作模組會使用銷售機會ID，從清單中移除一或多個銷售機會。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單ID]</td> 
   <td>輸入或映射要刪除銷售線索的清單的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL潛在客戶ID]</td> 
   <td> <p>對於要從清單中移除的每個銷售機會，按一下 <b>[!UICONTROL添加]</b>，然後輸入或對應您要移除之銷售機會的ID。 您最多可以新增300個銷售機會，讓模組從清單中移除。 </p> <p>按一下對應切換按鈕，以對應您要從清單中移除的現有銷售機會集合。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 排程促銷活動]

此動作模組會針對特定日期排程現有促銷活動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL促銷活動ID]</td> 
   <td>輸入或對應您要排程的促銷活動ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL日期計畫]</p> </td> 
   <td>選取要執行促銷活動的日期。 如果此欄位留空，則促銷活動會在情境開始後5分鐘執行。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製方案]

此動作模組會使用現有程式的ID來製作程式的復本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL現有程式ID]</td> 
   <td>輸入或映射要複製的程式的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL新程式名]</p> </td> 
   <td> <p>輸入或映射新程式的名稱</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID]</td> 
   <td>輸入或映射要新程式所在的資料夾的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 清單記錄]](#list-records)
* [[!UICONTROL 搜索記錄]](#update-a-record)

#### [!UICONTROL 清單記錄]

此動作模組會擷取特定類型的所有記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要列出的記錄類型。</p> 
    <ul> 
     <li> <p>[!UICONTROL讀取所有促銷活動]</p> </li> 
     <li> <p>[!UICONTROL讀取所有程式]</p> </li> 
     <li> <p>[!UICONTROL讀取所有銷售機會] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位]</td> 
   <td>如果您已選擇檢索銷售機會，請選擇要從清單還是從程式檢索銷售機會。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選擇要包含在此模組的輸出包中的資訊。 欄位根據您選取的[!UICONTROL記錄類型]而可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索記錄]

此搜索模組檢索符合特定搜索條件的記錄清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Marketo] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要搜索的記錄類型。</p> 
    <ul> 
     <li> <p>[!UICONTROL促銷活動]</p> </li> 
     <li> <p>[!UICONTROL銷售機會]</p> </li> 
     <li> <p>[!UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL欄位]</p> </td> 
   <td> <p>選擇要按名稱、程式名或工作區名稱進行搜索。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td>針對您要搜尋的每個值，按一下 <b>[!UICONTROL添加項]</b> 並輸入值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>
