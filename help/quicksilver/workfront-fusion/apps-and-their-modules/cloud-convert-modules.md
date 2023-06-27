---
title: CloudConvert模組
description: CloudConvert模組
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3041'
ht-degree: 0%

---

# [!DNL CloudConvert] 模組

在Adobe Workfront Fusion案例中，您可以自動化使用CloudConvert的工作流程，並將其連線到多個第三方應用程式和服務。 此 [!DNL CloudConvert] 模組可讓您監視和管理工作、任務，以及匯入和匯出中的檔案。 [!DNL CloudConvert] 帳戶。

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

## Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

若要連線您的 [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，您必須向取得API金鑰 [!DNL CloudConvert] 帳戶。

1. 登入您的 [!DNL CloudConvert] 帳戶並開啟您的 [!UICONTROL 儀表板].
1. 開啟 **[!UICONTROL Authorization] > [!UICONTROL API金鑰]** 區段。
1. 按一下 **[!UICONTROL 建立新的API金鑰]**.
1. 輸入API金鑰的名稱，啟用您要使用的範圍，然後按一下 **[!UICONTROL 建立]**.
1. 複製提供的Token並將其儲存在安全的地方。
1. 在 [!DNL Workfront Fusion]，開始建立情境並開啟 [!DNL CloudConvert] 模組的 **[!UICONTROL 建立連線]** 對話方塊。

   如需指示，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 輸入您在步驟5中儲存的Token，然後按一下 **[!UICONTROL 繼續]** 以建立連線。

## [!DNL CloudConvert] 模組及其欄位 {#cloudconvert-modules-and-their-fields}

當您設定 [!DNL CloudConvert] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL CloudConvert] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [常見任務](#common-tasks)
* [工作](#jobs)
* [任務](#tasks)
* [其他](#other)

### 常見任務

* [擷取網站](#capture-a-website)
* [[!UICONTROL 轉換檔案]](#convert-a-file)
* [建立封存](#create-an-archive)
* [合併檔案](#merge-files)
* [最佳化檔案](#optimize-a-file)

#### [!UICONTROL 擷取網站]

此動作模組會擷取指定的網站，並以PDF、JPG或PNG格式儲存。

您可以指定網站的URL和其他資訊，例如要儲存資訊的位置。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入您要擷取的網站URL。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出格式] </td> 
   <td>選取您要以PNG、JPG或PDF格式儲存擷取的網站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案名稱] </td> 
   <td>輸入目標輸出檔案的檔案名稱（包括副檔名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭] </td> 
   <td> <p>（選用）定義請求標頭。 </p> <p>這在指定的URL需要授權時很有用。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL轉換和引擎特定選項] </p> </td> 
   <td>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 以下專案的檔案 <code>input_format</code> 和 <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下載檔案] </td> 
   <td> <p>如果您也想要在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 轉換檔案]

將檔案轉換為選取的輸出格式。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案]</td> 
   <td>選擇您是否要使用上傳檔案 [!DNL Workfront Fusion] 或提供檔案上傳來源的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上傳檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL從URL匯入檔案]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL URL]</strong> </p> <p>輸入您要轉換之檔案的URL。</p> </li> 
     <li> <p><strong>[！UICONTROL標頭]</strong></p> <p>定義請求標頭（選用）。 這在指定的URL需要授權時很有用。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL格式]</td> 
   <td>選取是否要指定要轉換之檔案的輸入格式。 如果未指定，則會使用輸入檔案的副檔名作為輸入格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>選取檔案的目前格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL輸出格式]</td> 
   <td>選取您要轉換檔案的目標檔案格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL檔案名稱]</td> 
   <td>選擇目標輸出檔案的檔案名稱（包括副檔名）。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL轉換和引擎特定選項] </p> </td> 
   <td>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 以下專案的檔案 <code>input_format</code> 和 <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL下載檔案] </td> 
   <td> <p>如果您也想要在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立封存]

可讓您新增一或多個檔案至ZIP、RAR、7Z、TAR、TAR.GZ或TAR.BZ2封存。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL輸入檔案]</p> </td> 
   <td> <p>指定您要新增至封存的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上傳檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL從URL匯入檔案]</p> </td> 
   <td> <p><strong>[！UICONTROL URL]</strong> </p> <p>輸入您要封存檔案的URL。</p> <p><strong>[！UICONTROL標頭]</strong> </p> <p>定義請求標頭（選用）。 這在指定的URL需要授權時很有用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出格式]</td> 
   <td> <p> 選取已封存檔案的目標格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案名稱]</td> 
   <td> <p> 輸入目標輸出檔案的檔案名稱（包括副檔名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL轉換和引擎特定選項] </td> 
   <td> <p>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 以下專案的檔案 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下載檔案]</td> 
   <td> <p>如果您也想要在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 合併檔案]

