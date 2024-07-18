---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Dropbox模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Dropbox的工作流程，以及將其連線至多個協力廠商應用程式和服務。這可讓您自動執行Dropbox中的監控、搜尋、擷取、列出、建立及編輯檔案與資料夾等活動。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 86be8b6e1c21f3fd5f5b66afa3bf930d6bafbd63
workflow-type: tm+mt
source-wordcount: '3208'
ht-degree: 0%

---

# [!DNL Dropbox]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動執行使用[!UICONTROL Dropbox]或[!DNL Dropbox Business]的工作流程，以及將其連線至多個協力廠商應用程式和服務。這可讓您自動執行諸如監視、搜尋、擷取、列出、建立及編輯[!UICONTROL Dropbox]中的檔案與資料夾等活動。

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

## 先決條件

* 若要使用[!DNL Dropbox]模組，您必須有[!DNL Dropbox]帳戶。

>[!IMPORTANT]
>
>Dropbox必須核准使用者超過50人的應用程式。
>
>如需詳細資訊，請在Dropbox開發人員指南中搜尋「生產核准」。


## 建立與[!DNL Dropbox]的連線

若要為您的[!DNL Dropbox]模組建立連線：

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
        <tr>
        <td role="rowheader">[！UICONTROL環境]</td>
        <td>選取此連線是用於生產或非生產環境。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL型別]</td>
        <td>選取您要連線到服務帳戶還是個人帳戶。</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的[！UICONTROLDropbox] [！UICONTROL使用者端ID]。 </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的[!DNL Dropbox] [！UICONTROL使用者端密碼]。 </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL帳戶型別]</td>
        <td>選取您要連線至個人Dropbox帳戶或企業(Dropbox企業)帳戶。</td>
        </tr>
      </tbody>
    </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以儲存連線並返回模組。## [!DNL Dropbox]模組及其欄位

## [!DNL Dropbox]模組及其欄位

