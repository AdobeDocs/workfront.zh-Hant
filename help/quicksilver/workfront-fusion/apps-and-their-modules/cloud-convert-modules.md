---
title: CloudConvert模組
description: CloudConvert模組
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2993'
ht-degree: 0%

---

# [!DNL CloudConvert] 模組

在Adobe Workfront Fusion案例中，您可以自動執行使用CloudConvert的工作流程，並將其連接至多個協力廠商應用程式和服務。 此 [!DNL CloudConvert] 模組可讓您監視和管理作業、任務，以及匯入和匯出 [!DNL CloudConvert] 帳戶。

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

## Connect [!DNL CloudConvert] to [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，您必須向 [!DNL CloudConvert] 帳戶。

1. 登入 [!DNL CloudConvert] 帳戶，並開啟 [!UICONTROL 控制面板].
1. 開啟 **[!UICONTROL 授權] > [!UICONTROL API金鑰]** 區段。
1. 按一下 **[!UICONTROL 建立新API金鑰]**.
1. 輸入API密鑰的名稱，啟用您要使用的範圍，然後按一下 **[!UICONTROL 建立]**.
1. 複製提供的代號，並將其儲存在安全的位置。
1. 在 [!DNL Workfront Fusion]，開始建立案例並開啟 [!DNL CloudConvert] 模組 **[!UICONTROL 建立連線]** 對話框。

   如需指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 輸入您在步驟5中儲存的代號，然後按一下 **[!UICONTROL 繼續]** 建立連接。

## [!DNL CloudConvert] 模組及其欄位 {#cloudconvert-modules-and-their-fields}

設定時 [!DNL CloudConvert] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL CloudConvert] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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

此動作模組會擷取指定的網站，並將其儲存為PDF、JPG或PNG格式。

您可指定網站的URL和其他資訊，例如您要儲存資訊的位置。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入要擷取的網站URL。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出格式] </td> 
   <td>選擇要以PNG、JPG或PDF格式保存捕獲的網站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名] </td> 
   <td>輸入目標輸出檔案的檔案名（包括副檔名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題] </td> 
   <td> <p>（選用）定義請求標題。 </p> <p>例如，當指定的URL需要授權時，這個方法就很實用。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL轉換和引擎特定選項] </p> </td> 
   <td>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 檔案 <code>input_format</code> 和 <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下載檔案] </td> 
   <td> <p>如果您也想在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 轉換檔案]

將檔案轉換為選定的輸出格式。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案]</td> 
   <td>選取是否要使用 [!DNL Workfront Fusion] 或提供要上傳檔案的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上載檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL從URL導入檔案]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>輸入要轉換的檔案的URL。</p> </li> 
     <li> <p><strong>[!UICONTROL標題]</strong></p> <p>定義請求標題（選用）。 例如，當指定的URL需要授權時，這個方法就很實用。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL格式]</td> 
   <td>選擇是否要指定要轉換的檔案的輸入格式。 如果未指定，則使用輸入檔案的副檔名作為輸入格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>選取檔案的目前格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL輸出格式]</td> 
   <td>選擇要將檔案轉換為的目標檔案格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td>為目標輸出檔案選擇檔案名（包括副檔名）。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL轉換和引擎特定選項] </p> </td> 
   <td>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 檔案 <code>input_format</code> 和 <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL下載檔案] </td> 
   <td> <p>如果您也想在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立封存]

可讓您將一或多個檔案新增至ZIP、RAR、7Z、TAR、TAR.GZ或TAR.BZ2封存。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL輸入檔案]</p> </td> 
   <td> <p>指定要添加到存檔的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上載檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL從URL匯入檔案]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>輸入要存檔的檔案的URL。</p> <p><strong>[!UICONTROL標題]</strong> </p> <p>定義請求標題（選用）。 例如，當指定的URL需要授權時，這個方法就很實用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出格式]</td> 
   <td> <p> 選取封存檔案的目標格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td> <p> 輸入目標輸出檔案的檔案名（包括副檔名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL轉換和引擎特定選項] </td> 
   <td> <p>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 檔案 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下載檔案]</td> 
   <td> <p>如果您也想在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 合併檔案]

