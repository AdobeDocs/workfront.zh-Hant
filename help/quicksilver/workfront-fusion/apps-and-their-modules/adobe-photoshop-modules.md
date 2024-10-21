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
source-git-commit: c3187e3dc21b4705a0e249ed8cc6df66575ef06b
workflow-type: tm+mt
source-wordcount: '4308'
ht-degree: 0%

---

# [!DNL Adobe Photoshop]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Adobe Photoshop]的工作流程，並將其連線至多個協力廠商應用程式和服務。


如果您需要有關建立案例的指示，請參閱[建立案例](../../workfront-fusion/scenarios/create-a-scenario.md)。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 存取需求

+++**展開以檢視本文中功能的存取需求。**

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
      <td>您的組織必須購買[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文所述的功能。</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

&#42;&#42;如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

+++

## 先決條件

使用[!DNL Adobe Photoshop]聯結器之前，您必須確定符合下列先決條件：

* 您必須擁有使用中的[!DNL Adobe Photoshop]帳戶。

## 建立與[!DNL Adobe Photoshop]的連線

若要為您的[!DNL Adobe Photoshop]模組建立連線：

1. 按一下[連線]方塊旁的&#x200B;**[!UICONTROL 新增]**。

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
        <td>輸入您的[!DNL Adobe] [！UICONTROL使用者端密碼]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL技術帳戶ID]</td>
        <td>輸入您的[!DNL Adobe] [！UICONTROL技術帳戶ID]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL組織ID]</td>
        <td>輸入您的[!DNL Adobe] [！UICONTROL組織識別碼]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL私密金鑰]</td>
        <td>
          <p>輸入在[!DNL Adobe Developer Console]中建立認證時產生的私密金鑰。 </p>
          <p>若要擷取您的私密金鑰或憑證：</p>
          <ol>
            <li value="1">
              <p>按一下<b>[！UICONTROL Extract]</b>。</p>
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
              <p>按一下<b>儲存</b>以擷取檔案，並返回th[！UICONTROL ]e連線設定。</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以儲存連線並返回模組。

## [!DNL Adobe Photoshop]模組及其欄位

當您設定[!DNL Adobe Photoshop]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Adobe Photoshop]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [套用PSD編輯](#apply-psd-edits)
* [自動色彩校正影像](#auto-color-correct-an-image)
* [轉換影像格式](#convert-image-format)
* [建立遮色片](#create-a-mask)
* [建立新PSD](#create-a-new-psd)
* [編輯文字圖層](#edit-text-layers)
* [執行深度模糊](#execute-depth-blur)
* [執行Photoshop動作](#execute-photoshop-actions)
* [執行Photoshop動作(JSON)](#execute-photoshop-actions-json)
* [執行產品裁切](#execute-product-crop)
* [取得圖層資訊](#get-layer-info)
* [進行自訂API呼叫](#make-a-custom-api-call)
* [移除背景](#remove-background)
* [取代智慧型物件](#replace-a-smart-object)
* [調整影像大小](#resize-an-image)
* [為影像加上浮水印](#watermark-an-image)

### 套用PSD編輯

此動作模組會套用各種檔案和圖層層級編輯。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸入）儲存體]</td>
      <td>
        <p>選取儲存您要編輯之檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應您要編輯之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項&gt;檔案&gt;影像大小）高度]</p>
      </td>
      <td> 輸入或對應影像的高度（畫素）。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項&gt;檔案&gt;影像大小）寬度]</p>
      </td>
      <td> 輸入或對應影像的寬度（畫素）。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項&gt;檔案&gt;畫布大小） Top]</p>
      </td>
   <td> 輸入或對應檔案左上角的y座標（畫素）。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項&gt;檔案&gt;畫布大小）底部]</p>
      </td>
   <td> 輸入或對應檔案右下角的y座標（畫素）。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項&gt;檔案&gt;畫布大小）左側]</p>
      </td>
   <td> 輸入或對應檔案左上角的x座標（畫素）。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項&gt;檔案&gt;畫布大小） Right]</p>
      </td>
   <td> 輸入或對應檔案右下角的x座標（畫素）。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項&gt;檔案）修剪]</p>
      </td>
   <td> 選取「透明畫素」，讓修剪以影像中的透明畫素為依據。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項）預設字型]</p>
      </td>
   <td> 輸入要做為檔案全域預設值之字型的完整postscript名稱。 此字型將用於任何文字圖層，該文字圖層缺少字型，而且沒有為該圖層特別提供其他字型。 如果缺少此字型，則在「管理缺少的字型」中指定的選項將會生效。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL (Options) Fonts]</p>
      </td>
   <td> 針對檔案所需的每種字型，按一下「新增專案」並輸入字型的儲存位置和檔案位置。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL (Options) Manage missing fonts]</p>
      </td>
   <td> 選取當檔案中有一或多個遺失字型時要採取的動作。 <ul><li><code>fail</code>：工作不會成功，且狀態會設定為「失敗」，並在狀態的「詳細資訊」區段中提供錯誤的詳細資訊。</li><li><code>useDefault</code>：工作將成功，但依預設，所有遺失的字型都將替換為ArialMT。</li></ul></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （選項）圖層]</p>
      </td>
   <td> 對於每個要新增的圖層，按一下「新增專案」並填入圖層詳細資訊。 <p>如需圖層選項的詳細資訊，請參閱Adobe Photoshop檔案中的<a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_applyPsdEdits/">套用PSD編輯</a>。  </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出]</td>
      <td>
        <p>針對每一個要建立的轉換檔案，按一下「新增專案」，然後輸入儲存體、位置及型別，如本表所列。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取您要儲存新檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應將儲存新檔案的URL或路徑。 只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）型別]</p>
      </td>
   <td>選取您要轉換檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
    </tbody>
</table>



### 自動色彩校正影像

此動作模組自動色彩校正指定的影像。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸入）儲存體]</td>
      <td>
        <p>選取儲存您要校正色彩之檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應您要校正顏色之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取您要儲存新檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應將儲存新檔案的URL或路徑。 只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）型別]</p>
      </td>
   <td>選取您要轉換檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
    </tbody>
</table>


### 轉換影像格式

此動作模組會將檔案轉換為JPEG、PNG、PSD或TIFF。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸入）儲存體]</td>
      <td>
        <p>選取要從中移除背景的檔案儲存所在的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應您要移除背景之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出]</td>
      <td>
        <p>針對每一個要建立的轉換檔案，按一下「新增專案」，然後輸入儲存體、位置及型別，如本表所列。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取您要儲存新檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應將儲存新檔案的URL或路徑。 只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）型別]</p>
      </td>
   <td>選取您要轉換檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
    </tbody>
