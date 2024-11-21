---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google磁碟機模組
description: ' [!DNL Adobe Workfront Fusion Google Drive] 模組可讓您監視、搜尋、建立、更新、刪除及管理 [!DNL Google Drive]中的檔案、資料夾或共用磁碟機。'
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 0%

---

# [!DNL Google Drive]模組

[!DNL Adobe Workfront Fusion] [!DNL Google Drive]模組可讓您監視、搜尋、建立、更新、刪除及管理[!DNL Google Drive]中的檔案、資料夾或共用磁碟機。

在[!DNL Adobe Workfront Fusion]案例中，您可以將[!DNL Google Drive]帳戶連線至多個協力廠商應用程式和服務。

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

## Google Drive API資訊

Google磁碟機聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td> https://www.googleapis.com/drive/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v4.1.22</td> 
  </tr>
 </tbody> 
 </table>



## 正在連線[!DNL Google Drive]至[!DNL Workfront Fusion]

如果您是[!DNL @gmail.com]或[!DNL @googlemail.com]使用者，您必須在[the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project)上建立OAuth使用者端，才能取得[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼]。

如需如何建立OAuth使用者端（以及取得[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼]）的逐步指示，請參閱[使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 。

如需有關將您的[!DNL Google Drive]帳戶連線到[!UICONTROL Workfront Fusion]的指示，請參閱[建立與[!UICONTROL Adobe Workfront Fusion]的連線](../../workfront-fusion/connections/connect-to-fusion-general.md) — 基本指示

## [!DNL Google Drive]模組及其欄位

當您設定[!DNL Google Drive]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Google Drive]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)



* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

* [[!UICONTROL 在資料夾]中監視檔案](#watch-files-in-folder)
* [[!UICONTROL 觀看所有檔案]](#watch-all-files)
* [[!UICONTROL 觀看共用檔案]](#watch-shared-files)
* [[!UICONTROL 觀看註解]](#watch-comments)

#### [!UICONTROL 在資料夾]中監視檔案

在指定的資料夾中新增或修改檔案時，擷取檔案詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection] </td>
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL選取要監看的資料夾]</td>
    <td >選取您要在磁碟機上觀看檔案的資料夾。</td>
  </tr> 
  <tr> 
    <td>[！UICONTROL要觀看的檔案]</td>
   <td> <p>選取您要觀看的檔案型別。</p> 
    <ul> 
     <li>[！UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[！UICONTROL將[!DNL Google Documents]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Documents]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Spreadsheets]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Spreadsheets]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Slides]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Slides]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Drawings]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Drawings]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL手錶]</td>
    <td>選取您要監視新檔案與所有變更，還是隻監視新檔案。</td>
  </tr> 
  <tr> 
    <td>[！UICONTROL下載檔案數上限]</td>
    <td>設定[!DNL Workfront Fusion]在一個週期內下載的結果數目上限（每個案例執行的重複數目）。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看所有檔案]

新增或修改您[!DNL Google Drive]中的檔案時擷取檔案詳細資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL要觀看的檔案]</td> 
   <td> <p>選取您要觀看的檔案型別。</p> 
    <ul> 
     <li>[！UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[！UICONTROL將[!DNL Google Documents]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Documents]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Spreadsheets]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Spreadsheets]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Slides]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Slides]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Drawings]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Drawings]轉換成的檔案格式。</td>
  </tr>  
  <tr> 
   <td>[！UICONTROL手錶]</td> 
   <td>選取您要監視新檔案與所有變更，還是隻監視新檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL下載檔案數上限]</td> 
   <td>設定[!DNL Workfront Fusion]在一個週期內下載的結果數目上限（每個案例執行的重複數目）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看共用檔案]

