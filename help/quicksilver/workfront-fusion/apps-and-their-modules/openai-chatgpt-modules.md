---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Openai (ChatGPT)模組
description: 在Adobe Workfront Fusion案例中，您可以自動化使用OpenAIT(ChatGPT)的工作流程，並將其連結到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
source-git-commit: a8bc882f393dcf17bca80da86c25c053272e27c9
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# [!DNL OpenAI (ChatGPT & DALL-E)] 模組

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL OpenAI (ChatGPT & DALL-E)]，並連結至多個協力廠商應用程式和服務。

如果您需要有關建立情境的指示，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先決條件

使用 [!DNL OpenAI (ChatGPT & DALL-E)] 模組，您必須擁有 [!DNL OpenAI] 帳戶，包括API金鑰和組織ID。

## 正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]

您可以建立與您的電腦的連線， [!DNL OpenAI (ChatGPT & DALL-E)] 直接從 [!DNL OpenAI (ChatGPT & DALL-E)] 模組。

1. 在任何 [!DNL OpenAI (ChatGPT & DALL-E)] 模組，按一下 **[!UICONTROL 新增]** 在 [!UICONTROL 連線] 欄位。
1. 輸入下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL連線名稱]</p> </td> 
      <td> <p>輸入新連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL API Key]</td> 
      <td>您可以在OpenAI使用者設定中找到API金鑰。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL組織ID] </td> 
      <td>您可以在OpenAI的「組織設定」頁面上找到您的組織ID。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。


## [!DNL OpenAI (ChatGPT & DALL-E)] 模組及其欄位

當您設定 [!DNL OpenAI (ChatGPT & DALL-E)] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL OpenAI (ChatGPT & DALL-E)] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 建立完成

此動作模組會為提供的提示或聊天建立完成。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL模型]</td> 
   <td> 輸入或對映要使用的模型ID。 您可以使用「取得模型」模組來檢視所有可用的模型。 </td> 
  </tr> 
  <!--<tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">[！UICONTROL進階設定]</td> 
   <td> <p>如需此模組中選擇性進階設定的相關資訊，請參閱此模組中有關建立完成的資訊。 <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">OpenAI API檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 建立稽核

此動作模組會判斷文字是否違反OpenAI的內容原則。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入]</td> 
   <td> 對於要包含的每個文字範例，按一下 <b>新增專案</b> 並輸入或對應文字。 包含整個文字範例。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL模型]</td> 
   <td> 輸入或對映要使用的模型ID。 您可以使用「取得模型」模組來檢視所有可用的模型。 </td> 
  </tr> 
 </tbody> 
</table>

### 建立編輯

此動作模組會依照您的指示，傳回您提供的提示的編輯版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL模型]</td> 
   <td> 輸入或對映要使用的模型ID。 您可以使用「取得模型」模組來檢視所有可用的模型。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入]</td> 
   <td> 輸入或對應您要編輯的文字。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL指令]</td> 
   <td> 輸入或對映編輯的指示。 範例：「修正拼字錯誤」。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL進階設定]</td> 
   <td> <p>如需此模組中選擇性進階設定的相關資訊，請參閱 <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">OpenAI API檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 建立內嵌

此動作模組會建立代表輸入文字的內嵌向量。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL模型]</td> 
   <td> 輸入或對映要使用的模型ID。 您可以使用「取得模型」模組來檢視所有可用的模型。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要嵌入的輸入文字]</td> 
   <td> 輸入或對應您要內嵌的文字。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用者ID]</td> 
   <td> 輸入或對應代表一般使用者的唯一識別碼，可協助OpenAI監控及偵測不當行為 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> 輸入或對應每個案例執行週期中您希望模組使用的最大編輯次數。</td> 
  </tr> 
 </tbody> 
</table>

### 建立聊天完成

