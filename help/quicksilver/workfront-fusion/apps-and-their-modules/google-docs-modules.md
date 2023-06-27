---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google檔案模組
description: Adobe Workfront Fusion [!DNL Google Docs] 模組可讓您監視、建立、編輯和擷取您檔案中的 [!DNL Google Docs] 和 [!DNL Google Docs] （適用於[！DNL G Suite]使用者）。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '4090'
ht-degree: 0%

---

# [!DNL Google Docs] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Docs] 模組可讓您監視、建立、編輯和擷取您檔案中的 [!DNL Google Docs] 和 [!DNL Google Docs] (適用於 [!DNL G Suite] 使用者)。

為了使用 [!DNL Google Docs] 替換為 [!DNL Adobe Workfront Fusion]，必須有 [!DNL Google] 帳戶。 如果您沒有 [!DNL Google] 帳戶尚未完成時，您可以在 [!DNL Google] 帳戶說明頁面。

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

使用 [!DNL Google Docs] 模組，您必須擁有Google帳戶。

## [!DNL Google Docs] 模組及其欄位

當您設定 [!DNL Google Docs] 模組， [!UICONTROL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Google Docs] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 文件

* [[!UICONTROL 觀看檔案]](#watch-documents)
* [[!UICONTROL 列出檔案]](#list-documents)
* [[!UICONTROL 取得檔案內容]](#get-content-of-a-document)
* [[!UICONTROL 建立檔案]](#create-a-document)
* [[!UICONTROL 從範本建立檔案]](#create-a-document-from-a-template)
* [[!UICONTROL 在檔案中插入段落]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL 將影像插入檔案]](#insert-an-image-to-a-document)
* [[!UICONTROL 以新影像取代影像]](#replace-an-image-with-a-new-image)
* [[!UICONTROL 取代檔案中的文字]](#replace-text-in-a-document)
* [[!UICONTROL 下載檔案]](#download-a-document)
* [[!UICONTROL 刪除檔案]](#delete-a-document)

#### [!UICONTROL 觀看檔案]

在選取的資料夾中建立或修改新檔案時，此觸發模組會傳回檔案詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Watch Documents]</td> 
   <td> <p style="color: #000000;">選取您要觀看已建立的([！UICONTROL By Created Date])或已修改的([！UICONTROL By Modified Date])檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要監視的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要監視已建立或已修改檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要監視已建立或已修改檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要觀看的共用磁碟機。</p> <p>附註：如果您已選取 [!DNL Google Shared Drive] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>設定Workfront Fusion在一個執行週期內傳回的最大檔案數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出檔案]

此動作模組會從選取的資料夾中擷取檔案清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要列出檔案的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要列出其檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要列出其檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要列出檔案的共用磁碟機。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>設定檔案數量上限 [!DNL Workfront Fusion] 會在一個執行週期內傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案內容]

此動作模組會擷取指定的檔案。

您可能需要擴充許可權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得檔案的內容]</td> 
   <td> <p>選取您要對應檔案的檔案ID，或從下拉式選單中手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取包含您要擷取之檔案的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取包含您要擷取之檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取包含您要擷取之檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取包含您要擷取之檔案的共用磁碟機。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL篩選器]</p> </td> 
   <td> <p>選取您要在模組輸出中傳回的物件。</p> 
    <ul> 
     <li>[！UICONTROL影像] （預設）</li> 
     <li>[！UICONTROL Drawing]</li> 
     <li>[！UICONTROL圖表]</li> 
    </ul> <p>備註:  <p>若要進一步對應這些物件，請在此模組的輸出中使用[！UICONTROL Inline物件陣列]值（而非[！UICONTROL inlineObjects]）。</p> <p>[！UICONTROL Inline Objects Array]物件會以它們在檔案中的顯示順序排序。 如此一來，任何進一步處理作業都會更輕鬆。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立檔案]

此動作模組可讓您在選取的資料夾中建立新檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱] </td> 
   <td> <p>輸入檔名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內容]</td> 
   <td> <p>輸入檔案的內容。 支援HTML。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要建立檔案的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要建立檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要建立檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要建立檔案的共用磁碟機。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入頁首]</td> 
   <td> <p> 啟用此選項可將頁首插入檔案，然後輸入或對映頁首的文字。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入頁尾] </td> 
   <td> <p>啟用此選項可將頁尾插入檔案，然後輸入或對映頁首的文字。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從範本建立檔案]

