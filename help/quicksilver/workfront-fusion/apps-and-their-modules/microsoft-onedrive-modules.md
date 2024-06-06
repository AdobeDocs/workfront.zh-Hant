---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft Onedrive模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用OneDrive的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '4073'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] 模組

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL OneDrive]，並連結至多個協力廠商應用程式和服務。

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
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先決條件

使用 [!DNL OneDrive] 模組，您必須擁有 [!DNL Microsoft OneDrive] 帳戶。




## 連線 [!DNL OneDrive] 服務對象 [!DNL Workfront Fusion]

如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!UICONTROL Workfront Fusion]，請參閱 [建立與的連線 [!UICONTROL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>部分Microsoft應用程式使用相同的連線，而此連線會繫結至個別使用者許可權。 因此，在建立連線時，許可權同意畫面會顯示先前授與此使用者連線的所有許可權，以及目前應用程式所需的任何新許可權。
>
>例如，如果使用者擁有透過Excel聯結器授予的「讀取表格」許可權，然後在Outlook聯結器中建立連線以讀取電子郵件，則許可權同意畫面會顯示已授予的「讀取表格」許可權和新要求的「寫入電子郵件」許可權。

## [!DNL Microsoft OneDrive] 模組及其欄位

當您設定 [!DNL OneDrive] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL OneDrive] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [檔案/資料夾](#filefolder)
* [其他](#other)

### 檔案/資料夾

* [[!UICONTROL 監視檔案/資料夾]](#watch-filesfolders)
* [[!UICONTROL 搜尋檔案/資料夾]](#search-filesfolders)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 下載檔案]](#download-a-file)
* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 取得共用連結]](#get-a-share-link)
* [[!UICONTROL 移動檔案/資料夾]](#move-a-filefolder)
* [[!UICONTROL 複製檔案]](#copy-a-file)
* [[!UICONTROL 刪除檔案/資料夾]](#delete-a-filefolder)

#### [!UICONTROL 監視檔案/資料夾]

此觸發模組會在檔案或資料夾建立或更新時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL監視檔案/資料夾]</td> 
   <td> <p>選取您要如何監視檔案或資料夾：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL By Created Time]</b> </p> <p>留意新檔案或資料夾。</p> </li> 
     <li> <p><b>[！UICONTROL，按更新時間]</b> </p> <p>留意已更新的現有檔案或資料夾。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要觀看的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入您要模組觀看的磁碟機ID。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> <p>導覽至您要模組觀看的資料夾。 您也可以輸入查詢來篩選傳回的結果。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL與我共用]</b> </p> <p>模組會監視已和磁碟機擁有者共用的檔案。</p> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取您要模組觀看的SharePoint網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取您要模組監視其磁碟機的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇專案型別]</td> 
   <td> <p>選取您要監視檔案、資料夾或兩者。</p> <p>注意：您無法在[！UICONTROL與我共用]磁碟機中監視資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL 搜尋檔案/資料夾]

此搜尋模組會根據您設定的條件傳回檔案和資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要搜尋的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入您希望模組搜尋的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> <p>導覽至您要模組搜尋的資料夾。 您也可以輸入查詢來篩選傳回的結果。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL與我共用]</b> </p> <p>模組會搜尋與磁碟機擁有者共用的檔案。</p> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取 [!DNL SharePoint] 您希望模組搜尋的網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取您要模組搜尋其磁碟機的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇專案型別]</td> 
   <td> <p>選取您要搜尋檔案、資料夾或兩者。</p> <p>注意：您無法在[！UICONTROL與我共用]磁碟機中搜尋資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此動作模組取得指定檔案的中繼資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入（檔案ID和檔案路徑）]</td> 
   <td>選取您要依「檔案ID」或「檔案路徑」來識別檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案識別碼] / [！UICONTROL檔案路徑]</td> 
   <td> <p>選取您要如何輸入「檔案ID」或「檔案路徑」：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您要從可用檔案或路徑清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要搜尋的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入包含您要取得之檔案的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取包含您要取得之檔案的SharePoint網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取其磁碟機包含您要取得之檔案的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要取得之檔案的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案] / [！UICONTROL檔案識別碼] / [！UICONTROL檔案路徑]</td> 
   <td> <p>如果您選取[！UICONTROL手動輸入]，請輸入或對應您要取得之檔案的檔案ID或路徑。</p> <p>如果您選取了[！UICONTROL從清單中選取]，請選取您要取得的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會下載指定的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入（檔案ID和檔案路徑）]</td> 
   <td>選取您要依「檔案ID」或「檔案路徑」來識別檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸入檔案ID /檔案路徑</td> 
   <td> <p>選取您要如何輸入「檔案ID」或「檔案路徑」：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您要從可用檔案或路徑清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要包含要下載之檔案的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入包含您要下載之檔案的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取包含您要下載之檔案的SharePoint網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取磁碟機包含要下載之檔案的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要下載之檔案的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案] / [！UICONTROL檔案識別碼] / [！UICONTROL檔案路徑]</td>
   <td> <p>如果您選取[！UICONTROL Enter Manually]，請輸入或對應您要下載的檔案識別碼或路徑。</p> <p>如果您選取了[！UICONTROL從清單中選取]，請選取您要下載的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL轉換為PDF]</td> 
   <td> <p>啟用此選項可將檔案轉換成PDF檔案。 您可以從下列檔案型別轉換：</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組會將檔案上傳至指定的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸入（資料夾位置ID與路徑）</td> 
   <td>選取您要依ID或路徑識別目標資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要上傳檔案的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>選取包含您要取得之檔案的磁碟機。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取 [!DNL SharePoint] 包含您要上傳檔案之資料夾的網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取其磁碟機包含要上傳檔案之資料夾的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取包含您要上傳檔案之資料夾的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL來源檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL，如果存在相同名稱的檔案]</td> 
   <td>選取當同名檔案已存在時如何繼續。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>新增說明至上傳的檔案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

