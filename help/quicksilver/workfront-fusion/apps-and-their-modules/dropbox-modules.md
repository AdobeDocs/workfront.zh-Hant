---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Dropbox模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Dropbox的工作流，並將其連接到多個第三方應用程式和服務。這允許您自動執行諸如監視、搜索、檢索、列出、建立和編輯Dropbox中的檔案和資料夾等活動。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3013'
ht-degree: 0%

---

# [!DNL Dropbox] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL Dropbox]，並將其連接到多個第三方應用程式和服務。這允許您自動執行諸如監視、搜索、檢索、列出、建立和編輯您中的檔案和資料夾等活動 [!UICONTROL Dropbox].

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

## 必要條件

使用 [!DNL Dropbox] 模組，您必須 [!DNL Dropbox] 帳戶。

## [!DNL Dropbox] 模組及其欄位

設定時 [!DNL Dropbox] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Dropbox] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發模組](#trigger-modules)
* [用於獲取的模組 [!DNL Dropbox] 檔案和資料夾](#modules-for-getting-dropbox-files-and-folders)
* [建立和編輯模組 [!DNL Dropbox] 檔案和資料夾](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [其他模組](#other-modules)

### 觸發模組

#### [!UICONTROL 監視檔案]

當修改指定資料夾中的檔案時，此觸發器類型模組會傳回檔案詳細資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇要監視更改的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch也是子資料夾]</td> 
   <td> <p> 啟用此選項還監視所選資料夾中已修改檔案的子資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制] </td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 用於獲取的模組 [!DNL Dropbox] 檔案和資料夾

* [[!UICONTROL 搜索檔案/資料夾]](#search-filesfolders)
* [[!UICONTROL 下載檔案]](#download-a-file)
* [[!UICONTROL 取得資料夾中繼資料]](#get-a-folder-metadata)
* [[!UICONTROL 列出資料夾中的所有檔案/子資料夾]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL 列出檔案修訂]](#list-file-revisions)

#### [!UICONTROL 搜索檔案/資料夾]

此搜尋模組會在 [!DNL Dropbox] 符合您指定的搜尋查詢。

您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>輸入搜索詞。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇要搜索的資料夾。 此模組會搜尋整個 [!DNL Dropbox] 如果未選擇資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>檔案狀態</td> 
   <td> <p> 選擇檔案狀態以將搜索限制為選定的檔案狀態。</p> </td> 
  </tr> 
  <tr> 
   <td>檔案類別</td> 
   <td> <p> 選擇檔案類別，以限制搜索到選定的類別。</p> </td> 
  </tr> 
  <tr> 
   <td>副檔名</td> 
   <td> <p> 選擇要搜索的副檔名。</p> </td> 
  </tr> 
  <tr> 
   <td>限制 </td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會從資料夾下載檔案。

您可以指定檔案及其位置。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

>[!NOTE]
>
>此模組對於將檔案提供給後續模組非常有用。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>檔案的選取方式</td> 
   <td> <p> 選擇要映射檔案路徑還是手動選擇檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檔案路徑/檔案</p> </td> 
   <td> <p style="font-weight: bold;">檔案路徑</p> <p>輸入或映射目標路徑至檔案。</p> <p style="font-weight: bold;">檔案</p> <p>從功能表中選取檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得資料夾中繼資料]

此動作模組會擷取共用資料夾詳細資訊。

指定資料夾的ID。

模組會傳回資料夾和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>共用資料夾ID</td> 
   <td> <p> 輸入或映射要檢索有關詳細資訊的資料夾的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出資料夾中的所有檔案/子資料夾]

此操作模組列出特定資料夾中的檔案或資料夾。

指定資料夾的ID。

模組會傳回檔案或資料夾及任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>清單 </td> 
   <td> <p>選擇要檢索檔案還是資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>僅顯示可下載的檔案</td> 
   <td> <p> 啟用此選項只傳回可下載的檔案。 某些類型的檔案(例如Google檔案)無法下載。</p> </td> 
  </tr> 
  <tr> 
   <td>資料夾 </td> 
   <td> <p>輸入或映射要從中檢索檔案或資料夾的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>限制 </td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中列出的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出檔案修訂]

此動作模組會擷取特定檔案的所有檔案修訂版本（版本記錄）。\
您可指定檔案的ID。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>檔案的選取方式</td> 
   <td> <p> 選擇要映射檔案路徑還是手動選擇檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檔案路徑/檔案</p> </td> 
   <td> <p style="font-weight: bold;">檔案路徑</p> <p>輸入或映射目標路徑至檔案。</p> <p style="font-weight: bold;">檔案</p> <p>從功能表中選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>限制</p> </td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中列出的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 建立和編輯模組 [!DNL Dropbox] 檔案和資料夾

* [[!UICONTROL 上傳] 檔案](#upload-a-file)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 建立/覆寫文字檔案]](#createoverwrite-a-text-file)
* [[!UICONTROL 建立/更新共用連結]](#createupdate-a-share-link)
* [[!UICONTROL 還原檔案]](#restore-a-file)
* [[!UICONTROL 移動檔案/資料夾]](#move-a-filefolder)
* [[!UICONTROL 更名檔案/資料夾]](#rename-a-filefolder)
* [[!UICONTROL 刪除檔案/資料夾]](#delete-a-filefolder)

#### [!UICONTROL 上傳檔案]

此動作模組會將檔案上傳至資料夾。

您可以指定檔案的位置、要上傳的檔案，以及檔案的可選新名稱等資訊。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾]</td> 
   <td> <p> 選取 [!DNL Dropbox] 您要將檔案上傳至。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源檔案]</p> </td> 
   <td> <p>輸入或對應您要新增至的檔案 [!DNL Dropbox] 檔案夾。</p> <p style="font-weight: bold;">[!UICONTROL檔案名]</p> <p>輸入或映射檔案名，包括副檔名。</p> <p style="font-weight: bold;">[!UICONTROL檔案資料]</p> <p>輸入或映射檔案資料(來自以前的模組，如[!UICONTROL Google驅動器] &gt;[!UICONTROL獲取檔案)]。</p> <p>注意：上傳檔案的大小上限為150 MB。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL覆蓋現有檔案]</td> 
   <td> <p> 啟用此選項可將現有檔案替換為新檔案。 如果此選項保留為停用狀態，上傳的檔案會重新命名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

此動作模組會建立新資料夾。

可指定資料夾的路徑和名稱。

模組會傳回資料夾和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾名稱] </td> 
   <td> <p>輸入新資料夾的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL資料夾]</p> </td> 
   <td> <p>輸入或映射要建立新資料夾的路徑。</p> <p>備註:   <p>如果您使用 [!DNL Dropbox Business] 帳戶（含團隊空間），您必須移除斜線 <code>/</code>，或不點按 <strong>[!UICONTROL按一下這裡]以選擇資料夾</strong> 以在根目錄中建立團隊資料夾。</p> <p>如果斜線未移除錯誤 <code>[409] path/malformed_path/..</code> 的URL。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自動更名]</td> 
   <td> <p> 如果目標位置中已存在同名資料夾，請啟用此選項以更名新資料夾。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立/覆寫文字檔案]

此操作模組建立DOC檔案或覆蓋現有檔案的內容。

指定源檔案和資料夾。

模組會傳回資料夾和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇為]</td> 
   <td> <p> 選擇是建立還是覆蓋DOC檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇要建立檔案的目標位置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源檔案]</p> </td> 
   <td> <p>輸入或對應您要新增至的檔案 [!DNL Dropbox] 檔案夾。</p> <p style="font-weight: bold;">檔案名</p> <p>輸入新DOC檔案的檔案名（不帶副檔名）。</p> <p style="font-weight: bold;">檔案內容</p> <p>輸入DOC檔案的文本內容。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立/更新共用連結]