此動作模組會建立現有範本檔案的復本並取代任何標籤。 此模組也可讓使用者依URL將影像取代為新的影像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL從範本建立檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>選取此選項，從下拉式選單中選擇檔案範本。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取範本所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown]，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取範本所在的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取範本所在的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取範本所在的共用磁碟機。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL值]</p> </td> 
   <td> <p>輸入將輸入的值，而不是新檔案的變數。</p> 
    <ul> 
     <li><strong>[！UICONTROL標籤]</strong> <br>輸入檔案範本中包含的標籤。 不要使用 <code>&#123;&#123;&#125;&#125;</code>. 範例：使用 <code>name</code> 而非 <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[！UICONTROL取代的值]</strong><br>輸入標籤的值。</li> 
    </ul> <p>例如<code> &#123;&#123;name&#125;&#125;</code> 來原始檔中的變數會顯示為「名稱」欄位，可在此處插入值，例如 <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL影像取代]</p> </td> 
   <td> <p>輸入將取代目前影像的[！UICONTROL影像物件ID]和[！UICONTROL影像URL]連結。</p> <p>注意：您可以使用[！UICONTROL Get a Document]模組擷取影像ID，其中ID包含在陣列[！UICONTROL內嵌物件陣列]中。</p> <p>建議您將ALT文字新增至中的影像 [!DNL Google] 檔案。 </p> <p>若要將替代文字新增至 [!DNL Google Docs] 影像：</p> 
    <ol> 
     <li value="1">以滑鼠右鍵按一下影像。</li> 
     <li value="2">選取[！UICONTROL替代文字]選項。</li> 
     <li value="3">在[！UICONTROL標題]欄位中輸入[！UICONTROL替代文字]，然後按一下[！UICONTROL確定]。</li> 
    </ol> <p>將ALT文字新增至影像後，ALT文字會以括弧顯示在欄位名稱中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標題] </td> 
   <td> <p>輸入新檔案的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取範本所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown]，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要建立檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要建立檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要建立檔案的共用磁碟機。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在檔案中插入段落]

此動作模組會將新段落附加或插入至現有檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>選取此選項以對應檔案。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br> 選取此選項，從下拉式選單中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要新增段落的檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown]，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要新增段落的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要新增段落的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要新增段落的檔案所在的共用磁碟機，然後選取檔案。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL插入段落]</p> </td> 
   <td> <p>選取您要將新文字插入檔案中的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL依位置規格]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[！UICONTROL索引]</strong> </p> <p>輸入要插入文字的索引編號。 您可以使用[！UICONTROL Get a Document]模組擷取索引號碼。</p> <p>若要顯示檔案中的所有字元（包括隱藏字元），您可以使用[！UICONTROL Show]附加元件。 您可以在[！UICONTROL Add-ons] &gt; [！UICONTROL Get add-ons]下找到附加元件。 搜尋[！UICONTROL Show]並安裝[！UICONTROL Show]附加元件。</p> </li> 
         <li> <p><strong>[！UICONTROL插入文字]</strong> </p> <p>輸入您要插入檔案的文字。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL，依區段ID]</strong> </p> <p>選取您要插入文字內容的頁首與頁尾，然後輸入要插入至對應欄位的文字。</p> <p>如果頁首或頁尾已包含文字，則新文字會新增到現有文字之前。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL附加至檔案本文]</strong> </p> <p>在檔案內文內容的結尾附加輸入的文字。</p> <p>新段落的樣式將從目前插入索引處的段落複製，包括清單和專案符號。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，附加到區段（頁首和頁尾）的結尾]</strong> </p> <p>選取您要插入文字內容的頁首與頁尾，然後輸入要插入至對應欄位的文字。</p> <p>如果頁首或頁尾已包含文字，則新文字會新增至現有文字之後。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL附加文字]</td> 
   <td>輸入或對應您要附加至檔案的文字</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將影像插入檔案]

