---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google磁碟機模組
description: 此 [!DNL Adobe Workfront Fusion Google Drive] 模組可讓您監視、搜尋、建立、更新、刪除和管理您的檔案、資料夾或共用磁碟機。 [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2956'
ht-degree: 0%

---

# [!DNL Google Drive] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Drive] 模組可讓您監視、搜尋、建立、更新、刪除和管理您的檔案、資料夾或共用磁碟機。 [!DNL Google Drive].

在 [!DNL Adobe Workfront Fusion] 情境，您可以連線至 [!DNL Google Drive] 帳戶至多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## 正在連線 [!DNL Google Drive] 至 [!DNL Workfront Fusion]

如果您是 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您需要建立OAuth使用者端的使用者 [此 [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 為了取得 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼].

如需如何建立OAuth使用者端（和取得）的逐步指示 [!UICONTROL 使用者端ID] 和 [!UICONTROL 使用者端密碼])，請參閱 [Connect [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!UICONTROL Workfront Fusion]，請參閱 [建立與的連線 [!UICONTROL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] 模組及其欄位

當您設定 [!DNL Google Drive] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Google Drive] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

* [[!UICONTROL 監看資料夾中的檔案]](#watch-files-in-folder)
* [[!UICONTROL 觀看所有檔案]](#watch-all-files)
* [[!UICONTROL 觀看共用檔案]](#watch-shared-files)
* [[!UICONTROL 觀看評論]](#watch-comments)

#### [!UICONTROL 監看資料夾中的檔案]

在指定的資料夾中新增或修改檔案時擷取檔案詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL連線] </td>
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL選取要監視的資料夾]</td>
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
    <td >[！UICONTROL轉換 [!DNL Google Documents] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Documents] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Spreadsheets] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Spreadsheets] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Slides] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Slides] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Drawings] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Drawings] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL監視]</td>
    <td>選取您要觀看新檔案與所有變更，還是隻觀看新檔案。</td>
  </tr> 
  <tr> 
    <td>[！UICONTROL下載檔案數上限]</td>
    <td>設定符合以下條件的最大結果數量： [!DNL Workfront Fusion] 會在一個週期內下載（每個案例執行的重複次數）。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看所有檔案]

當檔案位於以下位置時擷取檔案詳細資訊： [!DNL Google Drive] 新增或修改。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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
    <td >[！UICONTROL轉換 [!DNL Google Documents] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Documents] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Spreadsheets] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Spreadsheets] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Slides] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Slides] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Drawings] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Drawings] 至。</td>
  </tr>  
  <tr> 
   <td>[！UICONTROL監視]</td> 
   <td>選取您要觀看新檔案與所有變更，還是隻觀看新檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL下載檔案數上限]</td> 
   <td>設定符合以下條件的最大結果數量： [!DNL Workfront Fusion] 會在一個週期內下載（每個案例執行的重複次數）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看共用檔案]

當您共用新檔案或更新現有共用檔案時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取要監視的資料夾]</td> 
   <td>選取您想要在其中觀看檔案的共用資料夾。</td> 
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
    <td >[！UICONTROL轉換 [!DNL Google Documents] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Documents] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Spreadsheets] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Spreadsheets] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Slides] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Slides] 至。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL轉換 [!DNL Google Drawings] 要格式化的檔案]</td>
    <td>選取您要轉換的檔案格式 [!DNL Google Drawings] 至。</td>
  </tr> 
  <tr> 
   <td>[！UICONTROL監視]</td> 
   <td>選取您要觀看新檔案與所有變更，還是隻觀看新檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL下載檔案數上限]</td> 
   <td>設定符合以下條件的最大結果數量： [!DNL Workfront Fusion] 會在一個週期內下載（每個案例執行的重複次數）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看評論]

在選取的檔案上新增或修改註解時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案]</td> 
   <td>選取您要觀看註解的檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL監視]</td> 
   <td>選取您是要觀看所有變更，還是隻觀看新註解</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回評論的最大數量]</td> 
   <td>設定評論數目上限，此上限會 [!DNL Workfront Fusion] 會在一個週期內傳回（每個案例執行的重複次數）。</td> 
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

