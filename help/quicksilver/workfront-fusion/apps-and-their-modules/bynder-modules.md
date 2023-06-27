---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Bynder模組
description: 在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Bynder]，以及將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1664'
ht-degree: 0%

---

# [!DNL Bynder] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Bynder]，以及將其連線到多個協力廠商應用程式和服務。

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

使用 [!DNL Bynder] 模組，您必須擁有 [!DNL Bynder] 帳戶。

## Connect [!DNL Bynder] 至Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [建立與的連線 [!DNL Bynder] 從 [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [產生 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼] 在 [!DNL Bynder] （可選）](#generate-a-client-id-and-client-secret-in-bynder-optional)

### 建立與的連線 [!DNL Bynder] 從 [!DNL Workfront Fusion]

您可以從以下位置建立連線： [!DNL Workfront Fusion] 至您的 [!DNL Bynder] 直接從a內的帳戶 [!DNL Bynder] 模組。

1. 在任何 [!DNL Bynder] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選取 [!DNL Bynder] 您要連線的網域。
1. （可選）按一下 **[!UICONTROL 進階設定]**，然後輸入您的 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼].

   如需產生使用者端ID和使用者端密碼的說明，請參閱 [在中產生使用者端ID和使用者端密碼 [!DNL Bynder] （可選）](#generate-a-client-id-and-client-secret-in-bynder-optional) 本文章內容。

1. 在 [!UICONTROL 登入] 視窗，輸入您的使用者名稱（電子郵件地址）和密碼。
1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

### 產生 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼] 在 [!DNL Bynder] （可選）

如果您想要使用使用者端ID和使用者端密碼建立連線，您可以從產生 [!DNL Bynder] 帳戶。 使用者端ID和使用者端密碼會在您建立應用程式時產生，位置如下： [!DNL Bynder].

如需在中建立應用程式的指示 [!DNL Bynder]，請參閱 [Oauth 2.0應用程式](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) 在 [!DNL Bynder] 說明檔案。

>[!NOTE]
>
>在中建立應用程式時 [!DNL Bynder]，請輸入下列專案作為 `redirect uri`：
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] 模組及其欄位

當您設定 [!DNL Bynder] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Bynder] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)
* [觸發器](#triggers)

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 讀取資產中繼資料]](#read-asset-metadata)
* [[!UICONTROL 更新資產中繼資料]](#update-asset-metadata)
* [[!UICONTROL 將資產新增至集合]](#add-assets-to-a-collection)
* [[!UICONTROL 從集合中移除資產]](#remove-assets-from-collection)
* [[!UICONTROL 新增標籤至資產]](#add-a-tag-to-assets)
* [[!UICONTROL 移除標籤] 從資產](#remove-a-tag-from-assets)
* [[!UICONTROL 下載資產]](#download-asset)
* [[!UICONTROL 上傳資產]](#upload-asset)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Bynder] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Bynder] 模組。

當您設定此模組時，會顯示下列欄位。

模組會傳回狀態代碼，以及API呼叫的標題和正文。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>輸入相對於 <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
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
 </tbody> 
</table>

#### [!UICONTROL 讀取資產中繼資料]

此動作模組會讀取資產的中繼資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td>輸入或對應您要擷取中繼資料的資產ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td>輸入或對應您要更新中繼資料的資產ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位]</td> 
   <td> <p>選取您要輸入資訊的欄位，然後輸入或對應您要更新中繼資料的資訊到這些欄位。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Metaproperties]</p> </td> 
   <td>選取您要更新的選項，然後輸入資訊或將資訊對應至這些屬性。 中繼屬性是不代表資產中特定欄位的資產相關資訊。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將資產新增至集合]

此動作模組會新增一或多個資產至集合。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL集合ID]</td> 
   <td> <p>輸入或對映您要新增資產的集合ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您想要新增至集合的每個資產，按一下 <strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL集合ID]</td> 
   <td> <p>輸入或對映您要移除資產之集合的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您要從集合中移除的每個資產，按一下 <strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤ID]</td> 
   <td> <p>輸入或對應您要新增至資產的標籤ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您要標籤的每個資產，按一下 <strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從資產中移除標籤]

從一個或多個資產中移除標籤

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤ID]</td> 
   <td> <p>輸入或對應您要從資產移除之標籤的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您想要從中移除標籤的每個資產，按一下 <strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td>輸入或對應您要下載的資產的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產版本]</td> 
   <td> <p>輸入或對映您要下載的資產版本。 若要下載資產的最新版本，請將此欄位留空。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL另存新檔]</td> 
   <td> <p>選取要如何儲存上傳的檔案。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL新資產]</strong> </p> <p>選取您要輸入資訊的欄位和中繼屬性，然後在這些欄位中輸入資訊。</p> <p>輸入或對應您要用於上傳資產的品牌ID。</p> </li> 
     <li> <p><strong>[！UICONTROL新資產版本]</strong> </p> <p>輸入您要上傳新版本之資產的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL來源檔案]</td> 
   <td>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 清單記錄]](#list-record)
* [[!UICONTROL 搜尋資產]](#search-for-assets)

#### [!UICONTROL 清單記錄]

此搜尋模組會擷取特定型別的所有專案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要列出的記錄型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL讀取所有集合]</strong> </p> </li> 
     <li> <p><strong>[！UICONTROL讀取所有標籤的相關資訊]</strong> </p> </li> 
     <li> <p><strong>[！UICONTROL讀取集合的所有資產]</strong> </p> <p>輸入或對應您要列出其資產的集合ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的資產數量上限。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL條件]</td> 
   <td> <p>輸入搜尋條件。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL欄位]</strong> </p> <p>選取您要用於搜尋的欄位</p> </li> 
     <li> <p><strong>[！UICONTROL邏輯運運算元]</strong> </p> <p>選取要在搜尋中使用的運運算元。</p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>在選取的欄位中輸入或對應要尋找的值。 值型別應與所選欄位的資料型別相同。 </p> <p>如需資料型別的詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">中的專案資料型別 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結果集]</td> 
   <td>選取您要傳回第一個相符的資產，還是所有相符的資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序依據]</td> 
   <td> <p>選取您要作為排序依據的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序方向]</td> 
   <td> <p>選取您要遞增排序還是遞減排序。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的資產數量上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 觸發器

#### [!UICONTROL 觀看資產]

建立或更新資產時，此觸發模組就會啟動案例。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Bynder] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Connect [!DNL Bynder] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[！UICONTROL集合]</td>
   <td> <p>選取您要觀看新資產的集合。 若要觀看所有集合，請將此欄位留空。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[！UICONTROL限制]</td>

<td> <p>輸入您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>
