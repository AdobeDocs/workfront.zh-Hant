---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Photoshop模組
description: 透過Adobe Photoshop模組，您可以根據Adobe Photoshop帳戶中的事件啟動Adobe Workfront Fusion案例，建立、讀取或更新協定和其他記錄，使用您設定的條件搜尋記錄，以及上傳檔案。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 6bcf404432129a812b5e4d840b59e72f036ec723
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] 模組

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Adobe Photoshop]，並連結至多個協力廠商應用程式和服務。


如果您需要有關建立情境的指示，請參閱 [建立情境](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
      <td>
        <p>[！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
      <td>
        <p>[！UICONTROL計畫]，[！UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td>
      <td >
        <p>[！UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">產品</td>
      <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

&#42;&#42;有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先決條件

開始使用 [!DNL Adobe Photoshop] 聯結器時，您必須確定符合下列先決條件：

* 您必須擁有使用中 [!DNL Adobe Photoshop] 帳戶。

## 建立與的連線 [!DNL Adobe Photoshop]

若要為建立連線，請執行下列步驟： [!DNL Adobe Photoshop] 模組：

1. 按一下 **[!UICONTROL 新增]** ，位於「連線」方塊旁。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[！UICONTROL連線名稱]</td>
        <td>
          <p>輸入此連線的名稱。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的[！UICONTROLAdobe] [！UICONTROL使用者端ID]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的 [!DNL Adobe] [！UICONTROL使用者端密碼]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL技術帳戶ID]</td>
        <td>輸入您的 [!DNL Adobe] [！UICONTROL技術帳戶ID]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL組織ID]</td>
        <td>輸入您的 [!DNL Adobe] [！UICONTROL組織識別碼]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL私密金鑰]</td>
        <td>
          <p>輸入在中建立您的認證時產生的私密金鑰 [!DNL Adobe Developer Console]. </p>
          <p>若要擷取您的私密金鑰或憑證：</p>
          <ol>
            <li value="1">
              <p>按一下 <b>[！UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>選取要解壓縮的檔案型別。</p>
            </li>
            <li value="3">
              <p>選取包含私密金鑰或憑證的檔案。</p>
            </li>
            <li value="4">
              <p>輸入檔案的密碼。</p>
            </li>
            <li value="5">
              <p>按一下 <b>儲存</b> 以擷取檔案並返回[！UICONTROL ]e連線設定。</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## [!DNL Adobe Photoshop] 模組及其欄位

當您設定 [!DNL Adobe Photoshop] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Adobe Photoshop] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### 動作

* [建立新PSD](#create-a-new-psd)
* [編輯文字圖層](#edit-text-layers)
* [執行深度模糊](#execute-depth-blur)
* [執行Photoshop動作](#execute-photoshop-actions)
* [執行產品裁切](#execute-product-crop)
* [取得圖層資訊](#get-layer-info)
* [進行自訂API呼叫](#make-a-custom-api-call)

#### 建立新PSD

此動作模組會建立具有選用圖層的新PSD，並產生轉譯或儲存為PSD。

如需與此模組相關的欄位，請參閱 [建立新PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) (位於Adobe Photoshop檔案中)。

#### 編輯文字圖層

此動作模組會編輯Photoshop檔案上的文字圖層。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Photoshop]，請參閱 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與的連線 [!DNL Adobe Photoshop]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入檔案儲存]</td>
      <td>
        <p>選取儲存您要編輯之檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸入檔案URL]</p>
      </td>
   <td> 輸入或對應您要編輯之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Manage missing fonts]</td>
      <td>
        <p>選取當檔案中有一或多個遺失字型時要採取的動作。 如果未提供字型，模組會使用預設字型。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL預設字型]  </td>
      <td>
        <p>輸入要做為檔案全域預設值之字型的完整postscript名稱。 此字型將用於任何文字圖層，該文字圖層缺少字型，而且沒有為該圖層特別提供其他字型。 如果缺少此字型，則在「管理缺少的字型」中指定的選項將會生效。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL圖層]</td>
   <td> <p>如需圖層選項的詳細資訊，請參閱 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">編輯文字圖層</a> (位於Adobe Photoshop檔案中)。</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出檔案儲存]</td>
      <td>
        <p>選取要儲存編輯檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案URL]</p>
      </td>
   <td> 輸入或對應將儲存已編輯檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案型別]</p>
      </td>
   <td> 選取已編輯檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL壓縮]</p>
      </td>
   <td> 選取輸出檔案的壓縮等級。 </td> 
    </tr>
  </tbody>