將檔案上傳至 [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>[！UICONTROL來源檔案]</td> 
   <td>選取您要使用從先前模組傳入的檔案，或是要手動對應檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案名稱]</td> 
   <td>選取檔案名稱。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對應]」，則此選項可供使用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料]</td> 
   <td>選取您要上傳的資料檔案。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對應]」，則此選項可供使用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標題]</td> 
   <td>輸入新檔案的標題。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換檔案]</td> 
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
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>選取是否要取代檔案內容。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL來源檔案]</td> 
   <td>選取您要使用從先前模組傳入的檔案，或是要手動對應檔案。 如果您在上一個欄位中選取變更檔案內容，則可使用此欄位。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案名稱]</td> 
   <td>選取檔案名稱。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對應]」，則此選項可供使用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料]</td> 
   <td>選取您要上傳的資料檔案。 如果您在[！UICONTROL來源檔案]欄位中選取「[！UICONTROL對應]」，則此選項可供使用。</td> 
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
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td>將您要移動的檔案ID對應至垃圾桶。</td> 
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
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Documents] 要格式化的檔案]</td> 
   <td>選取您要轉換的檔案格式 [!DNL Google Documents] 至。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Spreadsheets] 要格式化的檔案]</td> 
   <td>選取您要轉換的檔案格式 [!DNL Google Spreadsheets] 至。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Slides] 要格式化的檔案]</td> 
   <td>選取您要轉換的檔案格式 [!DNL Google Slides] 至。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Drawings] 要格式化的檔案]</td> 
   <td>選取您要轉換的檔案格式 [!DNL Google Drawings] 至。</td> 
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
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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
       <li> <p><strong>[！UICONTROL查詢]</strong> </p> <p>輸入要搜尋的檔案名稱或完整檔案名稱（包括字尾）的一部分。</p> </li> 
       <li> <p><strong>[！UICONTROL搜尋選項]</strong> </p> <p>選取您要搜尋確切的字詞，或是要搜尋包含該搜尋字詞的名稱。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL Fulltext]搜尋</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查詢]</strong> </p> <p>輸入您要搜尋的任何搜尋字詞 [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>輸入自訂搜尋查詢</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查詢]</strong> </p> <p>輸入自訂搜尋查詢。 如需更多詳細資料，請參閱本文章的[！UICONTROL搜尋檔案]一節。</p> </li> 
       <li> <p><strong>將上方選取的資料夾新增至查詢</strong> </p> <p>搜尋父集合中的資料夾。 這會尋找直接位於上方所選資料夾中的所有檔案和資料夾。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回結果的最大數目]</td> 
   <td>設定檔案或資料夾的最大數量 [!DNL Workfront Fusion] 會在一個執行週期內傳回。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL即使模組未傳回任何結果，仍繼續執行路由]</td> 
   <td>啟用此選項以確保模組未傳回任何結果時不會停止此案例。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

在指定位置建立資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>如果您想要與任何具有[！UICONTROL Share]連結的人共用資料夾，請選取此選項。 否則，共用連結僅供擁有者使用。</td> 
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
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在連線 [!DNL Google Drive] 至[！UICONTROL Workfront Fusion]</a></p> </td> 
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

* 上傳的檔案太大，超過您的允許檔案大小上限。 [!DNL Google Drive] 計畫或您已超過您的 [!DNL Google Drive] 儲存空間限制。 您可以升級您的儲存空間計畫，或是從 [!DNL Google Drive] 服務。
* 要上傳檔案至的所選資料夾已不存在。 此情境會停止，然後需要再次選取目標資料夾。

## 搜尋檔案

在模組List files in a folder中，您可以使用自己的查詢，該查詢由以下部分組成：

* **[!UICONTROL 欄位]**  — 正在搜尋之檔案的屬性，例如，屬性 `name` 檔案的。

* **[!UICONTROL 運運算元]**  — 對資料執行以提供相符的測試，例如， `contains`.

* **[!UICONTROL 值]**  — 測試之屬性的內容，例如檔案的名稱 `My cool document`.

結合條款與聯結 `and` 或 `or`，並使用否定查詢 `not`.