將至少兩個檔案合併為一個PDF。 如果輸入檔案不是PDF，則會自動轉換為PDF。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL輸入檔案]</p> </td> 
   <td> <p>指定要合併的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上載檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL從URL匯入檔案]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>輸入要存檔的檔案的URL。</p> <p><strong>[!UICONTROL標題]</strong> </p> <p>定義請求標題（選用）。 例如，當指定的URL需要授權時，這個方法就很實用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出格式]</td> 
   <td> <p> 選取合併檔案的目標格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td> <p> 輸入目標輸出檔案的檔案名（包括副檔名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL轉換和引擎特定選項] </td> 
   <td> <p>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 檔案 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下載檔案]</td> 
   <td> <p>如果您也想在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 最佳化檔案]

此動作模組會以PDF、PNG或JPG格式來最佳化和壓縮檔案。

可指定檔案以及用於優化和儲存該檔案的參數。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案]</td> 
   <td>選取您要使用Workfront Fusion上傳檔案，還是提供要上傳檔案的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL上載檔案]</p> </td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL從URL匯入檔案] </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>:輸入要轉換的檔案的URL。</li> 
     <li><strong>[!UICONTROL標題]</strong>:（選用）定義請求標題。 例如，當指定的URL需要授權時，這個方法就很實用。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL針對]的優化 </td> 
   <td> <p>根據特定目標需求選取最佳化設定檔。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Web]</strong>:網頁最佳化（預設）</p> 
      <ul> 
       <li>為Web刪除冗餘和不必要的資料</li> 
       <li>下採樣、剪輯和智慧地壓縮影像</li> 
       <li>合併字型和子集字型</li> 
       <li>將顏色轉換為RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL打印]</strong>:打印優化</p> 
      <ul> 
       <li> <p>移除用於打印的冗餘和不必要的資料</p> </li> 
       <li> <p>下採樣、剪輯和智慧地壓縮影像</p> </li> 
       <li> <p>合併字型和子集字型</p> </li> 
       <li> <p>將顏色轉換為CMYK</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL存檔]</strong>:針對歸檔目的而優化</p> 
      <ul> 
       <li> <p>移除備援和不必要的資料以進行封存</p> </li> 
       <li> <p>智慧地壓縮影像</p> </li> 
       <li> <p>合併字型和子集字型</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL掃描的影像]</strong>:掃描影像的最佳化</p> 
      <ul> 
       <li> <p>針對主要由光柵影像組成的PDF而優化的配置檔案</p> </li> 
       <li> <p>壓縮影像而不顯著降低視覺質量</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL最大尺寸縮減]</strong>:最大尺寸減小的優化</p> 
      <ul> 
       <li> <p>使用最大可能的壓縮</p> </li> 
       <li> <p>可能會降低視覺品質</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入格式] </td> 
   <td>選取要最佳化的輸入檔案格式。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td> <p>輸入目標輸出檔案的檔案名（包括副檔名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL轉換和引擎特定選項]</td> 
   <td> <p>指定轉換和引擎特定選項。 若要檢視可用選項，請參閱 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 檔案 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下載檔案]</td> 
   <td> <p>如果您也想在模組的輸出中包含檔案資料，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 工作

* [[!UICONTROL 建立作業（進階）]](#create-a-job-advanced)
* [[!UICONTROL 新作業事件]](#new-job-event)
* [[!UICONTROL 清單作業]](#list-jobs)
* [[!UICONTROL 找工作]](#get-a-job)
* [[!UICONTROL 刪除作業]](#delete-a-job)

#### [!UICONTROL 建立作業（進階）]

此模組會建立作業。 作業可以是 [!UICONTROL 名稱] 欄位，並使用 [!UICONTROL 輸入] 欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案]</td> 
   <td> <p>選取是否要使用 [!DNL Workfront Fusion]，或提供要上傳檔案的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上載檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL從URL導入檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>:輸入要處理的檔案的URL。</li> 
     <li><strong>[!UICONTROL標題]</strong>:（選用）定義請求標題。 例如，當指定的URL需要授權時，這個方法就很實用。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL任務]</p> </td> 
   <td> <p>添加將在作業內執行的任務。</p> <p>請在相應部分中查找操作欄位的說明。</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[!UICONTROL轉換檔案]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[!UICONTROL捕獲網站]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[!UICONTROL優化檔案]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[!UICONTROL建立存檔]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[!UICONTROL合併檔案]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL執行命令]</strong> </p> <p>有關執行命令的詳細資訊，請參見 <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] API檔案</a>.</p> </li> 
     <li> <p><strong>[!UICONTROL將檔案導出到臨時URL]</strong> </p> <p> 指定任務名和輸入任務名（例如轉換）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤] </td> 
   <td> <p>輸入標籤。 標籤是用於標識作業的任意字串。 它們沒有任何作用，可用來將工作與ID建立關聯。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除作業]

