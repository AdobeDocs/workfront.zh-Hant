---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: 可空氣模組
description: Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。
author: Becky
hidefromtoc: true
source-git-commit: 6955c979d504adb6514ae64bf5108174d7a90ce4
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 2%

---


# 可空氣模組


使用 [!DNL Airtable] 連接器 [!DNL Adobe Workfront Fusion]，您可以根據 [!DNL Airtable] 帳戶、建立、上傳和更新記錄、搜尋記錄，以及對Airtable API進行自訂API呼叫。

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

您必須有Airtable帳戶才能使用本文中的功能。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## 將Airtable連接到Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. 開啟Workfront Fusion與 **建立連線** 對話方塊。
1. 輸入連線的名稱。
1. （可選）按一下「顯示高級設定」 ，然後輸入「Airtable Client ID」和「Client Secret」。
1. 按一下 **繼續** 按鈕，建立連線並返回模組。

## 可空中模組及其欄位

### 記錄

* [建立記錄](#create-a-record)
* [刪除記錄](#delete-a-record)
* [獲取記錄](#get-a-record)
* [搜索記錄](#search-records)
* [更新記錄](#update-a-record)
* [更新記錄](#upsert-a-record)
* [監看記錄](#watch-records)
* [監看回應](#watch-responses)
* [進行API呼叫](#make-an-api-call)

#### 建立記錄 {#create-a-record}

此動作模組會建立新記錄。

您可以在記錄中指定想要的資料，以及要將其儲存的位置。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選擇新記錄將屬於的基礎。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選擇新記錄將屬於的表。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>記錄</p> </td> 
   <td> <p>輸入新記錄的值。 可用欄位是根據您選取的表格而定。</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
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
   <td>智慧連結</td> 
   <td> <p>啟用此選項，可在連結至其他表格的欄位中輸入名稱，而非記錄ID。 如果沒有匹配項，則在連結的表中自動建立記錄。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 刪除記錄 {#delete-a-record}

此動作模組會刪除特定記錄。

您可以指定記錄的ID和位置。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選擇包含要刪除的記錄的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選擇包含要刪除的記錄的表。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID</td> 
   <td> <p>輸入或映射您希望模組刪除的記錄的唯一可用ID。 例如，您可以使用「搜尋記錄」模組來擷取ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 獲取記錄 {#get-a-record}

此動作模組會擷取記錄詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選擇包含要檢索記錄的表的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表格</td> 
   <td> <p> 選擇包含要檢索詳細資訊的記錄的表。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID</td> 
   <td> <p> 輸入或映射要檢索詳細資訊的記錄的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 搜索記錄 {#search-records}

此搜索模組在Airtable中查找與您指定的搜索查詢匹配的對象中的記錄。

您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選擇要搜索記錄的基礎。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選擇要搜索記錄的表。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>公式</p> </td> 
   <td> <p>用於篩選記錄的公式。 系統會為每個記錄評估公式，如果結果不是 <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>，或 <code>#Error!</code> 該記錄會包含在回應中。</p> <p>若與 <code>view</code>，只會傳回該檢視中符合公式的記錄。</p> <p>例如，要僅包含名稱不為空的記錄，請傳入：<code> NOT({Name} = '')</code></p> <p>要了解更多資訊，請在Airtable支援文檔中搜索有關公式欄位引用的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td>排序 </td> 
   <td> <p>選擇排序方向和要按結果排序的欄位。</p> </td> 
  </tr> 
  <tr> 
   <td>檢視 </td> 
   <td> <p>選擇要搜索記錄的視圖。</p> </td> 
  </tr> 
  <tr> 
   <td>限制</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 更新記錄 {#update-a-record}

此動作模組會更新特定記錄。

您可指定記錄的ID以及要包含的新資料。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選擇包含要更新記錄的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選擇包含要更新記錄的表。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID </td> 
   <td> <p>輸入或映射要更新模組的記錄的唯一可用ID。 例如，您可以使用「搜尋記錄」模組來擷取ID。</p> </td> 
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
   <td>智慧連結</td> 
   <td> <p>輸入名稱，而不是記錄ID，以輸入連結至其他表格的欄位。 如果沒有匹配項，則在連結的表中自動建立記錄。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 更新記錄

此動作模組會更新或插入特定記錄。

您可指定記錄的ID以及要包含的新資料。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選擇包含要更新記錄的基。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選擇包含要更新記錄的表。</p> </td> 
  </tr> 
  <tr> 
   <td>記錄ID </td> 
   <td> <p>如果要更新記錄，請輸入或映射要模組更新的記錄的唯一可用ID。 例如，您可以使用「搜尋記錄」模組來擷取ID。</p> </td> 
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
   <td>智慧連結</td> 
   <td> <p>輸入名稱，而不是記錄ID，以輸入連結至其他表格的欄位。 如果沒有匹配項，則在連結的表中自動建立記錄。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 監看記錄 {#watch-records}

當在指定的表中建立或更新記錄時，此觸發模組會啟動方案。

>[!NOTE]
>
>若要使用此模組，必須在表中建立「建立時間」欄位或「上次修改時間」欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>連接 </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>根據 </td> 
   <td> <p>選擇要監視新記錄的基礎。</p> </td> 
  </tr> 
  <tr> 
   <td>表格 </td> 
   <td> <p>選擇要監視的新記錄的表。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>觸發設定</p> </td> 
   <td> <p>觸發欄位</p> <p>A <code>Created Time</code> 或 <code>Last Modified Time</code> 用於排序記錄的欄位。 如果您沒有 <code>Created Time</code> 或 <code>Last Modified Time</code> 欄位，則您需要建立。 </p> <p>標籤欄位</p> <p>用作記錄標籤的欄位，例如，在「選擇開始位置」對話框中。</p> </td> 
  </tr> 
  <tr> 
   <td>限制</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中監視的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>檢視</td> 
   <td> <p>選取您要使用的檢視。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>公式</p> </td> 
   <td> <p>用於篩選記錄的公式。 系統會為每個記錄評估公式，如果結果不是 <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>，或 <code>#Error!</code> 該記錄會包含在回應中。</p> <p>若與 <code>view</code>，只會傳回該檢視中符合公式的記錄。</p> <p>例如，要僅包含名稱不為空的記錄，請傳入：<code> NOT({Name} = '')</code></p> <p>要了解更多資訊，請參閱Airtable支援文檔中有關公式欄位引用的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 監看回應

此觸發器模組會在表單提交時啟動案例。

>[!NOTE]
>
>此功能僅適用於付費Airtable Pro計畫。

Webhook URL必須在Workfront Fusion中產生，然後新增至Airtable的表單設定。

1. 將Watch New Responses模組新增至您的Workfront Fusion案例。
1. 產生並複製網頁連結URL。

   如需指示，請參閱 [Adobe Workfront Fusion中的即時觸發器(Webhook)](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. 登入您的Airtable帳戶。
1. 開啟「基」(Base)和要用於表單的表，並建立「表單」視圖。
1. 視需要設定表單，向下捲動表單，並啟用提交表單後重新導向至URL選項。
1. 將步驟2中生成的Webhook URL輸入到顯示的對話框，並在Webhook URL後面添加？record_id={record_id}以在模組的輸出中包含Record ID，然後按一下「保存」。 例如，產生的URL看起來會像這樣：
1. 返回到您的Workfront Fusion方案，並執行Watch Responses模組，僅載入來自Airtable的欄位，並能夠將這些欄位映射至其他模組。
1. 在Airtable中提交表單，其中已啟用「提交表單後重新導向至URL」選項並新增Webhook URL（上述步驟6）。

   觸發監看回應模組，並載入所需資料。

1. 在「表」>「監看響應」模組後面添加「表」>「獲取記錄」模組，並將record_id映射到「記錄ID」欄位。

現在，每次提交表單時，都會觸發Workfront Fusion中的Watch Responses模組，而Get a Record模組會傳回已提交的表單詳細資訊。

#### 進行API呼叫

#### 自訂API呼叫

此動作模組可讓您對 [!DNL Airtable] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Airtable] 模組。

動作以您指定的實體類型（配置對象類型）為基礎。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>連接</p> </td> 
   <td> <p>有關將Airtable帳戶連接到Workfront Fusion的說明，請參見 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">將Airtable連接到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>輸入相對於的路徑 <code>https://api.airtable.com/}</code>. 範例: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">方法</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">標頭</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 為您添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">查詢字串</td> 
   <td> <p>以索引鍵和值的形式新增API呼叫的查詢</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">內文</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