當您設定[!DNL Dropbox]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Dropbox]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [觸發模組](#trigger-modules)
* [取得 [!DNL Dropbox] 檔案與資料夾的模組](#modules-for-getting-dropbox-files-and-folders)
* [建立和編輯 [!DNL Dropbox] 檔案與資料夾的模組](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [其他模組](#other-modules)

### 觸發模組

#### [!UICONTROL 觀看檔案]

修改指定資料夾中的檔案時，此觸發型別模組會傳回檔案詳細資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取您要監視變更的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Watch也包含子資料夾]</td> 
   <td> <p> 啟用此選項也可監視所選資料夾中用於修改檔案的子資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制] </td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 取得[!DNL Dropbox]檔案與資料夾的模組

* [[!UICONTROL 搜尋檔案/資料夾]](#search-filesfolders)
* [[!UICONTROL 下載檔案]](#download-a-file)
* [[!UICONTROL 取得資料夾中繼資料]](#get-a-folder-metadata)
* [[!UICONTROL 列出資料夾中的所有檔案/子資料夾]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL 列出檔案修訂版本]](#list-file-revisions)

#### [!UICONTROL 搜尋檔案/資料夾]

此搜尋模組會在[!DNL Dropbox]中尋找符合您指定之搜尋查詢的物件記錄。

您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋] </td> 
   <td> <p>輸入搜尋字詞。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取您要搜尋的資料夾。 如果您未選取資料夾，此模組會搜尋整個[!DNL Dropbox]。</p> </td> 
  </tr> 
  <tr> 
   <td>檔案狀態</td> 
   <td> <p> 選取檔案狀態，將搜尋限制在選取的檔案狀態。</p> </td> 
  </tr> 
  <tr> 
   <td>檔案類別</td> 
   <td> <p> 選取檔案類別，將搜尋限制在選取的類別。</p> </td> 
  </tr> 
  <tr> 
   <td>副檔名</td> 
   <td> <p> 選擇您要搜尋的副檔名。</p> </td> 
  </tr> 
  <tr> 
   <td>限制 </td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會從資料夾下載檔案。

您可以指定檔案及其位置。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

>[!NOTE]
>
>此模組對於提供檔案給後續模組相當實用。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>選取檔案的方式</td> 
   <td> <p> 選取您要對應檔案路徑還是手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檔案路徑/檔案</p> </td> 
   <td> <p style="font-weight: bold;">檔案路徑</p> <p>輸入或對應目標路徑至檔案。</p> <p style="font-weight: bold;">檔案</p> <p>從選單中選取檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得資料夾中繼資料]

此動作模組會擷取共用資料夾詳細資料。

您可以指定資料夾的ID。

模組會傳回資料夾的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>共用資料夾識別碼</td> 
   <td> <p> 輸入或對應您要擷取其詳細資訊的資料夾ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出資料夾中的所有檔案/子資料夾]

此動作模組會列出特定資料夾中的檔案或資料夾。

您可以指定資料夾的ID。

模組會傳回檔案或資料夾的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>清單 </td> 
   <td> <p>選取您要擷取檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>僅顯示可下載的檔案</td> 
   <td> <p> 啟用此選項以僅傳回可下載的檔案。 部分型別的檔案(例如Google檔案)無法下載。</p> </td> 
  </tr> 
  <tr> 
   <td>資料夾 </td> 
   <td> <p>輸入或對應您要從中擷取檔案或資料夾的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>限制 </td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中列出的最大記錄數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出檔案修訂版本]

此動作模組會擷取特定檔案的所有檔案修訂版本（版本記錄）。\
您指定檔案的ID。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>選取檔案的方式</td> 
   <td> <p> 選取您要對應檔案路徑還是手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檔案路徑/檔案</p> </td> 
   <td> <p style="font-weight: bold;">檔案路徑</p> <p>輸入或對應目標路徑至檔案。</p> <p style="font-weight: bold;">檔案</p> <p>從選單中選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>限制</p> </td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中列出的最大記錄數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 建立和編輯[!DNL Dropbox]檔案與資料夾的模組

* [[!UICONTROL 上傳]檔案](#upload-a-file)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 建立/覆寫文字檔]](#createoverwrite-a-text-file)
* [[!UICONTROL 建立/更新共用連結]](#createupdate-a-share-link)
* [[!UICONTROL 還原檔案]](#restore-a-file)
* [[!UICONTROL 移動檔案/資料夾]](#move-a-filefolder)
* [[!UICONTROL 重新命名檔案/資料夾]](#rename-a-filefolder)
* [[!UICONTROL 刪除檔案/資料夾]](#delete-a-filefolder)

#### [!UICONTROL 上傳檔案]

此動作模組會將檔案上傳至資料夾。

您可以指定資訊，例如檔案的位置、要上傳的檔案，以及檔案的可選新名稱。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾]</td> 
   <td> <p> 選取您要上傳檔案的[!DNL Dropbox]資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Source檔案]</p> </td> 
   <td> <p>輸入或對應您要新增至上方所選[!DNL Dropbox]資料夾的檔案。</p> <p style="font-weight: bold;">[！UICONTROL檔案名稱]</p> <p>輸入或對應檔案名稱，包括副檔名。</p> <p style="font-weight: bold;">[！UICONTROL檔案資料]</p> <p>輸入或對應檔案資料(來自先前的模組，例如[！UICONTROL Google Drive] &gt;[！UICONTROL Get a File])。</p> <p>注意：上傳檔案的大小上限為150 MB。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL覆寫現有檔案]</td> 
   <td> <p> 啟用此選項以新檔案取代現有檔案。 如果此選項保持停用，則會重新命名上傳的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

此動作模組會建立新資料夾。

您可以指定資料夾的路徑和名稱。

模組會傳回資料夾的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾名稱] </td> 
   <td> <p>輸入新資料夾的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL資料夾]</p> </td> 
   <td> <p>輸入或對應您要建立新資料夾的路徑。</p> <p>注意：   <p>如果您使用[!DNL Dropbox Business]帳戶（含團隊空間），您必須移除斜線<code>/</code>，或不要按一下<strong>[！UICONTROL按一下這裡]以選擇資料夾</strong>，在根目錄中建立團隊資料夾。</p> <p>如果未移除斜線，則會傳回錯誤<code>[409] path/malformed_path/..</code>。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自動重新命名]</td> 
   <td> <p> 啟用此選項可重新命名新資料夾（如果目標位置中已存在相同名稱的資料夾）。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立/覆寫文字檔]