此模組會刪除作業，包括所有任務和資料。

>[!NOTE]
>
>作業在結束後24小時自動刪除。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL作業ID]</td> 
   <td> <p>輸入或映射要刪除的作業的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 找工作]

此模組會擷取工作詳細資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL作業ID]</td> 
   <td> <p>輸入或映射要檢索有關詳細資訊的作業的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單作業]

此模組會擷取已在您帳戶中執行的所有作業。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL狀態] </td> 
   <td> <p>選擇要按篩選返回的作業的作業狀態。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>設定在一個執行週期期間，Workfront Fusion 2.0將傳回的作業數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新作業事件]

在帳戶或任務中建立、完成或失敗時觸發。

>[!NOTE]
>
>* 由 [!UICONTROL 建立作業（進階）] 模組包含 *幾個* 任務。
>* 此 [!UICONTROL 新作業事件] 觸發時 *個別* 任務已建立、已完成或已失敗。
>


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook名稱]</td> 
   <td>輸入Webhook名稱。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出格式] </td> 
   <td>選擇要以PNG、JPG或PDF格式保存捕獲的網站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件]</td> 
   <td>選擇在建立作業或任務、完成或失敗時觸發模組。</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 如果使用陣列聚合器（例如，您有許多不同格式的檔案要轉換），請使用 **[!UICONTROL 我不知道輸入格式]** 選項 [!UICONTROL 添加任務] 對話框。 否則會傳回錯誤。
>* 連結作業內的任務（名稱>輸入、名稱>輸入、..）:
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### 任務

* [[!UICONTROL 獲取任務]](#get-a-task)
* [[!UICONTROL 下載檔案]](#download-a-file)
* [[!UICONTROL 清單任務]](#list-tasks)
* [[!UICONTROL 重試任務]](#retry-a-task)
* [[!UICONTROL 取消任務]](#cancel-a-task)
* [[!UICONTROL 刪除任務]](#delete-a-task)

#### [!UICONTROL 取消任務]

此模組會取消狀態為等待或處理的任務。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任務ID]</td> 
   <td> <p> 輸入或映射要取消的任務的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除任務]

刪除任務，包括所有資料。

>[!NOTE]
>
>任務在結束後24小時自動刪除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任務ID]</td> 
   <td> <p> 輸入（映射）要刪除的任務的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此模組從指定任務中檢索檔案名和檔案資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任務ID]</td> 
   <td> <p> 輸入或映射要從下載檔案的任務的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 獲取任務]

此模組將檢索任務詳細資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任務ID]</td> 
   <td> <p>輸入或映射要檢索有關詳細資訊的任務的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單任務]

此模組會根據篩選設定，擷取您帳戶中的所有工作。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL狀態] </td> 
   <td> <p>選擇任務狀態以按篩選返回的任務。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL作業ID] </td> 
   <td> <p>輸入或映射作業ID以僅返回指定作業內的任務。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL操作] </td> 
   <td> <p>輸入操作類型，以僅返回具有指定操作的任務。 </p> <p>注意：使用[!UICONTROL List Possible Operations]模組檢索操作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重試任務]