在您共用新檔案或更新現有共用檔案時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取要監看的資料夾]</td> 
   <td>選取您想要監看檔案的共用資料夾。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL要觀看的檔案]</td> 
   <td> <p>選取您要觀看的檔案型別。</p> 
    <ul> 
     <li>[！UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[！UICONTROL將[!DNL Google Documents]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Documents]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Spreadsheets]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Spreadsheets]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Slides]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Slides]轉換成的檔案格式。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL將[!DNL Google Drawings]個檔案轉換為格式]</td>
    <td>選取您要將[!DNL Google Drawings]轉換成的檔案格式。</td>
  </tr> 
  <tr> 
   <td>[！UICONTROL手錶]</td> 
   <td>選取您要監視新檔案與所有變更，還是隻監視新檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL下載檔案數上限]</td> 
   <td>設定[!DNL Workfront Fusion]在一個週期內下載的結果數目上限（每個案例執行的重複數目）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看註解]

在選取的檔案上新增或修改註解時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案]</td> 
   <td>選取您要觀看註解的檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL手錶]</td> 
   <td>選取您是要監視所有變更，還是隻監視新註解</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回評論的最大數量]</td> 
   <td>設定[!DNL Workfront Fusion]在一個週期內傳回的評論數目上限（每個案例執行的重複數目）。</td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 更新檔案]](#update-a-file)
* [[!UICONTROL 複製檔案]](#copy-a-file)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 將檔案/資料夾移至垃圾桶]](#move-a-filefolder-to-trash)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 搜尋檔案/資料夾]](#search-for-filesfolders)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 取得共用連結]](#get-a-share-link)

#### [!UICONTROL 上傳檔案]

上傳檔案至您的[!DNL Google Drive]。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>選取您要上傳檔案的目的地。</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目標資料夾]</td> 
   <td>選取您要上傳檔案的資料夾。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source檔案]</td> 
   <td>選取您要使用從先前模組傳入的檔案，或是要手動對應檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案名稱]</td> 
   <td>選取檔案名稱。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對映]」，則此選項可供使用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料]</td> 
   <td>選取您要上傳的資料檔案。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對映]」，則此選項可供使用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標題]</td> 
   <td>輸入新檔案的標題。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換檔案]</td> 
   <td>啟用此選項可讓模組將檔案轉換為對應的[!DNL Google]格式。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新檔案]

更新檔案的中繼資料或內容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目的地]</td> 
   <td> <p>選取您要上傳檔案的目的地。</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL移至資料夾]</td> 
   <td>如果要將檔案移動到其他資料夾，請選取要將檔案移動到其中的資料夾。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td>對應您要更新的檔案ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標題]</td> 
   <td>輸入更新檔案的標題。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL變更檔案內容]</td> 
   <td>選取是否要取代檔案的內容。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source檔案]</td> 
   <td>選取您要使用從先前模組傳入的檔案，或是要手動對應檔案。 如果您在上一個欄位中選擇要變更檔案的內容，則可使用此欄位。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案名稱]</td> 
   <td>選取檔案名稱。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對映]」，則此選項可供使用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料]</td> 
   <td>選取您要上傳的資料檔案。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對映]」，則此選項可供使用。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製檔案]

將檔案複製到新位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目的地]</td> 
   <td> <p>選取您要上傳檔案的目的地。</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目標資料夾]</td> 
   <td>選取您要複製的檔案所在的資料夾/</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td>對應您要更新的檔案ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL副本的名稱]</td> 
   <td>輸入新檔案的標題。 如果您不想變更原始檔案名稱，請將此欄位保留空白。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

永久刪除檔案或資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td>對應您要刪除的檔案ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將檔案/資料夾移至垃圾桶]

將檔案或資料夾移至垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td>對應您要移至垃圾桶的檔案ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