此動作模組會建立檔案的公用連結。

您可指定連結的檔案和資訊。

模組會傳回連結的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇檔案的方式]</td> 
   <td> <p> 選擇要映射還是輸入檔案路徑，或手動選擇檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL檔案路徑/檔案]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL檔案路徑]</p> <p>輸入或映射目標路徑至檔案。</p> <p style="font-weight: bold;">[!UICONTROL檔案]</p> <p>從功能表中選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL請求的可見性]</p> </td> 
   <td> <p>選取連結為公用、適用於團隊或密碼受限。</p> <p>注意：[!UICONTROL僅團隊]和[!UICONTROL使用密碼訪問]選項僅適用於具有 [!DNL Dropbox Pro] 或更新版本。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL連結的到期日]</td> 
   <td> <p> 輸入連結將過期且將無法存取的日期和時間。 如果此欄位留空，連結將不會過期。 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> <p>注意：[!UICONTROL僅團隊]和[!UICONTROL使用密碼訪問]選項僅適用於具有[!UICONTROLDropboxPro]或更高版本的用戶。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL連結的訪問級別]</p> </td> 
   <td> <p>設定連結收件者的權限。</p> <p><strong>[!UICONTROL查看器]</strong> 使用連結的使用者可以檢視內容並加上註解。</p> <p><strong>[!UICONTROL編輯器]</strong> 使用連結的使用者可以編輯、檢視和註解內容。</p> <p><strong>[!UICONTROL最大值]</strong> 使用連結的使用者會獲得您可設定連結的最大存取層級。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 還原檔案]

此動作模組會還原檔案的舊版本。

可指定檔案和所需修訂的編號。

模組會傳回版本的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇檔案的方式]</td> 
   <td> <p> 選擇要映射還是輸入檔案路徑，或手動選擇檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL檔案路徑] / [!UICONTROL檔案]</p> </td> 
   <td> <p><strong>[!UICONTROL檔案路徑]</strong> </p> <p>輸入或映射目標路徑至檔案。</p> <p><strong>[!UICONTROL檔案]</strong> </p> <p>從功能表中選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL修訂版]</p> </td> 
   <td> <p>輸入或映射要還原的修訂版本編號。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動檔案/資料夾]

此動作模組會將檔案或資料夾移至不同位置。

您可指定檔案或資料夾，以及移動該檔案或資料夾的方式和位置。

