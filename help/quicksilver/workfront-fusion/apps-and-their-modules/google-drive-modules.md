---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Google驅動器模組
description: 此 [!DNL Adobe Workfront Fusion Google Drive] 模組可讓您監視、搜尋、建立、更新、刪除及管理檔案、資料夾或共用磁碟 [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2908'
ht-degree: 0%

---

# [!DNL Google Drive] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Drive] 模組可讓您監視、搜尋、建立、更新、刪除及管理檔案、資料夾或共用磁碟 [!DNL Google Drive].

在 [!DNL Adobe Workfront Fusion] 案例中，您可以連結 [!DNL Google Drive] 帳戶至多個協力廠商應用程式和服務。

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
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## 連接 [!DNL Google Drive] to [!DNL Workfront Fusion]

如果您 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您需要在 [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 為了獲得 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼].

如需如何建立OAuth用戶端(和取得 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼])，請參閱 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

有關連接 [!DNL Google Drive] 帳戶 [!UICONTROL Workfront融合]，請參閱 [建立連線至 [!UICONTROL Adobe Workfront融合]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] 模組及其欄位

設定時 [!DNL Google Drive] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Google Drive] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

* [[!UICONTROL 監視資料夾中的檔案]](#watch-files-in-folder)
* [[!UICONTROL 監視所有檔案]](#watch-all-files)
* [[!UICONTROL 監視共用檔案]](#watch-shared-files)
* [[!UICONTROL 觀看留言]](#watch-comments)

#### [!UICONTROL 監視資料夾中的檔案]

在指定的資料夾中添加或修改檔案時檢索檔案詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL連接] </td>
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL選擇要監視的資料夾]</td>
    <td >在驅動器上選擇要監視檔案的資料夾。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL要監視的檔案]</td>
   <td> <p>選擇要監視的檔案類型。</p> 
    <ul> 
     <li>[!UICONTROL全部]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL轉換 [!DNL Google Documents] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Documents] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Spreadsheets] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Spreadsheets] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Slides] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Slides] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Drawings] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Drawings] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>選擇要監視新檔案和所有更改，還是僅監視新檔案。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL下載檔案的最大數量]</td>
    <td>設定 [!DNL Workfront Fusion] 將在一個週期中下載（每個案例執行的重複次數）。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視所有檔案]

在 [!DNL Google Drive] 已新增或修改。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL要監視的檔案]</td> 
   <td> <p>選擇要監視的檔案類型。</p> 
    <ul> 
     <li>[!UICONTROL全部]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL轉換 [!DNL Google Documents] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Documents] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Spreadsheets] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Spreadsheets] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Slides] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Slides] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Drawings] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Drawings] 到。</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>選擇要監視新檔案和所有更改，還是僅監視新檔案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL下載檔案的最大數量]</td> 
   <td>設定 [!DNL Workfront Fusion] 將在一個週期中下載（每個案例執行的重複次數）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視共用檔案]

將新檔案共用給您或更新現有共用檔案時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇要監視的資料夾]</td> 
   <td>選擇要監視檔案的共用資料夾。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL要監視的檔案]</td> 
   <td> <p>選擇要監視的檔案類型。</p> 
    <ul> 
     <li>[!UICONTROL全部]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL轉換 [!DNL Google Documents] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Documents] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Spreadsheets] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Spreadsheets] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Slides] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Slides] 到。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL轉換 [!DNL Google Drawings] 檔案格式]</td>
    <td>選擇要轉換的檔案格式 [!DNL Google Drawings] 到。</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>選擇要監視新檔案和所有更改，還是僅監視新檔案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL下載檔案的最大數量]</td> 
   <td>設定 [!DNL Workfront Fusion] 將在一個週期中下載（每個案例執行的重複次數）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看留言]