</table>

#### 執行深度模糊

此動作模組會在選取的檔案上執行「深度模糊」。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Photoshop]，請參閱 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與的連線 [!DNL Adobe Photoshop]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入檔案儲存]</td>
      <td>
        <p>選取儲存您要編輯之檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸入檔案URL]</p>
      </td>
   <td> 輸入或對應您要編輯之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出檔案儲存]</td>
      <td>
        <p>選取要儲存編輯檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案URL]</p>
      </td>
   <td> 輸入或對應將儲存已編輯檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案型別]</p>
      </td>
   <td> 選取已編輯檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL其他欄位]</td>
      <td>
        <p>如需其他「深度模糊」選項的詳細資訊，請參閱 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">執行深度模糊 </a>在Adobe Photoshop API檔案中。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL壓縮]</p>
      </td>
   <td> 選取輸出檔案的壓縮等級。 </td> 
    </tr>
  </tbody>
</table>

#### 執行Photoshop動作

此動作模組會對選取的影像執行Photoshop動作。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Photoshop]，請參閱 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與的連線 [!DNL Adobe Photoshop]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入檔案儲存]</td>
      <td>
        <p>選取儲存您要編輯之檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸入檔案URL]</p>
      </td>
   <td> 輸入或對應您要編輯之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Actions檔案儲存]</td>
      <td>
        <p>選取儲存動作檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL動作檔案URL]</p>
      </td>
   <td> 輸入或對應動作檔案的URL或路徑。 </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL動作名稱]</p>
      </td>
   <td> 如果只想執行特定動作，您可以指定要從ActionSet播放哪個動作。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL字型/圖樣/筆刷儲存]</td>
      <td>
        <p>選取要用來儲存檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL字型/模式/筆刷檔案URL]</p>
      </td>
   <td> 輸入或對應您要使用的檔案URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出檔案儲存]</td>
      <td>
        <p>選取要儲存編輯檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案URL]</p>
      </td>
   <td> 輸入或對應將儲存已編輯檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案型別]</p>
      </td>
   <td> 選取已編輯檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL壓縮]</p>
      </td>
   <td> 選取輸出檔案的壓縮等級。 </td> 
    </tr>
  </tbody>
</table>

#### 執行產品裁切

此動作模組會針對選取的影像執行產品裁切。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Photoshop]，請參閱 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與的連線 [!DNL Adobe Photoshop]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入檔案儲存]</td>
      <td>
        <p>選取要儲存裁切之檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸入檔案URL]</p>
      </td>
   <td> 輸入或對應您要裁切之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL單位]</p>
      </td>
   <td> 選取您要以畫素或百分比描述高度和寬度調整。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL寬度]</p>
      </td>
   <td> 輸入或對映您想要新增的寬度邊框間距。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL Height]</p>
      </td>
   <td> 輸入或對映您想要增加的高度邊框間距。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出檔案儲存]</td>
      <td>
        <p>選取要儲存編輯檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案URL]</p>
      </td>
   <td> 輸入或對應將儲存已編輯檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案型別]</p>
      </td>
   <td> 選取已編輯檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL壓縮]</p>
      </td>
   <td> 選取輸出檔案的壓縮等級。 </td> 
    </tr>
  </tbody>
</table>

#### 取得圖層資訊

此動作模組會從指定的PSD檔案中擷取圖層資訊。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Photoshop]，請參閱 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與的連線 [!DNL Adobe Photoshop]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入檔案儲存]</td>
      <td>
        <p>選取要從中擷取圖層資訊的檔案儲存所在的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸入檔案URL]</p>
      </td>
   <td> 輸入或對應您要擷取圖層資訊之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL縮圖]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### 進行自訂API呼叫

此動作模組會對Photoshop API進行自訂呼叫。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Photoshop]，請參閱 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與的連線 [!DNL Adobe Photoshop]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>輸入相對於 <code>https://image.adobe.io/pie/psdService</code>. 範例： <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查詢字串]  </td>
      <td>
        <p>輸入請求查詢字串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