此模組會根據另一個任務的設定（裝載）建立新任務。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任務ID]</td> 
   <td> <p> 輸入或映射要建立新任務的任務ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 獲取我的資訊]](#get-my-info)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL 獲取我的資訊]

擷取目前使用者的已驗證帳戶詳細資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL CloudConvert] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connect [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關將[Fusion App]帳戶連接到Workfront Fusion的說明，請參見 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>輸入相對於的路徑 <code>https://api.cloudconvert.com/</code>. 例如： <code>/v2/tasks</code></p> <p>如需可用端點的清單，請參閱 <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] API v2檔案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式，新增API呼叫的內文內容。使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**範例：** 清單任務

下列API呼叫會傳回CloudFront帳戶的所有工作：

URL: `/v2/tasks`

方法: `GET`

![](assets/cloudconvert-api-example-input.png)

如需搜尋的相符項目，請在模組的「輸出」下方找到 [!UICONTROL 捆綁] > [!UICONTROL 主體] > [!UICONTROL 資料].

在我們的範例中，傳回6個工作：

![](assets/cloudconvert-api-example-output.png)

## 疑難排解 {#troubleshooting}

請參閱下表，了解可能的錯誤及其解決方案：

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
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL輸出檔案大小超過了您的方案允許的限制。]</span> </p> </td> 
   <td> <p>請參閱檔案大小限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL您已超過最大轉換時間。]</span> </p> </td> 
   <td> <p>免費 [!DNL CloudConvert] 計畫每天提供25分鐘轉換。 如果您的使用量超過免費計畫的限制，您可以切換至（預付）套件或訂閱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL無法讀取幀大小：無法查找1508。 �/output/JLIADSA00137P0.mp3:參數無效。]</span> </p> </td> 
   <td> <p>例如，將檔案從MP3轉換為WAV時，會擲回此錯誤。 請確定您已選取正確的區域，因為它會找到檔案的參考，而不只是正確的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL RuntimeError:] </p> <p><span style="font-weight: normal;">[!UICONTROL超過的重複數上限。]</span> </p> </td> 
   <td> <p>找出對應的 [!DNL CloudConvert] 工作 [!DNL CloudConvert] 控制面板的作業清單，並檢查作業的持續時間：</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>此 [!DNL CloudConvert] &gt; [!UICONTROL轉換檔案]模組的逾時設為3分鐘。 如果工作的持續時間超過3分鐘(可能是因為 [!DNL CloudConvert] 服務)，模組會擲回上述錯誤。</p> <p>在此案例中，請考量下列其中一個選項：</p> 
    <ul> 
     <li>啟用 <strong>[!UICONTROL允許儲存不完整的執行]</strong> 選項來儲存不完整的執行，以供稍後手動解析。 （可選）您可以將錯誤處理路由附加到 [!DNL CloudConvert] 模組，使用[!UICONTROL Break]指令自動解析不完整的執行。</li> 
     <li>停用 <strong>[!UICONTROL下載檔案]選項</strong> 在 [!DNL CloudConvert] &gt; [!UICONTROL轉換檔案]模組。 在此情況下，模組不會等待轉換結果。 若要取得轉換結果，請建立新案例並使用 [!DNL CloudConvert] &gt; [!UICONTROL新建作業事件]觸發器。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 工作流程範例 [!DNL CloudConvert] 連接器

>[!INFO]
>
>**範例：** 將視訊從MOV轉換為MP4格式
>
>1. 瀏覽 [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. 按一下 **[!UICONTROL 選擇檔案]** 並選擇示例MOV檔案。
>1. 按一下旁邊的下拉式清單 **[!UICONTROL 轉換為]** 選擇 **[!UICONTROL MP4]**.
>
>1. 按一下 **[!UICONTROL 扳手]** 表徵圖。
>1. 視需要配置MP4壓縮設定。
>1. 按一下 **[!UICONTROL 轉換]**.
>1. 轉換完成後，按一下 **[!UICONTROL 下載]**.
>1. 檢閱轉換的影片。
>1. 重複步驟1到8，直到找到步驟5的最佳轉換設定為止。
>1. 瀏覽 [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. 選擇 **[!UICONTROL mov]** 針對 **[!UICONTROL input_format]** 欄位。
>
>1. 選擇 **[!UICONTROL mp4]** 針對 **[!UICONTROL output_format]** 欄位。
>
>1. 所有可能參數（如video_codec、crf等）的清單。 即會出現。
>1. 在Workfront Fusion 2.0中，插入 **[!UICONTROL CloudConvert]** > **[!UICONTROL 轉換檔案]** 模組。
>
>1. 開啟模組的設定。
>1. 設定模組，如下所示：

>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. 請務必在「轉換」和「引擎特定選項」欄位中包含所有設定：對於步驟5中的每個設定，找出步驟13中對應的參數及其對應值。