這個動作模組會在指定的磁碟機中建立新資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要建立資料夾的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>選取您要建立資料夾的磁碟機。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取 [!DNL SharePoint] 您要建立資料夾的網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取擁有您要建立資料夾之驅動程式的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取您要建立資料夾的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>如果您希望新資料夾是子資料夾，請瀏覽至您希望它成為子資料夾的資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新資料夾名稱]</td> 
   <td> <p>輸入或對應新資料夾的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL，如果存在相同名稱的資料夾]</td> 
   <td>選取當同名檔案已存在時如何繼續。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得共用連結]

此動作模組會傳回指定檔案的共用連結。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入（檔案ID和檔案路徑）]</td> 
   <td>選取您要依「檔案ID」或「檔案路徑」來識別檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案識別碼] / [！UICONTROL檔案路徑]</td> 
   <td> <p>選取您要如何輸入「檔案ID」或「檔案路徑」：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您要從可用檔案或路徑清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要擷取共用連結的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入包含您要擷取共用連結之檔案的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取包含您要擷取共用連結之檔案的SharePoint網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取其磁碟機包含您要擷取共用連結之檔案的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要擷取共用連結之檔案的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案] / [！UICONTROL檔案識別碼] / [！UICONTROL檔案路徑]</td> 
   <td> <p>如果您選取[！UICONTROL手動輸入]，請輸入或對應您要擷取共用連結之檔案的檔案ID或路徑。</p> <p>如果您從清單中選取[！UICONTROL選取]，請選取您要擷取共用連結的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL許可權型別]</td> 
   <td> <p>選取您希望擁有連結的人員能夠讀取和寫入檔案，還是唯讀。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL範圍]</td> 
   <td>選取您希望檔案可供擁有該連結的任何人使用，還是僅供擁有該連結的組織成員使用。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動檔案/資料夾]

此動作模組會將檔案或資料夾移至新的資料夾位置

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入（檔案ID和檔案路徑）]</td> 
   <td>選取您要依「檔案ID」或「檔案路徑」來識別檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案ID /檔案路徑]</td> 
   <td> <p>選取您要如何輸入「檔案ID」或「檔案路徑」：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您要從可用檔案或路徑清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取包含您要移動之檔案或資料夾的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入包含您要移動之檔案或資料夾的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取 [!DNL SharePoint] 包含您要移動之檔案或資料夾的網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取其磁碟機包含您要移動之檔案或資料夾的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要移動之檔案或資料夾的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">選取[！UICONTROL檔案/資料夾]</td> 
   <td>選取您要移動檔案還是資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[！UICONTROL檔案] / [！UICONTROL檔案識別碼] / [！UICONTROL檔案路徑]</p> <p role="rowheader">[！UICONTROL資料夾] / [！UICONTROL資料夾識別碼] / [！UICONTROL資料夾路徑]</p> </td> 
   <td> <p>如果您選取[！UICONTROL手動輸入]，請輸入或對應您要移動之檔案或資料夾的ID或路徑。</p> <p>如果您從清單中選取[！UICONTROL選取]，請選取您要移動的檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入新資料夾位置]</td> 
   <td> <p>選取要如何輸入您要移動檔案或資料夾的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您要從可用檔案或路徑清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要移動檔案或資料夾的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入您要移動檔案或資料夾的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取 [!DNL SharePoint] 您要移動檔案或資料夾的網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取您要移動檔案或資料夾之磁碟機的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要移動檔案或資料夾之資料夾的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> <p>如果您將此專案留空，則檔案或資料夾只能在同一個 [!DNL OneDrive].</p> <p>您可以將檔案和資料夾從[！UICONTROL我的磁碟機]移動到[！UICONTROL網站的磁碟機]或[！UICONTROL群組的磁碟機]。 </p> <p>您只能將檔案從[！UICONTROL網站的磁碟機]移至相同網站的相同磁碟機。</p> <p>您只能將檔案從[！UICONTROL群組的磁碟機]移至相同群組中的相同磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>輸入或對應您要移動檔案或資料夾的資料夾。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製檔案]