在選取的檔案上新增或修改註解時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案]</td> 
   <td>選擇要監視的檔案以獲取注釋。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>選擇您要查看所有更改還是僅查看新注釋</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回的注釋數上限]</td> 
   <td>設定留言數上限 [!DNL Workfront Fusion] 會在一個週期中傳回（每個案例執行的重複次數）。</td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 更新檔案]](#update-a-file)
* [[!UICONTROL 複製檔案]](#copy-a-file)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 將檔案/資料夾移至清除]](#move-a-filefolder-to-trash)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 搜索檔案/資料夾]](#search-for-filesfolders)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 取得分享連結]](#get-a-share-link)

#### [!UICONTROL 上傳檔案]

將檔案上傳至 [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>選取要上傳檔案的目標。</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target資料夾]</td> 
   <td>選取要上傳檔案的資料夾。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td>選取您要使用從上一個模組傳入的檔案，還是要手動對應檔案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案名]</td> 
   <td>選取檔案名稱。 如果在[!UICONTROL源檔案]欄位中選擇「[!UICONTROL映射]」，則此選項可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料]</td> 
   <td>選取您要上傳的資料檔案。 如果在[!UICONTROL源檔案]欄位中選擇「[!UICONTROL映射]」，則此選項可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題]</td> 
   <td>輸入新檔案的標題。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換檔案]</td> 
   <td>啟用此選項可讓模組將檔案轉換為對應的 [!DNL Google] 格式。</td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標]</td> 
   <td> <p>選取要上傳檔案的目標。</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL移動到資料夾]</td> 
   <td>如果要將檔案移到其他資料夾，請選擇要將檔案移入的資料夾。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td>映射要更新的檔案的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題]</td> 
   <td>輸入更新檔案的標題。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更改檔案內容]</td> 
   <td>選擇是否替換檔案的內容。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td>選取您要使用從上一個模組傳入的檔案，還是要手動對應檔案。 如果您選取在上一個欄位中變更檔案的內容，此欄位即可使用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案名]</td> 
   <td>選取檔案名稱。 如果在[!UICONTROL源檔案]欄位中選擇「[!UICONTROL映射]」，則此選項可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料]</td> 
   <td>選取您要上傳的資料檔案。 如果在[!UICONTROL源檔案]欄位中選擇「[!UICONTROL映射]」，則此選項可用。</td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標]</td> 
   <td> <p>選取要上傳檔案的目標。</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target資料夾]</td> 
   <td>選擇要複製的檔案所在的資料夾/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td>映射要更新的檔案的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL副本的名稱]</td> 
   <td>輸入新檔案的標題。 如果您不想變更原始檔案名稱，請將此欄位留空。</td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td>對應您要刪除之檔案的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將檔案/資料夾移至清除]

將檔案或資料夾移至垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Documents] 檔案格式]</td> 
   <td>選擇要轉換的檔案格式 [!DNL Google Documents] 到。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Spreadsheets] 檔案格式]</td> 
   <td>選擇要轉換的檔案格式 [!DNL Google Spreadsheets] 到。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Slides] 檔案格式]</td> 
   <td>選擇要轉換的檔案格式 [!DNL Google Slides] 到。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Drawings] 檔案格式]</td> 
   <td>選擇要轉換的檔案格式 [!DNL Google Drawings] 到。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td>映射要檢索的檔案的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索檔案/資料夾]