此動作模組會將URL中的影像插入檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br> 選取此選項，從下拉式選單中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要新增影像的檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown]，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要新增影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要新增影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要新增影像的檔案所在的共用磁碟機，然後選取檔案。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL插入影像]</p> </td> 
   <td> <p>選取您要將新影像插入檔案中的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL依位置規格]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[！UICONTROL索引]</strong> </p> <p>輸入您要插入影像的索引編號。 您可以使用[！UICONTROL Get a Document]模組來擷取[！UICONTROL索引編號]。</p> <p>若要顯示檔案中的所有字元（包括隱藏字元），您可以使用[！UICONTROL Show]附加元件。 您可以在[！UICONTROL Add-ons] &gt; [！UICONTROL Get add-ons]下找到附加元件。 搜尋[！UICONTROL Show]並安裝[！UICONTROL Show]附加元件。</p> </li> 
         <li> <p><strong>[！UICONTROL影像URL]</strong> </p> <p>輸入您要插入檔案的影像URL。</p> <p>影像大小上限為50 MB。 不可超過2500萬畫素。 僅支援PNG、JPEG或GIF格式。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL，依區段ID]</strong> </p> <p>選取您要插入影像的頁首與頁尾，並在對應欄位中輸入影像URL。</p> <p>影像大小上限為50 MB。 影像不得超過2500萬畫素。 僅支援PNG、JPEG或GIF格式。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL附加至檔案本文]</strong> </p> <p>在檔案內文內容的結尾附加特定影像。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，附加到區段（頁首和頁尾）的結尾]</strong> </p> <p>選取您要插入影像的頁首與頁尾，然後輸入要插入至對應欄位的影像URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL以點為單位的高度量值/以點為單位的寬度量值]</p> </td> 
   <td> <p>定義插入影像的大小。 將會保持長寬比。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 以新影像取代影像]

此動作模組會取代現有影像。 將會維持原始影像的外觀比例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br> 選取此選項，從下拉式選單中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要取代影像之檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown]，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要取代影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要取代影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要取代影像之檔案所在的共用磁碟機，然後選取檔案。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL影像URL]</p> </td> 
   <td> <p>輸入或對映將取代現有影像的新影像URL。</p> <p>影像會以它們在檔案中的顯示順序列出。 例如， <code>Body: Image No. 1</code> 是檔案中的第一個影像。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取代檔案中的文字]

此動作模組會取代檔案中的文字。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br> 選取此選項，從下拉式選單中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要新增文字的檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown]，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要新增文字的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要新增文字的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要新增文字的檔案所在的共用磁碟機，然後選取檔案。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL取代文字]</p> </td> 
   <td> <p>新增您想要取代的每一個文字。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL要取代的舊文字]</strong> </p> <p>輸入您要取代的文字。</p> </li> 
     <li> <p><strong>[！UICONTROL要插入的新文字]</strong> </p> <p>輸入新文字。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會轉換及下載選取的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要下載的檔案所在的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要下載的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要下載的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要下載的檔案所在的共用磁碟機，然後選取檔案。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL型別] </p> </td> 
   <td> <p>選取已下載檔案的目標檔案格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

此動作模組會刪除檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要刪除的檔案所在的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要刪除的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要刪除的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要刪除的檔案所在的共用磁碟機，然後選取檔案。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共用磁碟機]</td> 
   <td> <p>選取包含您要下載之檔案的磁碟機，然後選取檔案。 如果您已選取「 」，則可使用此選項 [!DNL Google Docs] 在[！UICONTROL選擇磁碟機]欄位中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td> <p> 選取或對映您要取代一或多個影像的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 使檔案中的所有連結都可點按]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL 進行API呼叫]

此動作模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線] </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>輸入相對於 <code>https://docs.googleapis.com/</code>. 範例: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**範例：** 以下API呼叫會擷取您Google檔案中指定檔案的詳細資料：

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**方法:**

[!UICONTROL GET]

![](assets/api-call-example.png)

擷取檔案的詳細資訊可在模組的輸出中找到，位於 [!UICONTROL 組合] > [!UICONTROL 內文].

![](assets/api-output.png)

#### [!UICONTROL 使檔案中的所有連結都可點按]

此動作模組會尋找檔案中的所有連結，並讓這些連結可點按。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Google] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立情境 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Make All Links in a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br> 選取此選項，從下拉式選單中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您想讓連結可點按的檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown]，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要使連結可點選的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要使連結可點選的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共用磁碟機]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要使連結可點按的連結所在位置的共用磁碟機，然後選取檔案。</p> <p>附註：如果您已選取 [!DNL Google Docs] 選項，而您不是 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 會傳回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共用磁碟機]</td> 
   <td> <p>選取包含您要更新連結之檔案的磁碟機，然後選取檔案。 如果您已選取「 」，則可使用此選項 [!DNL Google Docs] 在[！UICONTROL選擇磁碟機欄位]中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td> <p> 選取或對映您要更新連結的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>