模組會傳回檔案或資料夾的ID以及任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇檔案的方式] </td> 
   <td> <p>選擇要映射還是輸入檔案路徑，或手動選擇檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL檔案/資料夾路徑] / [!UICONTROL檔案/資料夾]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL檔案/資料夾路徑]</p> <p>輸入或將目標路徑映射到檔案或資料夾。</p> <p style="font-weight: bold;">[!UICONTROL檔案/資料夾]</p> <p>從菜單中選擇檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL到資料夾]</p> </td> 
   <td> <p>輸入或映射檔案或資料夾的目標位置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL新名稱]</p> </td> 
   <td> <p>在新位置中輸入檔案或資料夾的新名稱。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL自動更名]</p> </td> 
   <td> <p>啟用此選項可確保如果存在同名的檔案或資料夾，則模組會通過在檔案或資料夾名稱后面添加([!UICONTROL NUMBER])來更名新檔案或資料夾。 否則，目標位置中的檔案或資料夾將被覆蓋。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL允許所有權轉讓]</p> </td> 
   <td> <p>啟用此選項可允許按所有者移動，即使這會導致移動內容的所有權轉移。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更名檔案/資料夾]

此動作模組會重新命名檔案或資料夾。

可指定檔案或資料夾以及新名稱。

模組會傳回檔案或資料夾的ID以及任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>檔案的選取方式</td> 
   <td> <p> 選擇要映射還是輸入檔案路徑，或手動選擇檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>檔案/資料夾路徑/檔案/資料夾</p> </td> 
   <td> <p style="font-weight: bold;">檔案/資料夾路徑</p> <p>輸入或將目標路徑映射到檔案或資料夾。</p> <p style="font-weight: bold;">檔案/資料夾</p> <p>從菜單中選擇檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>重新命名 </td> 
   <td> <p>輸入檔案的[!UICONTROL目標名稱]，包括副檔名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案/資料夾]

此動作模組會刪除檔案或資料夾。

可指定檔案或資料夾。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL選擇檔案的方式]</td> 
   <td> <p> 選擇要映射還是輸入檔案路徑，或手動選擇檔案。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL檔案路徑] / [!UICONTROL檔案]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL檔案路徑]</p> <p>輸入或映射目標路徑至檔案。</p> <p style="font-weight: bold;">[!UICONTROL檔案]</p> <p>從功能表中選取檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他模組

#### [!UICONTROL 進行API呼叫]

此動作模組可讓您對 [!DNL Dropbox] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Dropbox] 模組。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Dropbox] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對路徑輸入相對於的路徑 <code>https://api.dropboxapi.com</code>. 例如， <code>/2/files/list_folder</code></p> <p>注意：如需可用端點的清單，請參閱 <a href="https://www.dropbox.com/developers/documentation/http/documentation">DropboxAPI v2檔案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題] </td> 
   <td> <p>輸入所需的請求標題。 [!DNL Workfront Fusion] 自動添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查詢字串]</td> 
   <td> <p> 輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL正文] </td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:   <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 下列API呼叫會從 [!DNL /Text files] 檔案夾 [!DNL Dropbox] 帳戶：
>
>URL: `/2/files/list_folder`
>
>內文:
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
>如需搜尋的相符項目，請在模組的「輸出」下方找到 [!UICONTROL 捆綁] > [!UICONTROL 主體] >登入點。
>
>在此範例中，傳回10張票證：

## 常見問題

* [無法上傳或更新檔案](#unable-to-upload-or-update-a-file)
* [透過共用連結參考的影像不會轉譯](#image-referenced-via-a-shared-link-does-not-render)

### 無法上傳或更新檔案

上傳或更新檔案失敗時，有數種情況：

* 上傳的檔案太大，超過了您 [!DNL Dropbox] 計畫，或者你用了 [!DNL Dropbox] 帳戶的儲存配額。 您必須從 [!DNL Dropbox] 帳戶或升級您的計畫。
* 檔案上傳至的先前選取資料夾已不存在。 方案停止，您必須再次選取目標資料夾。

### 透過共用連結參考的影像不會轉譯

由 [!UICONTROL Dropbox] >[!UICONTROL 建立共用連結] 不會直接連結至影像，但會連結至 [!DNL Dropbox] 頁面。 若要強制下載影像，請取代結尾 `?dl=0` with `?dl=1`. 要強制渲染影像(例如，在Web瀏覽器中或在Facebook Messenger中)，請附加 `&raw=1` 至URL。

如果您需要取得網站或其他網站的影像直接或原始連結 [!DNL Workfront Fusion] 模組，您必須透過下列方式修改初始共用URL:

原始URL:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. 取代 `www` with `dl`.
1. 移除 `?dl=0`.

最終URL:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

若要自動修改URL，您可以使用 `replace()` 函式兩次：

* 用dl替換ww

   ![](assets/www-to-dl-350x32.png)

* 並刪除？dl=0

   ![](assets/remove-dl0-350x33.png)

若要在單一步驟中完成，請結合下列函式：

![](assets/replace-both-350x47.png)

您也可以複製它並貼到欄位中。 取代 `1.url` 和URL。

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