此動作模組會建立DOC檔案或覆寫現有檔案的內容。

您可以指定來源檔案和資料夾。

模組會傳回資料夾的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取至]</td> 
   <td> <p> 選取您要建立或覆寫DOC檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取您要建立檔案的目標位置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Source檔案]</p> </td> 
   <td> <p>輸入或對應您要新增至[!DNL Dropbox]資料夾的檔案。</p> <p style="font-weight: bold;">檔案名稱</p> <p>輸入新DOC檔案的檔案名稱（沒有副檔名）。</p> <p style="font-weight: bold;">檔案內容</p> <p>輸入DOC檔案的文字內容。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立/更新共用連結]

此動作模組會建立檔案的公開連結。

您可以指定檔案和連結的相關資訊。

模組會傳回連結的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取檔案的方式]</td> 
   <td> <p> 選取您要對映或輸入檔案路徑，或手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL檔案路徑/檔案]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL檔案路徑]</p> <p>輸入或對應目標路徑至檔案。</p> <p style="font-weight: bold;">[！UICONTROL檔案]</p> <p>從選單中選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL要求的可見度]</p> </td> 
   <td> <p>選取連結是公用連結、專案團隊連結或密碼限制連結。</p> <p>注意： [！UICONTROL Team only]和[！UICONTROL Access with password]選項僅適用於擁有[!DNL Dropbox Pro]或更新版本的使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL連結的到期日]</td> 
   <td> <p> 輸入連結到期且無法再存取的日期和時間。 如果此欄位留空，連結將不會過期。 如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p> <p>注意： [！UICONTROL Team only]和[！UICONTROL Access with password]選項僅適用於擁有[！UICONTROL Pro]或更高版本的Dropbox。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL連結的存取層級]</p> </td> 
   <td> <p>設定連結收件者的許可權。</p> <p><strong>[！UICONTROL Viewer]</strong>使用此連結的使用者可以檢視內容並加上註解。</p> <p><strong>[！UICONTROL Editor]</strong>使用該連結的使用者可以編輯、檢視和評論內容。</p> <p><strong>[！UICONTROL Max]</strong>使用連結的使用者會收到您可以設定連結的最大存取層級。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 還原檔案]

此動作模組會還原檔案的先前版本。

您可以指定檔案和您想要的修訂版本編號。

模組會傳回版本ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取檔案的方式]</td> 
   <td> <p> 選取您要對映或輸入檔案路徑，或手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL檔案路徑] / [！UICONTROL檔案]</p> </td> 
   <td> <p><strong>[！UICONTROL檔案路徑]</strong> </p> <p>輸入或對應目標路徑至檔案。</p> <p><strong>[！UICONTROL檔案]</strong> </p> <p>從選單中選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL修訂版]</p> </td> 
   <td> <p>輸入或對應您要還原之修訂版本的修訂版本編號。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動檔案/資料夾]

此動作模組會將檔案或資料夾移至其他位置。

您可以指定檔案或資料夾，以及移動的方式和位置。

模組會傳回檔案或資料夾的ID以及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取檔案的方式] </td> 
   <td> <p>選取您要對映或輸入檔案路徑，或手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL檔案/資料夾路徑] / [！UICONTROL檔案/資料夾]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL檔案/資料夾路徑]</p> <p>輸入或對應目標路徑至檔案或資料夾。</p> <p style="font-weight: bold;">[！UICONTROL檔案/資料夾]</p> <p>從選單中選取檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL至資料夾]</p> </td> 
   <td> <p>輸入或對應檔案或資料夾的目標位置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL新名稱]</p> </td> 
   <td> <p>在新位置輸入檔案或資料夾的新名稱。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL自動重新命名]</p> </td> 
   <td> <p>啟用此選項以確保如果存在具有相同名稱的檔案或資料夾，模組會重新命名新檔案或資料夾，方法是在檔案或資料夾名稱后面新增([！UICONTROL NUMBER])。 否則，會覆寫目標位置中的檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL允許所有權轉讓]</p> </td> 
   <td> <p>啟用此選項可允許所有者移動，即使這將導致所移動內容的所有權轉移。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新命名檔案/資料夾]