至少將兩個檔案合併到一個PDF中。 如果輸入檔案不是PDF，則會自動轉換為PDF。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL輸入檔案]</p> </td> 
   <td> <p>指定您要合併的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上傳檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL從URL匯入檔案]</p> </td> 
   <td> <p><strong>[！UICONTROL URL]</strong> </p> <p>輸入您要封存檔案的URL。</p> <p><strong>[！UICONTROL標頭]</strong> </p> <p>定義請求標頭（選用）。 這在指定的URL需要授權時很有用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出格式]</td> 
   <td> <p> 選取合併檔案的目標格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案名稱]</td> 
   <td> <p> 輸入目標輸出檔案的檔案名稱（包括副檔名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL轉換和引擎特定選項] </td> 
   <td> <p>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 以下專案的檔案 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下載檔案]</td> 
   <td> <p>如果您也想要在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 最佳化檔案]

此動作模組會最佳化並壓縮PDF、PNG或JPG格式的檔案。

您可以指定檔案以及最佳化和儲存檔案的引數。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案]</td> 
   <td>選取您要使用Workfront Fusion上傳檔案，或提供要從中上傳檔案的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL上傳檔案]</p> </td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL從URL匯入檔案] </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL URL]</strong>：輸入您要轉換之檔案的URL。</li> 
     <li><strong>[！UICONTROL標頭]</strong>：（選用）定義請求標頭。 這在指定的URL需要授權時很有用。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Optimization for] </td> 
   <td> <p>針對特定目標需求選取最佳化設定檔。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL Web]</strong>：最佳化網頁（預設）</p> 
      <ul> 
       <li>移除Web多餘和不必要的資料</li> 
       <li>縮減取樣、剪下並聰明地壓縮影像</li> 
       <li>合併字型和子集字型</li> 
       <li>將顏色轉換為RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL列印]</strong>：最佳化列印</p> 
      <ul> 
       <li> <p>移除多餘和不必要的列印資料</p> </li> 
       <li> <p>縮減取樣、剪下並聰明地壓縮影像</p> </li> 
       <li> <p>合併字型和子集字型</p> </li> 
       <li> <p>將顏色轉換為CMYK</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL封存]</strong>：針對封存用途最佳化</p> 
      <ul> 
       <li> <p>移除多餘和不必要的資料以進行封存</p> </li> 
       <li> <p>智慧型壓縮影像</p> </li> 
       <li> <p>合併字型和子集字型</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL掃描的影像]</strong>：最佳化掃描的影像</p> 
      <ul> 
       <li> <p>針對主要由點陣影像組成的PDF最佳化的設定檔</p> </li> 
       <li> <p>壓縮影像，而不大幅降低視覺品質</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL最大尺寸縮減]</strong>：最佳化以最大程度地縮減大小</p> 
      <ul> 
       <li> <p>使用最大可能的壓縮</p> </li> 
       <li> <p>可能會降低視覺品質</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入格式] </td> 
   <td>選取要最佳化的輸入檔案格式。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案名稱]</td> 
   <td> <p>輸入目標輸出檔案的檔案名稱（包括副檔名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL轉換和引擎特定選項]</td> 
   <td> <p>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 以下專案的檔案 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下載檔案]</td> 
   <td> <p>如果您也想要在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 工作