指定描述交談的訊息清單，此動作模組會傳回回應。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL模型]</td> 
   <td> 輸入或對映要使用的模型ID。 您可以使用「取得模型」模組來檢視所有可用的模型。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息]</td> 
   <td>訊息說明目前為止的交談。 對於每個要新增的訊息，按一下 <b>新增專案</b> 並填入下列內容：
   <ul>
   <li> <b>角色</b>：選取此訊息作者的角色。</li>
   <li> <b>內容</b>：輸入或對應此訊息的內容。</li>
   <li> <b>名稱</b>：輸入或對應此訊息作者的名稱。 名稱可包含大寫和小寫字母、數字和底線。 名稱的長度上限為64個字元。</li>
   </ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL進階設定]</td> 
   <td> <p>如需有關本單元中可選進階設定的資訊，請參閱 <a href="https://platform.openai.com/docs/api-reference/chat/create" class="MCXref xref">OpenAI API檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Edit image

This action module makes edits or creates variations of existing images.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to create edits or variations of the image.
   <p>NOTE: Images must be a valid PNG file, less than 4MB, and square. If mask is not provided, the image must have transparency, which will be used as the mask.</p> 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Text description of desired image]</td> 
   <td> <p>If editing an image, enter or map a description of the edits you want to create. Maximum length is 1000 characters.</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating image edits or variations in the <a href="https://platform.openai.com/docs/api-reference/images/createEdit" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### 產生影像

此動作模組會使用Dall-E模型產生或操作影像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL所要影像的文字說明]</td> 
   <td> 輸入或對應所需影像的說明。 說明長度上限為1000個字元。 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[！UICONTROL進階設定]</td> 
   <td> <p>如需此模組中選擇性進階設定的相關資訊，請參閱此模組中有關建立影像的資訊。 <a href="https://platform.openai.com/docs/api-reference/images/create" class="MCXref xref">OpenAI API檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 取得模型

此模組列出並說明OpenAI API中可用的各種模型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL動作]</td> 
   <td> 選取您要取得所有模型的清單或擷取特定模型。
    <ul>
    <li><p><b>清單模型 </b></p><p>此動作會列出目前可用的模型，並提供每個模型的基本資訊，例如擁有者和可用性。</p></li>
    <li><p><b>擷取模型 </b></p><p>輸入或對應您要擷取的模型ID。 </p></li>
   </ul>
 </td> 
 </tbody> 
</table>

### 進行自訂API呼叫

此動作模組會向OpenAI API傳送自訂HTTP請求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>輸入相對於 <code>https://api.openai.com/v1/</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Manage Audio

This action modules converts audio to text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to transcribe the audio into the input language, or into English.
   <p>If transcribing into the input language, you can select the language in this module's advanced settings. </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to work with during each scenario execution cycle.</td> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating transcriptions in the <a href="https://platform.openai.com/docs/api-reference/audio/createTranscription" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

-->

### 管理檔案

此動作模組會列出、刪除或擷取檔案或檔案內容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL動作]</td> 
   <td> 選取您要執行的動作。 
  </tr> 
   <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td> 如果您要刪除檔案，或擷取檔案或檔案內容，請輸入或對應檔案的ID。 
  </tr> 
</tbody>
</table>

### 管理微調

管理微調工作，根據您的特定訓練資料量身打造模型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion的帳戶，請參閱 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL OpenAI (ChatGPT & DALL-E)] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取操作]</td> 
   <td> 選取您要執行的動作。
   <ul>
   <li><p>從資料集微調模型</p><p>輸入或對應所需影像的說明。</p>
     <li><p>取得微調工作的相關資訊</p><p>輸入或對映工作的ID。</p>
   <li><p>取消微調工作</p><p>輸入或對映工作的ID。</p>
   <li><p>取消微調工作</p><p>輸入或對映工作的ID。</p>
   <li><p>取得微調工作的狀態更新</p><p>輸入或對應工作的ID，然後選取是否要串流這些更新。</p>
   <li><p>刪除微調模型</p><p>輸入或對應您要刪除的模型ID。</p>
 </ul> 
  </tr> 
   <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td> 如果您要刪除檔案，或擷取檔案或檔案內容，請輸入或對應檔案的ID。 
  </tr> 
</tbody>