此動作模組會重新命名檔案或資料夾。

您可以指定檔案或資料夾以及新名稱。

模組會傳回檔案或資料夾的ID以及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>選取檔案的方式</td> 
   <td> <p> 選取您要對映或輸入檔案路徑，或手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檔案/資料夾路徑/檔案/資料夾</p> </td> 
   <td> <p style="font-weight: bold;">檔案/資料夾路徑</p> <p>輸入或對應目標路徑至檔案或資料夾。</p> <p style="font-weight: bold;">檔案/資料夾</p> <p>從選單中選取檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>重新命名 </td> 
   <td> <p>輸入檔案的[！UICONTROL目標名稱]，包括副檔名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案/資料夾]

此動作模組會刪除檔案或資料夾。

您指定檔案或資料夾。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL選取檔案的方式]</td> 
   <td> <p> 選取您要對映或輸入檔案路徑，或手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL檔案路徑] / [！UICONTROL檔案]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL檔案路徑]</p> <p>輸入或對應目標路徑至檔案。</p> <p style="font-weight: bold;">[！UICONTROL檔案]</p> <p>從選單中選取檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他模組

#### [!UICONTROL 進行API呼叫]

此動作模組可讓您對[!DNL Dropbox] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL Dropbox]模組無法完成的資料流程自動化。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Dropbox]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection-to-dropbox" class="MCXref xref">建立與[!DNL Dropbox]</a>的連線。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對路徑。輸入相對於<code>https://api.dropboxapi.com</code>的路徑。 例如， <code>/2/files/list_folder</code></p> <p>注意：如需可用端點的清單，請參閱<a href="https://www.dropbox.com/developers/documentation/http/documentation">DropboxAPI v2檔案</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Headers] </td> 
   <td> <p>輸入所需的請求標頭。 [!DNL Workfront Fusion]會自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查詢字串]</td> 
   <td> <p> 輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Body] </td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：   <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：**&#x200B;下列API呼叫傳回您[!DNL Dropbox]帳戶中[!DNL /Text files]資料夾的前10個檔案：
>
>URL： `/2/files/list_folder`
>
>內文：
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>在[!UICONTROL 組合] > [!UICONTROL 內文] >專案下的模組輸出中，可找到搜尋的相符專案。
>
>在我們的範例中，傳回10張票證：

## 常見問題

* [無法上傳或更新檔案](#unable-to-upload-or-update-a-file)
* [透過共用連結參照的影像無法呈現](#image-referenced-via-a-shared-link-does-not-render)

### 無法上傳或更新檔案

上傳或更新檔案失敗時有幾種情況：

* 上傳的檔案太大，超過您的[!DNL Dropbox]計畫允許的最大檔案大小，或者您已使用所有[!DNL Dropbox]帳戶的儲存配額。 您必須從您的[!DNL Dropbox]帳戶刪除現有檔案，或升級您的計畫。
* 先前選取的資料夾（檔案將上傳至該資料夾）已不存在。 此情境將停止，您必須再次選取目標資料夾。

### 透過共用連結參照的影像無法呈現

[!UICONTROL Dropbox] >[!UICONTROL 建立共用連結]傳回的URL不會直接連結至影像，而是連結至[!DNL Dropbox]頁面。 若要強制下載影像，請將結尾的`?dl=0`取代為`?dl=1`。 若要強制轉譯影像(例如在網頁瀏覽器或Facebook Messenger中)，請將`&raw=1`附加至URL。

如果您需要取得您網站或其他[!DNL Workfront Fusion]模組的直接或原始影像連結，您必須以下列方式修改初始的共用URL：

原始URL：

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. 以`dl`取代`www`。
1. 移除`?dl=0`。

最終URL：

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

若要自動修改URL，您可以使用`replace()`函式兩次：

* 以dl取代www

  ![](assets/www-to-dl-350x32.png)

* 若要移除？dl=0

  ![](assets/remove-dl0-350x33.png)

若要在一個步驟中執行操作，請組合下列函式：

![](assets/replace-both-350x47.png)

您也可以複製並貼到欄位中。 以URL取代`1.url`。

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