* [欄位](#fields)
* [值型別](#value-types)
* [運運算元](#operators)
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
   <th>運運算元</th> 
   <th> <p> 說明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>字串</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 檔案的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>字串 </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> 檔案的全文，包括名稱、說明、內容和可編制索引的文字。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> 字串</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 檔案的MIME型別。</p> </td> 
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
   <td><code>=</code>， <code>!=</code></td> 
   <td> <p> 檔案是否在垃圾桶中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>布林值 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>檔案是否啟動。</p> </td> 
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

請考量下列這些欄位中的運運算元：

* 此 `contains` 運運算元只執行 `title`.

  例如，「HelloWorld」標題符合 `title contains 'Hello'` 但不適用於 `title contains 'World'`.

* 此 `contains` 運運算元只會對下列專案的整個字串Token執行比對 `fullText`.

  例如，如果檔案的全文包含字串「HelloWorld」，則只有查詢 `fullText contains 'HelloWorld'` 傳回結果。 查詢，例如 `fullText contains 'Hello'` 不會在此案例中傳回結果。

* 此 `contains` 運運算元會比對完全符合的英數字元片語（如果由雙引號包圍）。

  例如，如果 `fullText` 檔案內包含「Hello there world」字串，然後是查詢 `fullText contains '"Hello there"'` 傳回結果，但查詢 `fullText contains '"Hello world"'` 不會。

  此外，由於搜尋是英數字元，如果 `fullText` 檔案內含字串「Hello_world」，則為查詢 `fullText contains '"Hello world"'` 傳回結果。

* 欄位 `type` 日期目前無法相互比較，只能與固定日期比較。

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
   <td> <p>以單引號括住'。 使用逸出查詢中的單引號 <code>\'</code>，例如，<code> 'Valentine\'s Day'</code>.</p> </td> 
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

### 運運算元

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
   <td> <p> 字串或布林值的內容等於另一個。</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 字串或布林值的內容不等於另一個。</p> </td> 
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
   <td> <p> 一個日期晚於另一個日期。</p> </td> 
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
   <td> <p>集合包含符合引數的元素。</p> </td> 
  </tr> 
 </tbody> 
</table>

對於複合條款，您可以使用括弧將條款群組在一起。 例如：
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` 此搜尋會傳回影像或視訊MIME型別的所有檔案，其上次修改是在2012年6月4日之後。 因為 `and` 和 `or` 運運算元的評估方式為從左至右（不含括弧），上述範例只會傳回2012年6月4日之後修改的影像，但會傳回所有影片，甚至是2012年6月4日之前的影片。

### 範例

本頁的所有範例都會顯示未編碼的 `<q>q</q>` 引數，其中 `title = 'hello'` 編碼為 `title+%3d+%27hello%27`. 使用者端程式庫會自動處理此編碼。

* 搜尋名稱為「hello」的檔案
  <pre>title = 'hello'</pre>
* 使用資料夾特定的MIME型別搜尋資料夾
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* 搜尋不是資料夾的檔案
  <pre>mimeType！= 'application/vnd.google-apps.folder'</pre>
* 搜尋名稱包含「hello」和「goodbye」字樣的檔案
  <pre>標題包含'hello'，而[！UICONTROL名稱]包含'goodbye'</pre>
* 搜尋名稱不包含「hello」字樣的檔案
  <pre>標題不包含'hello'</pre>
* 搜尋內容中包含「hello」字樣的檔案
  <pre>fullText包含'hello'</pre>
* 搜尋內容中未包含「hello」字樣的檔案
  <pre>非fullText包含'hello'</pre>
* 搜尋內容中包含「hello world」確切片段的檔案
  <pre>fullText包含'"hello world"'fullText包含'"hello_world"'</pre>
* 使用包含「\」字元的查詢來搜尋檔案（例如「\authors」）
  <pre>fullText包含'\\author'</pre>
* 搜尋使用者&quot;test@example.org&quot;可寫入的檔案
  <pre>中的'test@example.org' [!DNL writers]</pre>
* 搜尋ID `1234567` 在 `parents` 集合。 這會尋找直接位於ID為的資料夾中的所有檔案和資料夾 `1234567`.
  <pre>[！UICONTROL父代]中的'1234567'</pre>
* 搜尋別名ID `appDataFolder` 在 `parents` 集合。 這會找到所有檔案和資料夾，這些檔案和資料夾位於 [應用程式資料資料夾](https://developers.google.com/drive/api/v2/appdata).
  <pre>父級中的'appDataFolder'</pre>
* 搜尋使用者&quot;test@example.org&quot;和&quot;test2@example.org&quot;可寫入的檔案
  <pre>writers中的「test@example.org」及writers中的「test2@example.org」</pre>
* 搜尋垃圾桶內包含「重要」文字的檔案
  <pre>fullText包含'important'且true = true</pre>
* 搜尋在2012年6月4日之後修改的檔案
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' //預設時區為UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00呎</pre>
* 搜尋與授權使用者共用的檔案，且名稱中包含「hello」
  <pre>sharedWithMe，且標題包含'hello'</pre>
* 使用搜尋檔案 [自訂檔案屬性](https://developers.google.com/drive/api/v2/properties) 已命名 `additionalID` 包含值 `8e8aceg2af2ge72e78`.
  <pre>屬性有{ key='additionalID'和value='8e8aceg2af2ge72e78'和visibility='PRIVATE' }</pre>

本指南的來源為 [[!DNL Google Drive] 檔案](https://developers.google.com/drive/api/v2/search-shareddrives).