擷取具有指定ID的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL將[!DNL Google Documents]個檔案轉換為格式]</td> 
   <td>選取您要將[!DNL Google Documents]轉換成的檔案格式。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL將[!DNL Google Spreadsheets]個檔案轉換為格式]</td> 
   <td>選取您要將[!DNL Google Spreadsheets]轉換成的檔案格式。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL將[!DNL Google Slides]個檔案轉換為格式]</td> 
   <td>選取您要將[!DNL Google Slides]轉換成的檔案格式。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL將[!DNL Google Drawings]個檔案轉換為格式]</td> 
   <td>選取您要將[!DNL Google Drawings]轉換成的檔案格式。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td>對應您要擷取的檔案ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋檔案/資料夾]

根據搜尋條件搜尋檔案或資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目的地]</td> 
   <td> <p>選取您要搜尋的目的地。</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL列出資料夾]</td> 
   <td>瀏覽至您要搜尋檔案或資料夾的資料夾。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Retrieve]</td> 
   <td> <p> 選取您要搜尋檔案、資料夾或兩者。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL搜尋]</p> </td> 
   <td> <p>選取您要執行的搜尋型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL在檔案/資料夾名稱內搜尋]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查詢]</strong> </p> <p>輸入要搜尋的部分檔案名稱或完整檔案名稱（包括尾碼）。</p> </li> 
       <li> <p><strong>[！UICONTROL搜尋選項]</strong> </p> <p>選取您要搜尋完全相同的字詞，或是要搜尋包含搜尋字詞的名稱。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL Fulltext]搜尋</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查詢]</strong> </p> <p>在[!DNL Google Drive]中輸入您要搜尋的任何搜尋字詞。</p> </li> 
      </ul> </li> 
     <li> <p><strong>輸入自訂搜尋查詢</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查詢]</strong> </p> <p>輸入自訂搜尋查詢。 如需更多詳細資料，請參閱本文的[！UICONTROL搜尋檔案]一節。</p> </li> 
       <li> <p><strong>將上面選取的資料夾新增到查詢</strong> </p> <p>搜尋父項集合中的資料夾。 這會尋找直接位於上方所選資料夾中的所有檔案和資料夾。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回結果的最大數目]</td> 
   <td>設定[!DNL Workfront Fusion]在一個執行週期內傳回的檔案或資料夾數目上限。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL即使模組未傳回任何結果，仍繼續執行路由]</td> 
   <td>啟用此選項可確保在模組未傳回任何結果時不會停止此案例。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

在指定位置中建立資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目的地]</td> 
   <td> <p>選取您要上傳檔案的目的地。</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新資料夾位置]</td> 
   <td>導覽至您要建立新資料夾的位置。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新資料夾的名稱]</td> 
   <td>輸入您正在建立的資料夾名稱。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL共用資料夾]</td> 
   <td>如果您想要與任何具有[！UICONTROL共用]連結的人共用資料夾，請選取此選項。 否則，共用連結僅供擁有者使用。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得共用連結]

擷取Google Drive中檔案的共用連結。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Drive]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">將[!DNL Google Drive]連線到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td>對應您要取得共用連結的檔案ID。</td> 
  </tr> 
 </tbody> 
</table>

## 疑難排解

### 無法上傳或更新檔案

上傳或更新檔案失敗時有幾種情況：

* 上傳的檔案太大，超過您的[!DNL Google Drive]計畫允許的最大檔案大小限制，或者您已超過[!DNL Google Drive]儲存空間限制。 您可以升級儲存空間方案，或從[!DNL Google Drive]服務中刪除現有檔案。
* 要上傳檔案到的所選資料夾已不存在。 此案例會停止，然後需要再次選取目標資料夾。

## 搜尋檔案

在模組「列出資料夾中的檔案」中，您可以使用自己的查詢，該查詢由以下部分組成：

* **[!UICONTROL 欄位]** — 正在搜尋之檔案的屬性，例如，檔案的屬性`name`。

* **[!UICONTROL 運運算元]** — 對資料執行的測試，以提供相符專案，例如`contains`。

* **[!UICONTROL 值]** — 測試之屬性的內容，例如，檔案`My cool document`的名稱。