* [[!UICONTROL 建立工作（進階）]](#create-a-job-advanced)
* [[!UICONTROL 新增工作事件]](#new-job-event)
* [[!UICONTROL 列出工作]](#list-jobs)
* [[!UICONTROL 取得工作]](#get-a-job)
* [[!UICONTROL 刪除工作]](#delete-a-job)

#### [!UICONTROL 建立工作（進階）]

此模組會建立工作。 一個工作可以是一個或多個任務，這些任務在 [!UICONTROL 名稱] 欄位，並使用 [!UICONTROL 輸入] 欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案]</td> 
   <td> <p>選擇您是否要使用上傳檔案 [!DNL Workfront Fusion]，或提供要從中上傳檔案的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上傳檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL從URL匯入檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL URL]</strong>：輸入您要處理的檔案URL。</li> 
     <li><strong>[！UICONTROL標頭]</strong>：（選用）定義請求標頭。 這在指定的URL需要授權時很有用。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL工作]</p> </td> 
   <td> <p>新增將在工作內執行的任務。</p> <p>請在對應區段中尋找作業的欄位說明。</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[！UICONTROL轉換檔案]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[！UICONTROL擷取網站]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[！UICONTROL最佳化檔案]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[！UICONTROL建立封存]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[！UICONTROL合併檔案]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL執行命令]</strong> </p> <p>如需執行命令的詳細資訊，請參閱 <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] API檔案</a>.</p> </li> 
     <li> <p><strong>[！UICONTROL將檔案匯出至暫存URL]</strong> </p> <p> 指定工作名稱和輸入工作名稱（例如轉換）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤] </td> 
   <td> <p>輸入標籤。 標籤是用來識別工作的任意字串。 註解沒有任何效果，可用來將工作與ID建立關聯。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除工作]

此模組會刪除工作，包括所有任務和資料。

>[!NOTE]
>
>工作會在結束後24小時自動刪除。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作ID]</td> 
   <td> <p>輸入或對應您要刪除之工作的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得工作]

此模組會擷取工作詳細資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作ID]</td> 
   <td> <p>輸入或對應您要擷取相關詳細資訊之作業的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作]

此模組會擷取已在您的帳戶中執行的所有工作。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL狀態] </td> 
   <td> <p>選取工作狀態，以篩選傳回的工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>設定Workfront Fusion 2.0在一個執行週期內傳回的工作數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增工作事件]

在您的帳戶或任務中建立、完成或失敗時觸發。

>[!NOTE]
>
>* 由建立的工作 [!UICONTROL 建立工作（進階）] 模組包含 *數個* 任務。
>* 此 [!UICONTROL 新增工作事件] 觸發條件為 *個人* 任務已建立、已完成或已失敗。
>

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名稱]</td> 
   <td>輸入webhook名稱。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出格式] </td> 
   <td>選取您要以PNG、JPG或PDF格式儲存擷取的網站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件]</td> 
   <td>選取在建立、完成或失敗工作或任務時是否觸發模組。</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 如果使用「陣列彙總」(Array Aggregator) （例如，有許多不同格式的檔案要轉換），請使用 **[!UICONTROL 我不知道輸入格式]** 中的選項 [!UICONTROL 新增任務] 對話方塊。 否則會傳回錯誤。
>* 連結工作內的任務（名稱>輸入、名稱>輸入……）：
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### 任務

* [[!UICONTROL 取得任務]](#get-a-task)
* [[!UICONTROL 下載檔案]](#download-a-file)
* [[!UICONTROL 列出任務]](#list-tasks)
* [[!UICONTROL 重試任務]](#retry-a-task)
* [[!UICONTROL 取消任務]](#cancel-a-task)
* [[!UICONTROL 刪除任務]](#delete-a-task)

#### [!UICONTROL 取消任務]

此模組會取消處於等待或處理狀態的任務。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任務ID]</td> 
   <td> <p> 輸入或對應您要取消的工作的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除任務]

刪除任務，包括所有資料。

>[!NOTE]
>
>任務結束後24小時會自動刪除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任務ID]</td> 
   <td> <p> 輸入（對應）您要刪除之任務的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此模組會從指定的工作擷取檔案名稱和檔案資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任務ID]</td> 
   <td> <p> 輸入或對應您要從其中下載檔案的工作的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得任務]

此模組會擷取任務詳細資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任務ID]</td> 
   <td> <p>輸入或對應您要擷取相關詳細資訊之任務的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出任務]

此模組會根據篩選設定擷取您帳戶中的所有任務。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL狀態] </td> 
   <td> <p>選取任務狀態，以篩選傳回的任務。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作ID] </td> 
   <td> <p>輸入或對應工作ID以僅傳回指定工作內的工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作] </td> 
   <td> <p>輸入作業型別，以僅傳回具有指定作業的任務。 </p> <p>注意：請使用[！UICONTROL List Possible Operations]模組來擷取作業。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重試任務]

此模組會根據其他任務的設定（裝載）建立新任務。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任務ID]</td> 
   <td> <p> 輸入或對應您要建立新任務的任務ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 取得我的資訊]](#get-my-info)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL 取得我的資訊]

擷取有關目前使用者的已驗證帳戶詳細資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL CloudConvert] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行API呼叫]