根據搜索標準搜索檔案或資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標]</td> 
   <td> <p>選擇要搜索的目標。</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL列出資料夾]</td> 
   <td>導航到要搜索檔案或資料夾的資料夾。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檢索]</td> 
   <td> <p> 選擇要搜索檔案、資料夾還是兩者。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL搜索]</p> </td> 
   <td> <p>選擇要執行的搜索類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL在檔案/資料夾名稱內搜索]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL查詢]</strong> </p> <p>輸入要搜索的檔案名或完整檔案名（包括尾碼）的一部分。</p> </li> 
       <li> <p><strong>[!UICONTROL搜索選項]</strong> </p> <p>選取您要搜尋確切的詞語，還是要搜尋包含搜尋詞的名稱。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL全文]搜索</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL查詢]</strong> </p> <p>輸入您要在 [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>輸入自定義搜索查詢</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL查詢]</strong> </p> <p>輸入自定義搜索查詢。 如需詳細資訊，請參閱本文的[!UICONTROL搜尋檔案]一節。</p> </li> 
       <li> <p><strong>將上述選取的資料夾新增至查詢</strong> </p> <p>搜索父集合中的資料夾。 這將查找直接位於上述所選資料夾中的所有檔案和資料夾。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回結果的最大數]</td> 
   <td>設定檔案或資料夾的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL即使模組未返回任何結果，仍繼續執行路由]</td> 
   <td>啟用此選項，以確保在模組未傳回任何結果時不會停止案例。</td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標]</td> 
   <td> <p>選取要上傳檔案的目標。</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新資料夾位置]</td> 
   <td>導覽至您要建立新資料夾的位置。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新資料夾的名稱]</td> 
   <td>輸入要建立的資料夾的名稱。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL共用資料夾]</td> 
   <td>如果要與任何具有[!UICONTROL共用]連結的人共用資料夾，請選擇此選項。 否則，共用連結僅適用於所有者。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得分享連結]

在Google驅動器中檢索檔案的共用連結。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">連接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td>對應您要取得共用連結之檔案的ID。</td> 
  </tr> 
 </tbody> 
</table>

## 疑難排解

### 無法上傳或更新檔案

上傳或更新檔案失敗時，有數種情況：

* 上傳的檔案太大，超過了您 [!DNL Google Drive] 計畫或超過 [!DNL Google Drive] 儲存限制。 您可以升級儲存計畫或刪除 [!DNL Google Drive] 服務。
* 要上傳檔案的所選資料夾已不存在。 情境停止，然後需要再次選取目標資料夾。

## 搜索檔案

在資料夾中的模組清單檔案中，您可以使用自己的查詢，該查詢由以下部分組成：

* **[!UICONTROL 欄位]**  — 要搜尋的檔案的屬性，例如屬性 `name` 檔案。

* **[!UICONTROL 運算元]**  — 對資料執行的測試以提供相符項目，例如 `contains`.

* **[!UICONTROL 值]**  — 測試的屬性內容，例如檔案名稱 `My cool document`.

將子句與連結組合 `and` 或 `or`，並否定查詢 `not`.