</table>



### 建立遮色片

此動作模組會傳回PNG檔案，並在主旨周圍套用主旨。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸入）儲存體]</td>
      <td>
        <p>選取要用來建立遮罩的檔案儲存所在的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應您要建立遮色片之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取您要儲存遮罩檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應遮罩檔案儲存位置的URL或路徑。 只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL色域]</p>
      </td>
   <td>選取輸出影像是使用RGB還是RGBA色彩。 </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL遮罩格式]</p>
      </td>
   <td>選取遮色片應該柔和（羽化）還是二進位。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL最佳化]</p>
      </td>
   <td>選取效能以最佳化速度，或選取批次以允許等待時間。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL後處理]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL版本]</p>
      </td>
   <td>預設值為4.0</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
    </tbody>
</table>

### 建立新PSD

此動作模組會建立具有選用圖層的新PSD，並產生轉譯或儲存為PSD。

如需與此模組相關的欄位，請參閱Adobe Photoshop檔案中的[建立新PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate)。

### 編輯文字圖層

此動作模組會編輯Photoshop檔案上的文字圖層。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
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
   <td> <p>如需圖層選項的詳細資訊，請參閱Adobe Photoshop檔案中的<a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">編輯文字圖層</a>。</p>  </td>     </tr>
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



### 執行Photoshop動作(JSON)

此動作模組會使用JSON命令執行Photoshop動作。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸入）儲存體]</td>
      <td>
        <p>選取儲存您要編輯之檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應您要編輯之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL動作JSON]</td>
      <td>
        <p>輸入您要執行動作的JSON命令。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL字型/圖案/筆刷/其他影像]</td>
      <td>
        <p>針對每一個要在此動作中使用的字型、圖樣、筆刷或其他影像，按一下「新增專案」，然後輸入專案的儲存和檔案位置。</p>
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
        <p>選取要儲存編輯檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL輸出檔案URL]</p>
      </td>
   <td> 輸入或對應將儲存已編輯檔案的URL或路徑。  只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
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
    <tr>
      <td role="rowheader">[！UICONTROL輸出]</td>
      <td>
        <p>針對每一個要建立的轉換檔案，按一下「新增專案」，然後輸入儲存體、位置及型別，如本表所列。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取您要儲存新檔案的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應將儲存新檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）型別]</p>
      </td>
   <td>選取您要轉換檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
      </tbody>
</table>

### 執行深度模糊

此動作模組會在選取的檔案上執行「深度模糊」。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
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
        <p>如需其他「深度模糊」選項的詳細資訊，請參閱Adobe Photoshop API檔案中的<a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">執行深度模糊</a>。</p>
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

### 執行Photoshop動作

此動作模組會對選取的影像執行Photoshop動作。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
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

### 執行產品裁切

此動作模組會針對選取的影像執行產品裁切。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
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

### 取得圖層資訊

此動作模組會從指定的PSD檔案中擷取圖層資訊。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
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

### 進行自訂API呼叫

此動作模組會對Photoshop API進行自訂呼叫。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>輸入相對於<code>https://image.adobe.io/pie/psdService</code>的路徑。 範例： <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
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
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### 移除背景