此動作模組會將檔案複製到新的資料夾位置

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入（檔案ID和檔案路徑）]</td> 
   <td>選取您要依「檔案ID」或「檔案路徑」來識別檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案識別碼] / [！UICONTROL檔案路徑]</td> 
   <td> <p>選取您要如何輸入「檔案ID」或「檔案路徑」：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您要從可用檔案或路徑清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取包含您要複製之檔案的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入包含您要複製之檔案或資料夾的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取包含您要移動之檔案的SharePoint網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取其磁碟機包含您要複製之檔案的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要複製之檔案的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[！UICONTROL檔案] / [！UICONTROL檔案識別碼] / [！UICONTROL檔案路徑]</p> </td> 
   <td> <p>如果您選取[！UICONTROL Enter Manually]，請輸入或對應您要複製之檔案的ID或路徑。</p> <p>如果您從清單中選取[！UICONTROL選取]，請選取您要複製的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入新資料夾位置]</td> 
   <td> <p>選取要如何輸入您要複製檔案的位置，或：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您想要從可用資料夾清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新OneDrive位置]</td> 
   <td> <p>選取您要複製檔案管理員的位置。 如果您選擇從清單中選取新資料夾位置，則此選項可供使用。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入您要複製檔案之磁碟機的識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取 [!DNL SharePoint] 您要複製檔案的網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取您要複製檔案的磁碟機所在的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要複製檔案之資料夾的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> <p>如果您將此保留為空白，則檔案或資料夾只能複製到相同的[！UICONTROL OneDrive]中。</p> <p>您可以將檔案和資料夾從[！UICONTROL我的磁碟機]複製到[！UICONTROL網站的磁碟機]或[！UICONTROL群組的磁碟機]。 </p> <p>您只能將檔案從[！UICONTROL網站的磁碟機]複製到相同網站的相同磁碟機。</p> <p>您只能將檔案從[！UICONTROL群組的磁碟機]複製到相同群組中的相同磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>輸入或對應您要移動復本或資料夾的資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新複製的檔案名稱]</td> 
   <td> <p>輸入或對應檔案新復本的名稱。 如果您不想變更原始檔案名稱，可以保留空白。</p> <p>名稱必須包含副檔名。 範例：<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案/資料夾]

此動作模組會刪除選取的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入（檔案/資料夾ID和路徑）]</td> 
   <td>選取您要依「檔案ID」或「檔案路徑」來識別檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入檔案/資料夾識別碼/輸入檔案/資料夾路徑]</td> 
   <td> <p>選取您要如何輸入「檔案ID」或「檔案路徑」：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL手動輸入]</b> </p> <p>如果您想要直接輸入ID或路徑，或是從先前的模組進行對應，請選取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL從清單中選取]</b> </p> <p>如果您要從可用檔案或路徑清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取您要搜尋的位置：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL我的磁碟機]</b> </p> <p>選取是否啟用模組以輸入磁碟機ID。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL是]</b> </p> <p>輸入包含您要刪除之檔案或資料夾的磁碟機識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網站磁碟機]</b> </p> <p>選取 [!DNL SharePoint] 包含您要刪除之檔案或資料夾的網站。 可用的網站是後面跟著登入使用者的網站。</p> </li> 
     <li> <p><b>[！UICONTROL Group's Drive]</b> </p> <p>選取其磁碟機包含您要刪除之檔案或資料夾的群組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取或對應包含您要刪除之檔案或資料夾的磁碟機。 如果您在[！UICONTROL啟用輸入磁碟機ID]欄位中選取[！UICONTROL否]，則無法使用此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">選取[！UICONTROL檔案/資料夾]</td> 
   <td>選取您要刪除檔案還是資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案] / [！UICONTROL檔案識別碼] / [！UICONTROL檔案路徑]</td>
   <td> <p>如果您選取[！UICONTROL手動輸入]，請輸入或對應您要刪除之檔案的檔案ID或路徑。</p> <p>如果您從清單中選取[！UICONTROL選取]，請選取您要刪除的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此模組會執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關連線您的電腦的指示 [!DNL OneDrive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於 <code>https://graph.microsoft.com</code>. 範例：<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
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



## 如果您無法上傳或更新檔案

上傳或更新檔案失敗時，可能會出現幾個問題：

* 上傳的檔案太大，超過您的檔案大小上限。 [!DNL OneDrive] 計畫或您已使用您的所有 [!DNL OneDrive] 帳戶的儲存配額。 若要取得更多儲存空間，請從刪除現有檔案 [!DNL OneDrive] 或升級您的 [!DNL OneDrive] 帳戶。
* OneDrive不允許將兩個同名檔案上傳至單一資料夾。 如果目標資料夾包含與正在上傳的檔案同名的檔案，則案例執行會以錯誤終止。 解決方法就是重新命名要上傳的檔案。 如果您的目的是更新檔案，請使用 [!UICONTROL 更新檔案] 動作。
* 先前選取的資料夾（檔案將上傳至該資料夾）已不存在。 此情境將停止，您將需要再次選取目標資料夾。
