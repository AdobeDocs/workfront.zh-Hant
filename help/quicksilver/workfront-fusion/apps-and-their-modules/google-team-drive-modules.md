---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google團隊磁碟機模組
description: 此 [!DNL Adobe Workfront Fusion Google Team Drive] 模組可讓您監視、上傳、更新、複製、刪除或擷取檔案，以及在 [!DNL Google Shared] 推動。
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# [!DNL Google Team Drive] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] 模組可讓您監視、上傳、更新、複製、刪除或擷取檔案，以及在 [!DNL Google Shared Drive].

為了使用 [!DNL Google Team Drive] 替換為 [!DNL Adobe Workfront Fusion]，必須有 [!DNL G Suite] 帳戶。 如果您沒有虛擬報表套裝，可以建立 [!DNL G Suite] 帳戶位於 [[!DNL G Suite] 註冊網站](https://gsuite.google.com/signup/businessstarter/welcome).

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Google Team Drive]，以及將其連線到多個協力廠商應用程式和服務。

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

## 必要條件

使用 [!DNL Google Team Drive] 模組，您必須擁有 [!DNL Google Team Drive].

## [!DNL Google Team Drive] 模組及其欄位

當您設定 [!DNL Google Team Drive] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Google Team Drive] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

在中顯示的模組對話方塊欄位 **粗體** (在 [!DNL Workfront Fusion] 情境， **not** 本文章中)為必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 觸發器

#### [!UICONTROL 觀看檔案]

在指定的資料夾中新增和/或修改新檔案時，傳回檔案詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL小組磁碟機]</td> 
   <td> <p> 選取您要觀看的共用磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取共用磁碟機中的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL要觀看的檔案]</td> 
   <td> <p> 選取您要觀看的檔案型別。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Documents] 要格式化的檔案] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Documents] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Sheets] 要格式化的檔案] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Sheets] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Slides] 要格式化的檔案] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Slides] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Drawings] 要格式化的檔案] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Drawings] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL監視]</td> 
   <td> <p> 選取您要監視資料夾中是否有新的和修改的檔案，或只監視新檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL下載檔案數上限]</td> 
   <td> <p> 設定檔案數量上限 [!DNL Workfront Fusion] 會在一個執行週期內傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 更新檔案]](#update-a-file)
* [[!UICONTROL 複製檔案]](#copy-a-file)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 將檔案移至垃圾桶]](#move-a-file-to-trash)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 取得檔案清單]](#get-a-file-list)
* [[!UICONTROL 建立資料夾]](#create-a-folder)

#### [!UICONTROL 上傳檔案]

將檔案上傳至指定的共用磁碟機。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL小組磁碟機] </td> 
   <td> <p>選取您要上傳檔案的共用磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取共用磁碟機中的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL來源檔案]</p> </td> 
   <td> <p>指定您要上傳至共用磁碟機的檔案。</p> <p>對應您要從上一個模組上傳的檔案(例如[！UICONTROL HTTP] &gt;[！UICONTROL取得檔案]或[！UICONTROLDropbox] &gt;[！UICONTROL取得檔案)]，或手動輸入檔案名稱和檔案資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標題]</td> 
   <td> <p> 輸入將在共用資料夾中顯示的檔案標題。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換檔案]</td> 
   <td> <p> 啟用此選項可將檔案轉換為共用資料夾中對應的Google格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新檔案]

可讓您變更檔案名稱和/或檔案內容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL小組磁碟機]</td> 
   <td> <p> 選取包含您要更新之檔案的共用磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取共用磁碟機中的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p> 輸入（對應）您要更新的檔案ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL來源檔案]</p> </td> 
   <td>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL標題] </td> 
   <td> <p>輸入更新檔案的新標題。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換檔案]</td> 
   <td> <p> 啟用此選項以將檔案轉換為對應的 [!DNL Google] 共用資料夾中的格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製檔案]

將指定的檔案複製到選取的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL小組磁碟機]</td> 
   <td> <p> 選取包含您要複製之檔案的共用磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取您要複製檔案的目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p> 輸入（對應）您要複製的檔案ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL複製檔案的名稱]</p> </td> 
   <td> <p>如果您想要在目標位置變更新檔案名稱，請輸入新檔案名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

刪除指定的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p> 輸入或對應您要刪除之檔案的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將檔案移至垃圾桶]

將指定的檔案移至垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p> 輸入或對應您要移至垃圾桶之檔案的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

擷取有關指定檔案的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Documents] 要格式化的檔案] </td> 
   <td> <p>選取您想要的格式 [!DNL Google Documents] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Sheets] 要格式化的檔案] </td> 
   <td> <p>選取您想要的格式 [!DNL Google Sheets] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Slides] 要格式化的檔案] </td> 
   <td> <p>選取您想要的格式 [!DNL Google Slides] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換 [!DNL Google Drawings] 要格式化的檔案] </td> 
   <td> <p>選取您想要的格式 [!DNL Google Drawings] 檔案已轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p> 輸入或對應您要擷取的檔案ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案清單]

根據搜尋字詞擷取檔案和/或資料夾詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL小組磁碟機]</td> 
   <td> <p> 選取您要列出檔案的共用磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取您要列出檔案的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋] </td> 
   <td> <p>選取您要執行的搜尋型別 — 請參閱下文。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL查詢]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[！UICONTROL在檔案名稱內搜尋]</p> <p style="font-weight: normal;">選取[！UICONTROL搜尋搜尋確切的字詞搜尋]選項時，輸入檔案名稱（包括副檔名），或選取[！UICONTROL搜尋包含搜尋字詞的名稱]選項時，輸入名稱的一部分。</p> </li> 
     <li> <p style="font-weight: bold;">[！UICONTROL全文檢索搜尋]</p> <p>輸入搜尋字詞，以搜尋檔案名稱、說明和內容。</p> </li> 
     <li> <p style="font-weight: bold;">[！UICONTROL自訂搜尋查詢]</p> <p>輸入 [!DNL Google] 搜尋查詢詞。 如需詳細資訊，請參閱 [!DNL Google]的 <a href="https://developers.google.com/drive/api/v2/ref-search-terms">搜尋查詢檔案</a>. 範例: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Retrieve]</td> 
   <td>選取您要擷取檔案、資料夾或兩者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回結果的最大數目]</td> 
   <td> <p> 設定檔案或資料夾的最大數量 [!DNL Workfront Fusion] 會在一個執行週期內傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

建立新資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google Team Drive] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL小組磁碟機]</td> 
   <td> <p> 選取您要建立資料夾的共用磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取您要建立資料夾的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新資料夾的名稱]</td> 
   <td> <p> 輸入新資料夾的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>