此動作模組會識別影像的主要主旨並移除背景。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸入）儲存體]</td>
      <td>
        <p>選取要從中移除背景的檔案儲存所在的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應您要移除背景之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取您要儲存新檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應將儲存新檔案的URL或路徑。  只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL色域]</p>
      </td>
   <td>選取輸出影像是使用RGB還是RGBA色彩。 </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL遮罩格式]</p>
      </td>
   <td>選取影像的邊緣應該是柔和（羽化）還是二進位。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL最佳化]</p>
      </td>
   <td>選取效能以最佳化速度，或選取批次以允許等待時間。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL後處理]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL版本]</p>
      </td>
   <td>預設值為4.0</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
    </tbody>
</table>



### 取代智慧型物件

此動作模組會取代PSD圖層中的「智慧型物件」，並產生新的轉譯。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸入）儲存體]</td>
      <td>
        <p>選取儲存智慧物件的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應智慧型物件的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL圖層]</p>
      </td>
   <td>針對您想要新增至「智慧型物件」的每個圖層，按一下「新增專案」，然後輸入物件的名稱或ID、儲存智慧型物件的檔案服務，以及圖層的URL或路徑。<p>如需此區域進階設定的說明，請參閱Photoshop API檔案中的<a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_replaceSmartObject/">取代智慧型物件</a> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出]</td>
      <td>
        <p>針對您希望模組產生的每個新轉譯，按一下「新增專案」並填寫下列欄位。 您最多可以有25個輸出檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取您要儲存新檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應將儲存新檔案的URL或路徑。  只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）寬度]</p>
      </td>
   <td> 輸出檔案的寬度（畫素）。 模組將保留原始的外觀比例。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
    </tbody>
</table>



### 調整影像大小

此動作會使用相同外觀比例來調整影像大小。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL儲存]</td>
      <td>
        <p>選取要儲存檔案大小的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL檔案位置]</p>
      </td>
   <td> 輸入或對應您要調整大小的檔案的URL或路徑。  只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸出]</td>
      <td>
        <p>針對每一個要建立的轉換檔案，按一下「新增專案」，然後輸入此表格中所列的儲存體、位置和其他選項。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL型別]</p>
      </td>
   <td>選取您要轉換檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL寬度]</p>
      </td>
   <td>請輸入數字，代表調整大小後影像的寬度（以畫素為單位）。 將會保留外觀比例。</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL最大寬度]</p>
      </td>
   <td>當寬度為0時，可提供的最大值搭配以取得大小。 最大寬度優先於小於檔案寬度。</td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL Trim to canvas]</p>
      </td>
   <td>選取「是」將轉譯裁剪為「畫布」大小，或選取「否」將轉譯設為「圖層大小」。</td> 
    </tr>
    </tbody>
</table>

### 為影像加上浮水印

此動作模組會將浮水印新增至選取的影像。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Photoshop]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >建立與[!DNL Adobe Photoshop]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （基底/輸入）儲存]</td>
      <td>
        <p>選取要新增浮水印的檔案儲存所在的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （基底/輸入）檔案位置]</p>
      </td>
   <td> 輸入或對應您要新增浮水印之檔案的URL或路徑。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （浮水印/輸入）儲存]</td>
      <td>
        <p>選取要儲存浮水印的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （浮水印/輸入）儲存]</td>
      <td>
        <p>選取要儲存浮水印的檔案服務。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （浮水印/界限）高度]</p>
      </td>
   <td>輸入或對應所需的浮水印高度（畫素）。</td> 
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （浮水印/界限）寬度]</p>
      </td>
   <td> 輸入或對應所需的浮水印寬度（畫素）。 </td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （浮水印/界限）左側]</p>
      </td>
   <td> 輸入或對應距離影像左側的距離（以畫素為單位），也就是浮水印應該距離的位置。</td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （浮水印/界限）頂端]</p>
      </td>
   <td> 輸入或對應浮水印應該位於的距離影像頂端（以畫素為單位）。</td> 
    </tr>  
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）儲存]</td>
      <td>
        <p>選取要儲存浮水印檔案的檔案服務。</p><p>選取Fusion內部儲存體可讓檔案供後續模組使用，但無法讓檔案在情境之外使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）檔案位置]</p>
      </td>
   <td> 輸入或對應要儲存浮水印檔案的URL或路徑。 只有在您尚未為輸出儲存體選擇Fusion內部儲存體時，才需要這樣做。</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）型別]</p>
      </td>
   <td>選取您要轉換檔案的檔案型別。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL （輸出）寬度]</p>
      </td>
   <td> 輸出檔案的寬度（畫素）。 模組將保留原始的外觀比例。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL （輸出）覆寫]</td>
      <td>
        <p>選取新編輯的檔案是否會覆寫任何已存在的輸出檔案。 這僅適用於Adobe儲存體中的檔案。</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回結果的最大數目]</p>
      </td>
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
    </tr>
    </tbody>
</table>















