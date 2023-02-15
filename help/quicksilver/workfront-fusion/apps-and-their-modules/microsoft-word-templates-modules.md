---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft Word範本模組
description: 在Adobe Workfront Fusion案例中，您可以自動執行使用Microsoft Word範本的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 0%

---


# [!DNL Microsoft Word Template] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Microsoft Word Templates]，並將其連接至多個協力廠商應用程式和服務。

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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

為了使用 [!DNL Miscrosoft Word Templates] with [!DNL Adobe Workfront Fusion]，則必須有 [!DNL Office 365] 帳戶。 您可以在www.office.com建立一個。

## 使用 [!DNL Microsoft Word Templates] 模組

您可以使用 [!DNL Microsoft Word Template] 從多個Web服務將資料合併到 [!DNL Microsoft Word] 檔案。

例如，您可以使用 [!DNL Microsoft Word] 範本：

![](assets/word-template-before-filled-350x62.png)

要建立此文檔，請執行以下操作：

![](assets/word-template-exampled-filled-350x85.png)

## 關於值標籤

A [!DNL Microsoft Word] 範本是一般 [!DNL Microsoft Word] 檔案（.docx檔案）的文字中加上特殊標籤，可決定合併或填入資料的位置和方式。 標籤有三種類型：

* [簡單值標籤](#simple-value-tag)
* [條件標籤](#condition-tag)
* [循環標籤](#loop-tag)

### 簡單值標籤 {#simple-value-tag}

簡單值標籤會直接取代為對應的值。 標籤的名稱與 [!UICONTROL 金鑰] 欄位的值，此值會放置在雙大括弧內；例如，


<pre>&#123;&#123;name&#125;&#125;</pre>


。

**範例：** 若要建立說「你好，Petr！」的檔案，您可以使用 [!DNL Microsoft Word Template] 模組來建立下列範本：

<pre>&gt;嗨&#123;&#123;name&#125;&#125;!</pre>

若要這麼做，請依下列方式設定模組：

![](assets/word-template-simple-value-350x286.png)

### 條件標籤 {#condition-tag}

您可以使用條件標籤來繞排應僅在符合特定條件時才呈現的文字。 若要繞排文字，請將其置於開啟和關閉條件標籤之間，例如「hasPhone」（如果條件是資料是否包含電話號碼）。 左標籤的名稱會以雜湊符號#為前置詞，右標籤的名稱會以斜線/為前置詞，如下列範例所示。

**範例：** 若要在輸入資料包含電話號碼但沒有電子郵件地址時生成包含客戶電話號碼的文檔，您可以使用 [!DNL Microsoft Word Template] 模組並建立下列範本：
<pre>> &#123;&#123;#hasPhone&#125;&#125;電話：&#123;&#123;phone&#125;&#125; &#123;&#123;/hasPhone&#125;&#125;</pre><pre>> &#123;&#123;#hasEmail&#125;&#125;電子郵件：&#123;&#123;email&#125;&#125; &#123;&#123;/hasEmail&#125;&#125;</pre>若要這麼做，請依下列方式設定模組：

![](assets/word-template-conditional-350x501.png)

在文檔中，電話號碼將顯示如下：
<pre>&gt;電話：4445551234</pre>

### 循環標籤 {#loop-tag}

您可以使用循環標籤（也稱為區段標籤）來重複文字的區段。 將文字放在開頭和結尾回圈標籤之間，以繞排文字。 開頭標籤的名稱會加上雜湊符號#;結尾標籤的名稱會以斜線/加上前置詞。

* [使用填寫檔案模組循環標籤](#loop-tag-with-fill-out-a-document-module)

<!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### 使用填寫檔案模組循環標籤 {#loop-tag-with-fill-out-a-document-module}

**範例：** 要生成列出客戶清單中每個聯繫人的姓名和電話號碼的文檔，可以使用 [!DNL Microsoft Word Template] 模組並建立下列範本：

<pre>> &#123;&#123;#contact&#125;&#125;</pre><pre>> &#123;&#123;name&#125;&#125;, &#123;&#123;phone&#125;&#125;</pre><pre>> &#123;&#123;/contact&#125;&#125;</pre>

若要這麼做，請依下列方式設定模組：


![](assets/word-template-fill-out-a-document-350x732.png)

該模組將建立以下文檔：

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] 模組

這些模組不需要連接。

* [填寫文檔](#fill-out-a-document)
* [用一批資料填寫文檔](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL 填寫文檔] {#fill-out-a-document}

此變壓器模組可讓您用您指定的資料填入檔案。 它可與簡單值標籤、條件標籤或回圈標籤搭配使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL要替換的文本的開始分隔符]</td> 
   <td> <p>輸入要標籤要替換的文本的開頭的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>輸入 <code>[[</code> 如果要替換類似於此文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL要替換的文本的結束分隔符]</p> </td> 
   <td> <p>輸入要標籤要替換的文本結尾的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>輸入 <code>]]</code> 如果要替換類似於此文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p> 對應您要從上一個模組上傳的檔案(例如，「HTTP &gt;取得檔案」或「Dropbox&gt;取得檔案模組」)。 或手動輸入資料檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL已填寫檔案的名稱]</td> 
   <td>輸入目標輸出檔案的檔案名（包括副檔名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料源]</td> 
   <td> <p>選取選項，以指出您使用的資料來自表單或原始資料收集（未處理的電腦資料）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td> <p>這必須是集合的陣列，其中：</p> 
    <ul> 
     <li>每個集合都對應至一個資料項目，並包含一個項目 <code>entry</code></li> 
     <li>項目 <code>entry </code>包含 <code>key </code>和 <code>value</code></li> 
     <li>項目 <code>key </code>包含標籤的名稱</li> 
     <li>項目 <code>value </code>包含標籤的值</li> 
    </ul> 
    <p>要添加條目：</p>
    <ol> 
     <li> 按一下 <b>[!UICONTROL添加項]</b>. </li> 
     <li>選擇條目的值類型。</li> 
     <li>新增名稱和值。 如需詳細資訊，請參閱本文中所選值類型的範例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">簡單值標籤</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">條件標籤</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">循環標籤</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 用一批資料填寫文檔] {#fill-a-document-with-a-batch-of-data}

如果您的資料項目是個別的套件組合，此匯總模組就十分實用。 使用此模組，您可以輕鬆設定「值」欄位所需的結構，並將項目對應至每個值項目。 與「填寫文檔」模組不同，「用批資料模組填寫文檔」中的「值」欄位僅允許包含變數的單個條目。

如果您的資料項目以陣列形式出現，也可以使用此模組，方法是使用 *迭代器* 模組，將陣列的內容轉換為一系列套件組合。

系統會為每個傳入套件建立並填入實際值。 處理所有輸入包後，將生成模板。

此匯總模組對於建立清單或報表特別有用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組]</td> 
   <td>選取文字來源的模組。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要替換的文本的開始分隔符]</td> 
   <td> <p>輸入要標籤要替換的文本的開頭的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>輸入 <code>[[</code> 如果要替換類似於此文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL要替換的文本的結束分隔符]</p> </td> 
   <td> <p>輸入要標籤要替換的文本結尾的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>輸入 <code>]]</code> 如果要替換類似於此文本： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL組依據]</td> 
   <td> 定義包含一或多個已對應項目的運算式。 匯總的資料在具有相同運算式值的「群組」下分隔。 每個組輸出為一個單獨的包，包含一個鍵，其中包含已評估的表達式和聚合文本。 執行此操作後，您就可以在後續模組中使用索引鍵作為篩選器。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL在空聚合後停止處理]</td> 
   <td>啟用此選項可在匯總不含套件時停止處理。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p> 對應您要從上一個模組上傳的檔案(例如，「HTTP &gt;取得檔案」或「Dropbox&gt;取得檔案模組」)。 或手動輸入資料檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL已填寫檔案的名稱]</td> 
   <td>輸入目標輸出檔案的檔案名（包括副檔名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料源]</td> 
   <td> <p>選取選項，以指出您使用的資料來自表單或原始資料收集（未處理的電腦資料）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td> <p>這必須是集合的陣列，其中：</p> 
    <ul> 
     <li>每個集合都對應至一個資料項目，並包含一個項目 <code>entry</code></li> 
     <li>項目 <code>entry </code>包含 <code>key </code>和 <code>value</code></li> 
     <li>項目 <code>key </code>包含標籤的名稱</li> 
     <li>項目 <code>value </code>包含標籤的值</li> 
    </ul> 
    <p>要添加條目：</p>
    <ol> 
     <li> 按一下 <b>[!UICONTROL添加項]</b>. </li> 
     <li>選擇條目的值類型。</li> 
     <li>新增名稱和值。 如需詳細資訊，請參閱本文中所選值類型的範例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">簡單值標籤</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">條件標籤</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">循環標籤</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