可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關將[Fusion應用程式]帳戶連線至Workfront Fusion的說明，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>輸入相對於 <code>https://api.cloudconvert.com/</code>. 例如： <code>/v2/tasks</code></p> <p>如需可用端點的清單，請參閱 <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] API v2檔案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**範例：** 列出任務

以下API呼叫傳回您CloudFront帳戶中的所有任務：

URL: `/v2/tasks`

方法: `GET`

![](assets/cloudconvert-api-example-input.png)

您可以在模組的輸出中找到搜尋的相符專案，位於 [!UICONTROL 組合] > [!UICONTROL 內文] > [!UICONTROL 資料].

在我們的範例中，傳回6項工作：

![](assets/cloudconvert-api-example-output.png)

## 疑難排解 {#troubleshooting}

請參閱下表以瞭解可能的錯誤及其解決方案：

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>錯誤</p> </th> 
   <th>後續步驟</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[！UICONTROL輸出檔案大小超過情境所允許的限制。]</span> </p> </td> 
   <td> <p>請參閱檔案大小限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[！UICONTROL您已超過轉換時間上限。]</span> </p> </td> 
   <td> <p>免費 [!DNL CloudConvert] 計畫提供每日25分鐘的轉換。 如果您的使用情況超過免費方案的限制，您可以切換至（預付）套件或訂閱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[！UICONTROL無法讀取影格大小：無法搜尋到1508。 /output/JLIADSA00137P0.mp3�：無效的引數。]</span> </p> </td> 
   <td> <p>例如，將檔案從MP3轉換為WAV時會擲回此錯誤。 請確定您選取了正確的區域，因為它會找到檔案的參照，而不只是正確的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL RuntimeError：] </p> <p><span style="font-weight: normal;">[！UICONTROL已超出最大重複次數。]</span> </p> </td> 
   <td> <p>找到對應的 [!DNL CloudConvert] 您的中的工作 [!DNL CloudConvert] 控制面板的工作清單，並檢查工作的持續時間：</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>此 [!DNL CloudConvert] &gt; [！UICONTROL轉換檔案]模組的逾時設為3分鐘。 如果工作的持續時間超過3分鐘(可能由於 [!DNL CloudConvert] 服務)，模組擲回上述錯誤。</p> <p>在此案例中，請考慮下列其中一個選項：</p> 
    <ul> 
     <li>啟用 <strong>[！UICONTROL允許儲存不完整的執行]</strong> 情境設定中的選項，用來儲存未完成的執行，以供稍後手動解決。 您可選擇將錯誤處理路由附加至 [!DNL CloudConvert] 包含[！UICONTROL Break]指示詞的模組，可自動解析未完成的執行。</li> 
     <li>停用 <strong>[！UICONTROL下載檔案]選項</strong> 在 [!DNL CloudConvert] &gt; [！UICONTROL轉換檔案]模組。 在此情況下，模組不會等待轉換結果。 若要取得轉換結果，請建立新情境並使用 [!DNL CloudConvert] &gt; [！UICONTROL新作業事件]觸發器。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 的工作流程範例 [!DNL CloudConvert] 聯結器

>[!INFO]
>
>**範例：** 將視訊從MOV轉換為MP4格式
>
>1. 造訪 [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. 按一下 **[!UICONTROL 選取檔案]** 並選擇您的範例MOV檔案。
>1. 按一下旁邊的下拉式清單 **[!UICONTROL 轉換為]** 並選擇 **[!UICONTROL MP4]**.
>
>1. 按一下 **[!UICONTROL 扳手]** 圖示。
>1. 視需要設定MP4壓縮設定。
>1. 按一下 **[!UICONTROL 轉換]**.
>1. 轉換完成後，請按一下 **[!UICONTROL 下載]**.
>1. 檢閱轉換後的影片。
>1. 重複步驟1至8，直到找到步驟5的最佳轉換設定。
>1. 造訪 [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. 選擇 **[!UICONTROL mov]** 的 **[!UICONTROL 輸入格式]** 欄位。
>
>1. 選擇 **[!UICONTROL mp4]** 的 **[!UICONTROL output_format]** 欄位。
>
>1. 所有可能的引數清單，例如video_codec、crf等。 將會出現。
>1. 在Workfront Fusion 2.0中插入 **[!UICONTROL CloudConvert]** > **[!UICONTROL 轉換檔案]** 模組。
>
>1. 開啟模組的設定。
>1. 設定模組，如下所示：
>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. 請務必在「轉換和引擎特定選項」欄位中納入所有設定：針對步驟5中的每個設定，找出步驟13中的對應引數及其對應值。
