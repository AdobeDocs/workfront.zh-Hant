---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 旁觀器模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用 [!DNL Bynder]的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1661'
ht-degree: 0%

---

# [!DNL Bynder]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Bynder]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL Bynder]模組，您必須有[!DNL Bynder]帳戶。

## 將[!DNL Bynder]連線至Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [從 [!DNL Workfront Fusion]建立與 [!DNL Bynder] 的連線](#create-a-connection-to-bynder-from-workfront-fusion)
* [在 [!DNL Bynder] 中產生[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼] （選擇性）](#generate-a-client-id-and-client-secret-in-bynder-optional)

### 從[!DNL Workfront Fusion]建立與[!DNL Bynder]的連線

您可以從[!DNL Bynder]模組內直接建立從[!DNL Workfront Fusion]到您[!DNL Bynder]帳戶的連線。

1. 在任何[!DNL Bynder]模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 選取您要連線的[!DNL Bynder]網域。
1. （選擇性）按一下&#x200B;**[!UICONTROL 進階設定]**，然後輸入您的[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼]。

   如需有關產生使用者端ID和使用者端密碼的指示，請參閱本文中的[在 [!DNL Bynder] （選擇性）](#generate-a-client-id-and-client-secret-in-bynder-optional)中產生使用者端ID和使用者端密碼。

1. 在[!UICONTROL 登入]視窗中輸入您的使用者名稱（電子郵件地址）和密碼。
1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

### 在[!DNL Bynder]中產生[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼] （選擇性）

如果您要使用使用者端ID和使用者端密碼建立連線，可以從您的[!DNL Bynder]帳戶產生連線。 當您在[!DNL Bynder]中建立應用程式時，會產生使用者端識別碼和使用者端密碼。

如需在[!DNL Bynder]中建立應用程式的指示，請參閱[!DNL Bynder]檔案中的[Oauth 2.0應用程式](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/)。

>[!NOTE]
>
>在[!DNL Bynder]中建立應用程式時，請輸入下列專案作為`redirect uri`：
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder]模組及其欄位

當您設定[!DNL Bynder]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Bynder]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)
* [觸發器](#triggers)

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 讀取資產中繼資料]](#read-asset-metadata)
* [[!UICONTROL 更新資產中繼資料]](#update-asset-metadata)
* [[!UICONTROL 將資產新增至集合]](#add-assets-to-a-collection)
* [[!UICONTROL 從集合]移除資產](#remove-assets-from-collection)
* [[!UICONTROL 新增標籤至資產]](#add-a-tag-to-assets)
* [[!UICONTROL 從資產移除標籤]](#remove-a-tag-from-assets)
* [[!UICONTROL 下載資產]](#download-asset)
* [[!UICONTROL 上傳資產]](#upload-asset)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對[!DNL Bynder] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL Bynder]模組無法完成的資料流程自動化。

當您設定此模組時，會顯示下列欄位。

模組會傳回狀態代碼，以及API呼叫的標題和正文。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>輸入相對於<code>https://{your-bynder-domain}/api/{api-version}/</code>的路徑。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td>輸入或對應您要更新中繼資料的資產ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位]</td> 
   <td> <p>選取您要輸入資訊的欄位，然後輸入或對應您要使用更新中繼資料的資訊，到這些欄位中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Metaproperties]</p> </td> 
   <td>選取您要更新的選項，然後輸入資訊或將資訊對應至這些屬性。 中繼屬性是不代表資產中特定欄位的資產相關資訊。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將資產新增至集合]

此動作模組新增一或多個資產至收藏集。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL集合ID]</td> 
   <td> <p>輸入或對應您要新增資產的集合ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您想要新增至集合的每個資產，按一下<strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從集合]移除資產

此動作模組會從集合中移除一或多個資產。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL集合ID]</td> 
   <td> <p>輸入或對映您要移除資產之集合的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您要從集合中移除的每個資產，按一下<strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤ID]</td> 
   <td> <p>輸入或對應您要新增至資產的標籤ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您要標籤的每個資產，按一下<strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從資產移除標籤]

從一個或多個資產中移除標籤

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤ID]</td> 
   <td> <p>輸入或對應您要從資產移除之標籤的ID。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您要移除標籤的每個資產，按一下<strong>[！UICONTROL新增專案]</strong>，然後輸入或對應資產ID。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td>輸入或對應您要下載的資產識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產版本]</td> 
   <td> <p>輸入或對映您要下載的資產版本。 若要下載最新版本的資產，請將此欄位留空。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL另存新檔]</td> 
   <td> <p>選取要如何儲存上傳的檔案。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL新資產]</strong> </p> <p>選取您要輸入資訊的欄位和中繼屬性，然後在這些欄位中輸入資訊。</p> <p>輸入或對應您要用於上傳資產的品牌ID。</p> </li> 
     <li> <p><strong>[！UICONTROL新資產版本]</strong> </p> <p>輸入您要上傳新版本之資產的識別碼。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source檔案]</td> 
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
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
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
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的資產最大數量。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL條件]</td> 
   <td> <p>輸入搜尋條件。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL欄位]</strong> </p> <p>選取您要在搜尋中使用的欄位</p> </li> 
     <li> <p><strong>[！UICONTROL邏輯運運算元]</strong> </p> <p>選取要在搜尋中使用的運運算元。</p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>在選取的欄位中輸入或對應要尋找的值。 值型別應與所選欄位的資料型別相同。 </p> <p>如需資料型別的詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">專案資料型別。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結果集]</td> 
   <td>選取您要傳回第一個相符的資產，還是所有相符的資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序依據]</td> 
   <td> <p>選取您要排序的欄位。</p> </td> 
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
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的資產最大數量。</p> </td> 
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
    <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Bynder]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">將[!DNL Bynder]連線到[!DNL Workfront Fusion] </a>。</p> </td> 
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

<td> <p>輸入您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>
