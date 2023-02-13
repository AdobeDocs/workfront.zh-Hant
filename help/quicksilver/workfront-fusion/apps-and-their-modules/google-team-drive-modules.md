---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Google團隊驅動器模組
description: 此 [!DNL Adobe Workfront Fusion Google Team Drive] 模組可讓您監視、上傳、更新、複製、刪除或擷取檔案，以及在您的 [!DNL Google Shared] 開車。
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# [!DNL Google Team Drive] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] 模組可讓您監視、上傳、更新、複製、刪除或擷取檔案，以及在您的 [!DNL Google Shared Drive].

為了使用 [!DNL Google Team Drive] with [!DNL Adobe Workfront Fusion]，則必須有 [!DNL G Suite] 帳戶。 如果沒有，您可以建立 [!DNL G Suite] 帳戶 [[!DNL G Suite] 註冊網站](https://gsuite.google.com/signup/businessstarter/welcome).

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Google Team Drive]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Google Team Drive] 模組，您必須 [!DNL Google Team Drive].

## [!DNL Google Team Drive] 模組及其欄位

設定時 [!DNL Google Team Drive] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Google Team Drive] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

顯示於的模組對話方塊欄位 **粗體** (在 [!DNL Workfront Fusion] 方案， **not** 在本檔案文章中)是必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 觸發器

#### [!UICONTROL 監視檔案]

在指定的資料夾中添加和/或修改新檔案時，返回檔案詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL團隊驅動器]</td> 
   <td> <p> 選擇要監視的共用驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇共用驅動器內的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL要監視的檔案]</td> 
   <td> <p> 選擇要監視的檔案類型。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Documents] 檔案格式] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Documents] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Sheets] 檔案格式] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Sheets] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Slides] 檔案格式] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Slides] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Drawings] 檔案格式] </td> 
   <td> <p>選取您要觀看的格式 [!DNL Google Drawings] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> 選擇要監視新檔案和已修改檔案的資料夾還是僅監視新檔案的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL下載檔案的最大數量]</td> 
   <td> <p> 設定檔案數上限 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 更新檔案]](#update-a-file)
* [[!UICONTROL 複製檔案]](#copy-a-file)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 將檔案移至清除]](#move-a-file-to-trash)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 取得檔案清單]](#get-a-file-list)
* [[!UICONTROL 建立資料夾]](#create-a-folder)

#### [!UICONTROL 上傳檔案]

將檔案上載到指定的共用驅動器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL團隊驅動器] </td> 
   <td> <p>選擇要將檔案上載到的共用驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇共用驅動器內的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源檔案]</p> </td> 
   <td> <p>指定要上載到共用驅動器的檔案。</p> <p>對應您要從上一個模組上傳的檔案(例如[!UICONTROL HTTP] &gt;[!UICONTROL獲取檔案]或[!UICONTROLDropbox] &gt;[!UICONTROL獲取檔案)]，或手動輸入檔案名和檔案資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題]</td> 
   <td> <p> 輸入要顯示在共用資料夾中的檔案標題。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換檔案]</td> 
   <td> <p> 啟用此選項，可將檔案轉換為共用資料夾中對應的Google格式。</p> </td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL團隊驅動器]</td> 
   <td> <p> 選擇包含要更新的檔案的共用驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇共用驅動器內的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td> <p> 輸入（映射）要更新的檔案的ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源檔案]</p> </td> 
   <td>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標題] </td> 
   <td> <p>輸入更新檔案的新標題。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換檔案]</td> 
   <td> <p> 啟用此選項可將檔案轉換為對應的 [!DNL Google] 格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製檔案]

將指定的檔案複製到所選資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL團隊驅動器]</td> 
   <td> <p> 選擇包含要複製的檔案的共用驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇要將檔案複製到的目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td> <p> 輸入（映射）要複製的檔案的ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL複製檔案的名稱]</p> </td> 
   <td> <p>如果要在目標位置中更改新檔案名，請輸入該檔案名。</p> </td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td> <p> 輸入或映射要刪除的檔案的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將檔案移至清除]

將指定的檔案移到垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td> <p> 輸入或映射要移至垃圾桶的檔案ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

檢索有關指定檔案的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Documents] 檔案格式] </td> 
   <td> <p>選取您要的格式 [!DNL Google Documents] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Sheets] 檔案格式] </td> 
   <td> <p>選取您要的格式 [!DNL Google Sheets] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Slides] 檔案格式] </td> 
   <td> <p>選取您要的格式 [!DNL Google Slides] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換 [!DNL Google Drawings] 檔案格式] </td> 
   <td> <p>選取您要的格式 [!DNL Google Drawings] 檔案轉換為。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td> <p> 輸入或映射要檢索的檔案的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案清單]

根據搜索詞檢索檔案和/或資料夾詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL團隊驅動器]</td> 
   <td> <p> 選擇要列出檔案的共用驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇要列出檔案的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>選擇要執行的搜索類型 — 請參閱下文。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL查詢]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL在檔案名內搜索]</p> <p style="font-weight: normal;">選取[!UICONTROL搜尋確切詞語「搜尋」選項時，輸入檔案名稱（包括副檔名），或選取[!UICONTROL搜尋包含所搜尋詞語的名稱]選項時，輸入名稱的一部分。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL全文搜索]</p> <p>輸入搜索詞，以搜索檔案名、說明和內容。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL自定義搜索查詢]</p> <p>輸入 [!DNL Google] 搜尋查詢詞。 欲知更多詳情，請參閱 [!DNL Google]'s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">搜尋查詢檔案</a>. 範例: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檢索]</td> 
   <td>選擇要檢索檔案、資料夾還是兩者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回結果的最大數]</td> 
   <td> <p> 設定檔案或資料夾的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
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
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Team Drive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL團隊驅動器]</td> 
   <td> <p> 選擇要建立資料夾的共用驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇要在中建立資料夾的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新資料夾的名稱]</td> 
   <td> <p> 輸入新資料夾的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>
