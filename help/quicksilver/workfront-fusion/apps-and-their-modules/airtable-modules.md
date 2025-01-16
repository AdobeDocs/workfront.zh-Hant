---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 可投放模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 1d78e0db-9a77-437d-a72f-88fb256981c0
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 1%

---

# 可投放模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [可空運模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/airtable-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。


使用[!DNL Adobe Workfront Fusion]的[!DNL Airtable]聯結器，您可以根據[!DNL Airtable]帳戶中的事件啟動案例、建立、上傳和更新記錄、搜尋記錄，以及對Airtable API進行自訂API呼叫。

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
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您的組織必須購買[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

您必須擁有Airtable帳戶才能使用本文中的功能。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Airtable API資訊

Airtable聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td>https://api.airtable.com/v0</td> 
  </tr>
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v3.3.28</td> 
  </tr>
 </tbody> 
 </table>

## 將Airtable連線至Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. 開啟Workfront Fusion並開啟所需模組的&#x200B;**建立連線**&#x200B;對話方塊。
1. 輸入連線的名稱。
1. （選用）按一下「顯示進階設定」 ，然後輸入您的Airtable使用者端ID和使用者端密碼。
1. 按一下&#x200B;**繼續**&#x200B;按鈕以建立連線並返回模組。

## 可座飛機模組及其欄位

### 記錄

* [建立記錄](#create-a-record)
* [刪除記錄](#delete-a-record)
* [取得記錄](#get-a-record)
* [搜尋記錄](#search-records)
* [更新記錄](#update-a-record)
* [更新插入記錄](#upsert-a-record)
* [觀看記錄](#watch-records)
* [觀看回應](#watch-responses)
* [進行API呼叫](#make-an-api-call)

#### 建立記錄 {#create-a-record}

此動作模組會建立新記錄。

您可以指定要在記錄中儲存的資料以及儲存位置。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選取新記錄將屬於的基底。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選取新記錄所屬的表格。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>記錄</p> </td> 
   <td> <p>輸入新記錄的值。 可用欄位取決於您選取的表格。</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>智慧型連結</td> 
   <td> <p>啟用此選項可輸入名稱，而不是將ID記錄到連結到其他表格的欄位。 如果沒有相符專案，系統會自動在連結的表格中建立記錄。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 刪除記錄 {#delete-a-record}

此動作模組會刪除特定記錄。

您可以指定記錄的ID和位置。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選取包含您要刪除之記錄的基底。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選取包含您要刪除之記錄的表格。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID</td> 
   <td> <p>輸入或對應您要模組刪除之記錄的唯一Airtable ID。 例如，您可以使用搜尋記錄模組來擷取ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 取得記錄 {#get-a-record}

此動作模組會擷取記錄詳細資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選取包含您要擷取記錄的表格的基底。</p> </td> 
  </tr> 
  <tr> 
   <td>表格</td> 
   <td> <p> 選取包含您要擷取其詳細資訊之記錄的表格。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID</td> 
   <td> <p> 輸入或對應您要擷取其詳細資訊的記錄ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 搜尋記錄 {#search-records}

此搜尋模組會在Airtable中尋找符合您指定之搜尋查詢的物件記錄。

您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選取您要搜尋記錄的基底。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選取您要搜尋記錄的表格。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>公式</p> </td> 
   <td> <p>用來篩選記錄的公式。 已針對每個記錄評估公式，如果結果不是<code>0</code>、<code>false</code>、<code>""</code>、<code>NaN</code>、<code>[]</code>或<code>#Error!</code>，則記錄會包含在回應中。</p> <p>如果與<code>view</code>結合，則只會傳回該檢視中滿足公式的記錄。</p> <p>例如，若要僅包含Name非空白的記錄，請傳入：<code> NOT({Name} = '')</code></p> <p>若要深入瞭解，請在Airtable支援檔案中搜尋有關公式欄位參考的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td>排序 </td> 
   <td> <p>選取排序方向以及要作為結果排序依據的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>檢視 </td> 
   <td> <p>選取您要搜尋記錄的檢視表。</p> </td> 
  </tr> 
  <tr> 
   <td>限制</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 更新記錄 {#update-a-record}

此動作模組會更新特定記錄。

您可以指定記錄的ID，以及要包含的新資料。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選取包含要更新之記錄的基底。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選取包含要更新的記錄的表格。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID </td> 
   <td> <p>輸入或對應您要模組更新的記錄的唯一Airtable ID。 例如，您可以使用搜尋記錄模組來擷取ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>記錄</p> </td> 
   <td> <p>輸入新記錄的值。 可用欄位取決於您選取的表格。</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>智慧型連結</td> 
   <td> <p>輸入連結至其他表格的欄位名稱，而非記錄ID。 如果沒有相符專案，系統會自動在連結的表格中建立記錄。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 更新插入記錄

此動作模組會更新或插入特定記錄。

您可以指定記錄的ID，以及要包含的新資料。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選取包含要更新之記錄的基底。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選取包含要更新的記錄的表格。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID </td> 
   <td> <p>如果您要更新記錄，請輸入或對應您要模組更新的記錄的唯一Airtable ID。 例如，您可以使用搜尋記錄模組來擷取ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>記錄</p> </td> 
   <td> <p>輸入新記錄的值。 可用欄位取決於您選取的表格。</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>智慧型連結</td> 
   <td> <p>輸入連結至其他表格的欄位名稱，而非記錄ID。 如果沒有相符專案，系統會自動在連結的表格中建立記錄。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 觀看記錄 {#watch-records}

此觸發模組會在指定表格中建立或更新記錄時啟動案例。

>[!NOTE]
>
>若要使用此模組，必須在表格中建立「建立時間」欄位或「上次修改時間」欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選取要監視新記錄的基底。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選取要監視新記錄的表格。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>觸發器設定</p> </td> 
   <td> <p>觸發器欄位</p> <p>用來排序記錄的<code>Created Time</code>或<code>Last Modified Time</code>欄位。 如果您的結構描述中沒有<code>Created Time</code>或<code>Last Modified Time</code>欄位，則需要建立一個。 </p> <p>標籤欄位</p> <p>用作記錄標籤的欄位，例如，在選擇開始位置對話方塊中。</p> </td> 
  </tr> 
  <tr> 
   <td>限制</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中監視的最大記錄數量。</p> </td> 
  </tr> 
  <tr> 
   <td>檢視</td> 
   <td> <p>選取您要使用的檢視。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>公式</p> </td> 
   <td> <p>用來篩選記錄的公式。 已針對每個記錄評估公式，如果結果不是<code>0</code>、<code>false</code>、<code>""</code>、<code>NaN</code>、<code>[]</code>或<code>#Error!</code>，則記錄會包含在回應中。</p> <p>如果與<code>view</code>結合，則只會傳回該檢視中滿足公式的記錄。</p> <p>例如，若要僅包含Name非空白的記錄，請傳入：<code> NOT({Name} = '')</code></p> <p>若要深入瞭解，請參閱Airtable支援檔案中有關公式欄位參考的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 觀看回應

此觸發模組會在表單提交時啟動案例。

>[!NOTE]
>
>此功能僅適用於付費的Airtable Pro Plan。

webhook URL需要在Workfront Fusion中產生，然後新增到Airtable中的表單設定。

1. 將「觀看新回應」模組新增至您的Workfront Fusion案例。
1. 產生並複製webhook URL。

   如需指示，請參閱Adobe Workfront Fusion](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)中的[即時觸發器(webhook)。

1. 登入您的Airtable帳戶。
1. 開啟「基底」和您要用於表單的表格，並建立「表單」檢視。
1. 視需要設定表單、向下捲動表單，並啟用提交表單後重新導向至URL選項。
1. 輸入在步驟2中產生的Webhook URL到顯示的對話方塊，並在webhook URL之後新增？record_id={record_id}，以將記錄ID加入模組輸出中，然後按一下「儲存」。 例如，產生的URL如下所示：
1. 返回Workfront Fusion案例並執行觀察回應模組，僅從Airtable載入欄位，並將這些欄位對應到其他模組。
1. 在Airtable中提交表單，其中在提交表單後重新導向至URL選項已啟用並新增Webhook URL （上述步驟6）。

   監看回應模組已觸發，且所需資料已載入。

1. 在Airtable >觀看回應模組之後新增「Airtable >取得記錄」模組，並將record_id對應至「記錄ID」欄位。

現在，每次提交表單時，都會觸發Workfront Fusion案例中的「觀看回應」模組，且「取得記錄」模組會傳回提交的表單詳細資料。

#### 進行API呼叫

#### 自訂API呼叫

此動作模組可讓您對[!DNL Airtable] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL Airtable]模組無法完成的資料流程自動化。

動作以您指定的圖元型別（Allocadia物件型別）為基礎。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>連接</p> </td> 
   <td> <p>如需有關將Airtable帳戶連線至Workfront Fusion的說明，請參閱本文中的<a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連線至Workfront Fusion</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>輸入相對於<code>https://api.airtable.com/}</code>的路徑。 範例： <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">方法</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">標頭</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">查詢字串</td> 
   <td> <p>以索引鍵和值的形式新增API呼叫的查詢</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">內文</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