* [欄位](#fields)
* [值類型](#value-types)
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
   <th>值類型 </th> 
   <th>運算子</th> 
   <th> <p> 說明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>字串</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 檔案名稱。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>字串 </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> 檔案的全文，包括名稱、說明、內容和可索引文本。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> 字串</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 檔案的MIME類型。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> 日期<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 上次修改檔案的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> 日期<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 使用者上次檢視檔案的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>布林值 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> 檔案是否在垃圾桶中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>布林值 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>檔案是否有星號。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>集合 </td> 
   <td><code>in </code> </td> 
   <td> <p>[!UICONTROL parents]集合是否包含指定的ID。</p> </td> 
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
   <td> <p>有權讀取檔案的用戶。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>布林值 </td> 
   <td><code>=</code>, <code>!=</code></td> 
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

請考量下列關於這些欄位中運算子的事項：

* 此 `contains` 運算子僅執行前置詞匹配 `title`.

   例如，標題「HelloWorld」符合的 `title contains 'Hello'` 但不是 `title contains 'World'`.

* 此 `contains` 運算子只執行整個字串代號的匹配 `fullText`.

   例如，如果文檔的全文僅包含查詢的字串&quot;HelloWorld&quot; `fullText contains 'HelloWorld'` 傳回結果。 查詢，例如 `fullText contains 'Hello'` 不會在此情況中傳回結果。

* 此 `contains` 運算子會在精確的英數字字片語上比對（如果包含雙引號）。

   例如，若 `fullText` doc包含字串&quot;Hello there world&quot;，然後是查詢 `fullText contains '"Hello there"'` 返回結果，但查詢 `fullText contains '"Hello world"'` 不會。

   此外，由於搜尋是英數字元，若 `fullText` doc包含字串&quot;Hello_world&quot;，然後是查詢 `fullText contains '"Hello world"'` 傳回結果。

* 欄位 `type` 日期目前無法互相比較，只能與固定日期比較。

### 值類型

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>值類型</th> 
   <th> <p> 附註</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>字串 </td> 
   <td> <p>用單引號'括住。 使用逸出查詢中的單引號 <code>\'</code>，例如<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td> <p><code>true </code>或 <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td> <p>RFC 3339格式，預設時區為UTC，例如 <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
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
   <td> <p> 字串或布林值的內容等於其他內容。</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 字串或布林值的內容不等於其他。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> 日期早於其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> 日期早於或等於其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> 日期晚於其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> 日期晚於或等於其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>元素包含在集合中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>返回與兩個子句都匹配的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>返回與任一子句匹配的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>否定搜索子句。</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>集合包含與參數相符的元素。</p> </td> 
  </tr> 
 </tbody> 
</table>

對於複合子句，可以使用括弧將子句分組。 例如：
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` 此搜尋會傳回所有影像或視訊MIME類型，且上次修改時間為2012年6月4日之後的檔案。 因為 `and` 和 `or` 運算子會從左到右評估，不含括弧，上述範例只會傳回2012年6月4日之後修改的影像，但會傳回所有影片，甚至是2012年6月4日之前的影片。

### 範例

此頁面上的所有範例都顯示未編碼的 `<q>q</q>` 參數，其中 `title = 'hello'` 編碼為 `title+%3d+%27hello%27`. 用戶端程式庫會自動處理此編碼。

* 搜索名為「hello」的檔案

   <pre>title = 'hello'</pre>
* 使用資料夾特定的MIME類型搜索資料夾

   <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* 搜索非資料夾的檔案

   <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* 搜索名為包含&quot;hello&quot;和&quot;goodbye&quot;的檔案

   <pre>標題包含'hello'，而[!UICONTROL名稱]包含'goodbye'</pre>
* 搜索名稱不包含&quot;hello&quot;的檔案

   <pre>標題不包含'hello'</pre>
* 搜尋內容中包含&quot;hello&quot;字的檔案

   <pre>fullText包含'hello'</pre>
* 搜尋內容中不含「hello」字的檔案

   <pre>not fullText包含'hello'</pre>
* 搜尋內容中包含確切字句「hello world」的檔案

   <pre>fullText包含「hello world」的fullText包含「hello_world」</pre>
* 搜索包含&quot;\&quot;字元的查詢（如&quot;\authors&quot;）的檔案

   <pre>fullText包含「\\authors」</pre>
* 搜索用戶「test@example.org」可寫的檔案

   <pre>'test@example.org'in [!DNL writers]</pre>
* 搜尋ID `1234567` 在 `parents` 集合。 這會找到ID為的資料夾中直接存在的所有檔案和資料夾 `1234567`.

   <pre>[!UICONTROL父母]中的'1234567'</pre>
* 搜尋別名ID `appDataFolder` 在 `parents` 集合。 這會找到位於 [應用程式資料夾](https://developers.google.com/drive/api/v2/appdata).

   <pre>父項中的'appDataFolder'</pre>
* 搜索用戶「test@example.org」和「test2@example.org」可寫的檔案

   <pre>作家中的「test@example.org」和作家中的「test2@example.org」</pre>
* 搜尋垃圾桶中包含「重要」文字的檔案

   <pre>fullText包含'important'和trashed = true</pre>
* 搜尋2012年6月4日後修改的檔案

   <pre>modifiedDate &gt; '2012-06-04T12:00:00' //預設時區為UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* 搜索與授權用戶共用的檔案，名稱為「hello」

   <pre>sharedWithMe和title包含'hello'</pre>
* 搜尋含有 [自定義檔案屬性](https://developers.google.com/drive/api/v2/properties) 已命名 `additionalID` 值 `8e8aceg2af2ge72e78`.

   <pre>屬性有{ key='additionalID'和value='8e8aceg2af2ge72e78'和visibility='PRIVATE' }</pre>

本指南的來源為 [[!DNL Google Drive] 檔案](https://developers.google.com/drive/api/v2/search-shareddrives).
