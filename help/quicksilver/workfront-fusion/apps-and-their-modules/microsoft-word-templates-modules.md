---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft Word範本模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 889b417c-04a9-4dbf-9a34-0dab65f11f03
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1436'
ht-degree: 0%

---

# [!DNL Microsoft Word Template]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [Microsoft Word範本模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-word-templates-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Microsoft Word Templates]的工作流程，並將其連線至多個協力廠商應用程式和服務。

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
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您的組織必須購買[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文所述的功能。</td> 
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

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要搭配[!DNL Adobe Workfront Fusion]使用[!DNL Miscrosoft Word Templates]，必須有[!DNL Office 365]帳戶。 您可以在www.office.com建立一個。



## 正在將[!DNL Office]服務連線到[!DNL Workfront Fusion]

如需有關將您的[!DNL Office]帳戶連線到[!UICONTROL Workfront Fusion]的指示，請參閱[建立與[!UICONTROL Adobe Workfront Fusion]的連線](../../workfront-fusion/connections/connect-to-fusion-general.md) — 基本指示

>[!NOTE]
>
>部分Microsoft應用程式使用相同的連線，而此連線會繫結至個別使用者許可權。 因此，在建立連線時，許可權同意畫面會顯示先前授與此使用者連線的所有許可權，以及目前應用程式所需的任何新許可權。
>
>例如，如果使用者擁有透過Excel聯結器授予的「讀取表格」許可權，然後在Outlook聯結器中建立連線以讀取電子郵件，則許可權同意畫面會顯示已授予的「讀取表格」許可權和新要求的「寫入電子郵件」許可權。

## 使用[!DNL Microsoft Word Templates]模組

您可以使用[!DNL Microsoft Word Template]模組將來自多個網站服務的資料合併到[!DNL Microsoft Word]檔案中。

例如，您可以使用此[!DNL Microsoft Word]範本：

![](assets/word-template-before-filled-350x62.png)

若要建立此檔案：

![](assets/word-template-exampled-filled-350x85.png)

## 關於值標籤

[!DNL Microsoft Word]範本是一般[!DNL Microsoft Word]檔案（.docx檔案），其文字中有特殊標籤，可決定合併或填入資料的位置和方式。 有三種型別的標籤：

* [簡單值標籤](#simple-value-tag)
* [條件標籤](#condition-tag)
* [回圈標籤](#loop-tag)

### 簡單值標籤 {#simple-value-tag}

簡單值標籤只會被對應的值取代。 標籤名稱對應至[!UICONTROL Key]欄位的值，此值放在雙大括弧內，例如`{{name}}`。

**範例：**&#x200B;若要建立顯示「嗨，Petr！」的檔案，您可以使用[!DNL Microsoft Word Template]模組來建立下列範本：

```
> Hi {{name}}!
```

若要這麼做，您需設定模組，如下所示：

![](assets/word-template-simple-value-350x286.png)

### 條件標籤 {#condition-tag}

您可以使用條件標籤來繞排文字，這些文字只有在符合某些條件時才應呈現。 若要繞排文字，請將其置於開始和結束條件標籤之間，例如「hasPhone」（如果條件為資料是否包含電話號碼）。 開始標簽名稱會加上雜湊符號#，而結束標簽名稱會加上斜線/ ，如下列範例所示。

**範例：**&#x200B;若要在輸入資料包含電話號碼但沒有電子郵件地址時產生包含客戶電話號碼的檔案，您可以使用[!DNL Microsoft Word Template]模組並建立下列範本：

```
> {{#hasPhone}}Phone: {{phone}} {{/hasPhone}}
> {{#hasEmail}}Email: {{email}} {{/hasEmail}}
```

若要這麼做，您需設定模組，如下所示：

![](assets/word-template-conditional-350x501.png)

在檔案中，電話號碼會顯示如下：

```
> Phone: 4445551234
```

### 回圈標籤 {#loop-tag}

您可以使用回圈標籤（也稱為節標籤）來重複文字的節。 將文字置於開啟和關閉回圈標籤之間，以繞排文字。 開始標簽名稱會加上雜湊符號#；結束標簽名稱會加上斜線/。

* [Loop標籤，填滿檔案模組](#loop-tag-with-fill-out-a-document-module)
  <!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### 使用「填寫檔案模組」的回圈標籤 {#loop-tag-with-fill-out-a-document-module}

**範例：**&#x200B;若要產生列出客戶清單中每個連絡人姓名和電話號碼的檔案，您可以使用[!DNL Microsoft Word Template]模組並建立下列範本：

```
> {{#contact}}
>     {{name}}, {{phone}}
> {{/contact}}
```

若要這麼做，您需設定模組，如下所示：


![](assets/word-template-fill-out-a-document-350x732.png)

此模組將建立以下檔案：

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

## [!DNL Microsoft Word Template]模組

這些模組不需要連線。

* [填寫檔案](#fill-out-a-document)
* [以批次資料填入檔案](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL 填寫檔案] {#fill-out-a-document}

此轉換器模組可讓您使用您指定的資料填入檔案。 它可與簡單值標籤、條件標籤或回圈標籤搭配使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL要取代之文字的開始分隔符號]</td> 
   <td> <p>輸入要標示取代文字開頭的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您要取代類似下列的文字，請輸入<code>[[</code>： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要取代之文字的結尾分隔符號]</p> </td> 
   <td> <p>輸入要標示取代文字結尾的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您要取代類似下列的文字，請輸入<code>]]</code>： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source檔案]</td> 
   <td> <p> 對應您要從上一個模組上傳的檔案(例如，「HTTP &gt;取得檔案」或「Dropbox&gt;取得檔案模組」)。 或手動輸入資料檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">已填寫檔案的[！UICONTROL名稱]</td> 
   <td>輸入目標輸出檔案的檔案名稱（包括副檔名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料來源]</td> 
   <td> <p>選取選項以指出您使用的資料來自表單還是原始資料集合（未處理的電腦資料）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td> <p>這必須是集合陣列，其中：</p> 
    <ul> 
     <li>每個集合都對應一個資料專案，並包含一個專案 <code>entry</code></li> 
     <li>專案<code>entry </code>包含<code>key </code>的集合，並且 <code>value</code></li> 
     <li>專案<code>key </code>包含標籤的名稱</li> 
     <li>專案<code>value </code>包含標籤的值</li> 
    </ul> 
    <p>若要新增專案：</p>
    <ol> 
     <li> 按一下<b>[！UICONTROL新增專案]</b>。 </li> 
     <li>選取專案的值型別。</li> 
     <li>新增名稱和值。 如需詳細資訊，請參閱本文所選值型別的範例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">簡單值標籤</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">條件標籤</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">回圈標籤</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 以批次資料填入檔案] {#fill-a-document-with-a-batch-of-data}

如果您的資料專案為個別的組合，此彙總模組相當實用。 使用此模組，您可以輕鬆設定值欄位所需的結構，並將專案對應至每個值專案。 相較於填寫檔案模組，使用資料模組批次填寫檔案中的值欄位僅允許包含變數的單一專案。

如果您的資料專案為陣列，您也可以使用此模組，方法是使用&#x200B;*疊代器*&#x200B;模組將陣列的內容轉換為一系列組合。

系統會為每個傳入的套件組合建立並填入實際值。 範本會在處理所有輸入組合後產生。

此彙總模組對於建立清單或報告特別實用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組]</td> 
   <td>選取作為文字來源的模組。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要取代之文字的開始分隔符號]</td> 
   <td> <p>輸入要標示取代文字開頭的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您要取代類似下列的文字，請輸入<code>[[</code>： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要取代之文字的結尾分隔符號]</p> </td> 
   <td> <p>輸入要標示取代文字結尾的字元。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您要取代類似下列的文字，請輸入<code>]]</code>： <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Group by]</td> 
   <td> 定義包含一或多個對應專案的運算式。 彙總資料會以相同運算式的值分隔在「群組」底下。 每個群組都會輸出為個別的組合，其中包含含運算式和彙總文字的索引鍵。 如此一來，您便可將索引鍵用作後續模組中的篩選條件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL在空白彙總後停止處理]</td> 
   <td>啟用此選項可在彙總不含任何組合時停止處理。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source檔案]</td> 
   <td> <p> 對應您要從上一個模組上傳的檔案(例如，「HTTP &gt;取得檔案」或「Dropbox&gt;取得檔案模組」)。 或手動輸入資料檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">已填寫檔案的[！UICONTROL名稱]</td> 
   <td>輸入目標輸出檔案的檔案名稱（包括副檔名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料來源]</td> 
   <td> <p>選取選項以指出您使用的資料來自表單還是原始資料集合（未處理的電腦資料）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td> <p>這必須是集合陣列，其中：</p> 
    <ul> 
     <li>每個集合都對應一個資料專案，並包含一個專案 <code>entry</code></li> 
     <li>專案<code>entry </code>包含<code>key </code>的集合，並且 <code>value</code></li> 
     <li>專案<code>key </code>包含標籤的名稱</li> 
     <li>專案<code>value </code>包含標籤的值</li> 
    </ul> 
    <p>若要新增專案：</p>
    <ol> 
     <li> 按一下<b>[！UICONTROL新增專案]</b>。 </li> 
     <li>選取專案的值型別。</li> 
     <li>新增名稱和值。 如需詳細資訊，請參閱本文所選值型別的範例。 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">簡單值標籤</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">條件標籤</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">回圈標籤</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>
