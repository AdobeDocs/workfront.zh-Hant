---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: 位元組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Bynder]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 0%

---

# [!DNL Bynder] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Bynder]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Bynder] 模組，您必須 [!DNL Bynder] 帳戶。

## Connect [!DNL Bynder] 到Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [建立連線至 [!DNL Bynder] 從 [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [產生 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼] in [!DNL Bynder] （可選）](#generate-a-client-id-and-client-secret-in-bynder-optional)

### 建立連線至 [!DNL Bynder] 從 [!DNL Workfront Fusion]

您可以從 [!DNL Workfront Fusion] 至 [!DNL Bynder] 直接從內部 [!DNL Bynder] 模組。

1. 在任何 [!DNL Bynder] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選取 [!DNL Bynder] 要連接的域。
1. （選用）按一下 **[!UICONTROL 進階設定]**，然後輸入 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼].

   如需產生用戶端ID和用戶端密碼的相關指示，請參閱 [在 [!DNL Bynder] （可選）](#generate-a-client-id-and-client-secret-in-bynder-optional) 這篇文章。

1. 在 [!UICONTROL 登入] 視窗中，輸入您的使用者名稱（電子郵件地址）和密碼。
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

### 產生 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼] in [!DNL Bynder] （可選）

如果您想使用用戶端ID和用戶端密碼來建立連線，可以從 [!DNL Bynder] 帳戶。 用戶端ID和用戶端密碼是您在 [!DNL Bynder].

在中建立應用程式的指示 [!DNL Bynder]，請參閱 [Oauth 2.0應用程式](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) 在 [!DNL Bynder] 檔案。

>[!NOTE]
>
>在中建立應用程式時 [!DNL Bynder]，請輸入下列作為 `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] 模組及其欄位

設定時 [!DNL Bynder] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Bynder] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)
* [觸發器](#triggers)

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 讀取資產中繼資料]](#read-asset-metadata)
* [[!UICONTROL 更新資產中繼資料]](#update-asset-metadata)
* [[!UICONTROL 新增資產至集合]](#add-assets-to-a-collection)
* [[!UICONTROL 從集合中移除資產]](#remove-assets-from-collection)
* [[!UICONTROL 新增標籤至資產]](#add-a-tag-to-assets)
* [[!UICONTROL 移除標籤] 從資產](#remove-a-tag-from-assets)
* [[!UICONTROL 下載資產]](#download-asset)
* [[!UICONTROL 上傳資產]](#upload-asset)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Bynder] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Bynder] 模組。

設定此模組時，會顯示下列欄位。

模組會傳回狀態代碼，以及API呼叫的標題和內文。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>輸入相對於的路徑 <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
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
 </tbody> 
</table>

#### [!UICONTROL 讀取資產中繼資料]

此動作模組會讀取資產的中繼資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td>輸入或對應您要擷取中繼資料之資產的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新資產中繼資料]

此動作模組會更新現有資產的中繼資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td>輸入或對應您要更新中繼資料的資產ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位]</td> 
   <td> <p>選擇要輸入資訊的欄位，然後輸入或將要更新元資料的資訊映射到這些欄位。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL元屬性]</p> </td> 
   <td>選擇要更新的選項，然後輸入或將資訊映射到這些屬性。 元屬性是不代表資產中特定欄位的資產相關資訊。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增資產至集合]

此動作模組會新增一或多個資產至集合。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL集合ID]</td> 
   <td> <p>輸入或對應您要新增資產之集合的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>針對您要新增至集合的每個資產，按一下 <strong>[!UICONTROL添加項]</strong>，然後輸入或對應資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從集合中移除資產]

此動作模組會從集合中移除一或多個資產。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL集合ID]</td> 
   <td> <p>輸入或對應您要移除資產之集合的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>針對您要從集合中移除的每個資產，按一下 <strong>[!UICONTROL添加項]</strong>，然後輸入或對應資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增標籤至資產]

新增標籤至一或多個資產

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤ID]</td> 
   <td> <p>輸入或對應您要新增至資產之標籤的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>針對您要標籤的每個資產，按一下 <strong>[!UICONTROL添加項]</strong>，然後輸入或對應資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從資產中移除標籤]

從一或多個資產中移除標籤

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤ID]</td> 
   <td> <p>輸入或對應您要從資產中移除的標籤ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>針對您要移除標籤的每個資產，按一下 <strong>[!UICONTROL添加項]</strong>，然後輸入或對應資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載資產]

此動作模組會下載單一資產。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td>輸入或對應您要下載的資產ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產版本]</td> 
   <td> <p>輸入或對應您要下載的資產版本。 若要下載最新版資產，請將欄位留空。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳資產]

此動作模組會上傳單一資產。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL另存為]</td> 
   <td> <p>選取您要如何儲存要上傳的檔案。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL新資產]</strong> </p> <p>選擇要輸入資訊的欄位和元屬性，然後在這些欄位中輸入資訊。</p> <p>輸入或對應您要用於已上傳資產的品牌ID。</p> </li> 
     <li> <p><strong>[!UICONTROL新資產版本]</strong> </p> <p>輸入您要上傳新版本的資產ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 清單記錄]](#list-record)
* [[!UICONTROL 搜尋資產]](#search-for-assets)

#### [!UICONTROL 清單記錄]

此搜尋模組會擷取特定類型的所有項目。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要列出的記錄類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL讀取所有集合]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL讀取有關所有標籤的資訊]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL讀取集合的所有資產]</strong> </p> <p>輸入或對應您要列出資產之集合的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期期間傳回的資產數量上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋資產]

此搜尋模組會根據您提供的條件來搜尋資產。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL條件]</td> 
   <td> <p>輸入搜索標準。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL欄位]</strong> </p> <p>選取您要在搜尋中使用的欄位</p> </li> 
     <li> <p><strong>[!UICONTROL邏輯運算子]</strong> </p> <p>選取您要在搜尋中使用的運算子。</p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>輸入或映射要在選定欄位中查找的值。 值類型應與所選欄位的資料類型相同。 </p> <p>如需資料類型的詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">中的項目資料類型 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結果集]</td> 
   <td>選取您要傳回第一個相符資產還是所有相符資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依據]</td> 
   <td> <p>選取要排序的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序方向]</td> 
   <td> <p>選取您要遞增排序或遞減排序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期期間傳回的資產數量上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 觸發器

#### [!UICONTROL 監看資產]

此觸發器模組會在資產建立或更新時啟動案例。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Bynder] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL集合]</td>
   <td> <p>選取您要監看新資產的集合。 若要監看所有集合，請將此欄位留空。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL限制]</td>

<td> <p>輸入在每個方案執行週期中希望模組返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>