將子句與結合項`and`或`or`結合，並使用`not`否定查詢。

* [欄位](#fields)
* [值型別](#value-types)
* [運算子](#operators)
* [範例](#examples)

### 欄位

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>欄位 </th> 
   <th>值型別 </th> 
   <th>運算子</th> 
   <th> <p> 說明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>字串</td> 
   <td><code>contains</code><sup>1</sup>，<code>=</code>， <code>!=</code></td> 
   <td> <p> 檔案的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>字串 </td> 
   <td><code>contains</code><sup>2， 3</sup> </td> 
   <td> <p> 檔案的全文，包括名稱、說明、內容和可建立索引的文字。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> 字串</td> 
   <td><code>contains</code>，<code>=</code>， <code>!=</code></td> 
   <td> <p> 檔案的MIME型別。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> 日期<sup>4</sup></td> 
   <td><code> &lt;=</code>，<code>&lt;</code>，<code>=</code>，<code>!=</code>，<code>></code>， <code>>=</code></td> 
   <td> <p> 上次修改檔案的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> 日期<sup>4</sup></td> 
   <td><code>&lt;=</code>，<code>&lt;</code>，<code>=</code>，<code>!=</code>，<code>></code>， <code>>=</code></td> 
   <td> <p> 使用者上次檢視檔案的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>布林值 </td> 
   <td><code>=</code>， <code>!=</code></td> 
   <td> <p> 檔案是否在垃圾桶中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>布林值 </td> 
   <td><code>=</code>， <code>!=</code></td> 
   <td> <p>是否啟動檔案。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>集合 </td> 
   <td><code>in </code> </td> 
   <td> <p>[！UICONTROL parents]集合是否包含指定的ID。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>集合 </td> 
   <td><code>in </code> </td> 
   <td> <p>擁有檔案的使用者。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>集合 </td> 
   <td><code>in </code> </td> 
   <td> <p>有權修改檔案的使用者。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>集合 </td> 
   <td><code>in </code> </td> 
   <td> <p>有權讀取檔案的使用者。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>布林值 </td> 
   <td><code>=</code>， <code>!=</code></td> 
   <td> <p> 使用者「與我共用」集合中的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>集合</td> 
   <td><code>has </code> </td> 
   <td> <p> 公用自訂檔案屬性。</p> </td> 
  </tr> 
 </tbody> 
</table>

請考量下列這些欄位中的運運算元：

* `contains`運運算元只會執行`title`的前置詞比對。

  例如，標題「HelloWorld」符合`title contains 'Hello'`，但不符合`title contains 'World'`。

* `contains`運運算元只對`fullText`的整個字串權杖執行比對。

  例如，如果檔案全文包含字串「HelloWorld」，則只有查詢`fullText contains 'HelloWorld'`會傳回結果。 在此案例中，`fullText contains 'Hello'`之類的查詢不會傳回結果。

* 如果`contains`運運算元由雙引號包圍，則其符合的是完整的英數字元片語。

  例如，如果檔案的`fullText`包含「Hello there world」字串，則查詢`fullText contains '"Hello there"'`會傳回結果，但查詢`fullText contains '"Hello world"'`不會傳回。

  此外，因為搜尋是英數字元，如果檔案的`fullText`包含字串「Hello_world」，則查詢`fullText contains '"Hello world"'`會傳回結果。

* `type`日期的欄位目前無法相互比較，只能比較常數日期。

### 值型別

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>值型別</th> 
   <th> <p> 附註</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>字串 </td> 
   <td> <p>以單引號括住'。 使用<code>\'</code> （例如<code> 'Valentine\'s Day'</code>）的查詢中逸出單引號。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td> <p><code>true </code>或<code>false</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td> <p>RFC 3339格式，預設時區為UTC，例如<code>2012-06-04T12:00:00-08:00</code>。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 運算子

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>運算子 </th> 
   <th> <p>附註</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>一個字串的內容存在於另一個字串中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> 字串或布林值的內容等於另一個字串。</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 字串或布林值的內容不等於其他字串。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> 日期早於另一個日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> 日期早於或等於另一個日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> 日期晚於另一個日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> 日期晚於或等於另一個日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>元素包含在集合中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>傳回符合兩個子句的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>傳回符合任一子句的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>讓搜尋子句無效。</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>收集包含符合引數的要素。</p> </td> 
  </tr> 
 </tbody> 
</table>

對於複合子句，您可以使用括弧將子句組合在一起。 例如：
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')`此搜尋會傳回影像或視訊MIME型別的所有檔案，其上次修改是在2012年6月4日之後。 由於`and`和`or`運運算元是從左到右評估，不含括弧，因此上述範例只會傳回2012年6月4日之後修改的影像，但會傳回所有視訊，甚至是2012年6月4日之前的視訊。

### 範例

本頁的所有範例皆顯示未編碼的`<q>q</q>`引數，其中`title = 'hello'`編碼為`title+%3d+%27hello%27`。 使用者端程式庫會自動處理此編碼。

* 搜尋名稱為「hello」的檔案
  <pre>標題= 'hello'</pre>
* 使用檔案夾特定的MIME型別來搜尋檔案夾
  <pre>mimetype = 'application/vnd.google-apps.folder'</pre>
* 搜尋不是資料夾的檔案
  <pre>mimeType ！= 'application/vnd.google-apps.folder'</pre>
* 搜尋名稱包含「hello」和「goodbye」字樣的檔案
  <pre>標題包含'hello'，[！UICONTROL名稱]包含'goodbye'</pre>
* 搜尋名稱不包含「hello」字樣的檔案
  <pre>標題不包含'hello'</pre>
* 搜尋內容中包含「hello」字樣的檔案
  <pre>fullText包含'hello'</pre>
* 搜尋內容中不含單字「hello」的檔案
  <pre>非fullText包含'hello'</pre>
* 搜尋包含內容中確切片語「hello world」的檔案
  <pre>fullText包含'"hello world"'fullText包含'"hello_world"'</pre>
* 使用包含「\」字元的查詢來搜尋檔案（例如「\authors」）
  <pre>fullText包含'\\authors'</pre>
* 搜尋使用者`test@example.org`可寫入的檔案
  <pre>中的'test@example.org' [!DNL writers]</pre>
* 搜尋`parents`集合中的識別碼`1234567`。 這會尋找直接位於識別碼為`1234567`的資料夾中的所有檔案與資料夾。
  <pre>[！UICONTROL父項]中的'1234567'</pre>
* 在`parents`集合中搜尋別名識別碼`appDataFolder`。 這會尋找位於[應用程式資料資料夾](https://developers.google.com/drive/api/v2/appdata)下方的全部檔案和資料夾。
  <pre>父級中的「appDataFolder」</pre>
* 搜尋使用者`test@example.org`和`test2@example.org`可寫入的檔案
  <pre>writer中的「test@example.org」及writer中的「test2@example.org」</pre>
* 搜尋垃圾桶內包含「重要」文字的檔案
  <pre>fullText包含'important'且true = true</pre>
* 搜尋在2012年6月4日之後修改的檔案
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' //預設時區為UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* 搜尋與授權使用者共用的檔案，其名稱中包含「hello」
  <pre>sharedWithMe且標題包含「hello」</pre>
* 搜尋具有名為`additionalID`且值為`8e8aceg2af2ge72e78`的[自訂檔案屬性](https://developers.google.com/drive/api/v2/properties)的檔案。
  <pre>屬性有{ key='additionalID'和value='8e8aceg2af2ge72e78'和visibility='PRIVATE' }</pre>

本指南的Source為[[!DNL Google Drive] 檔案](https://developers.google.com/drive/api/v2/search-shareddrives)。
