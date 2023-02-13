---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Google Docs模組
description: Adobe Workfront聚變 [!DNL Google Docs] 模組可讓您監視、建立、編輯和擷取 [!DNL Google Docs] 和 [!DNL Google Docs] （適用於[!DNL G Suite]使用者）。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '4042'
ht-degree: 0%

---

# [!DNL Google Docs] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Docs] 模組可讓您監視、建立、編輯和擷取 [!DNL Google Docs] 和 [!DNL Google Docs] ( [!DNL G Suite] 使用者)。

為了使用 [!DNL Google Docs] with [!DNL Adobe Workfront Fusion]，則必須有 [!DNL Google] 帳戶。 如果你沒有 [!DNL Google] 帳戶，您可以在 [!DNL Google] 帳戶說明頁面。

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

使用 [!DNL Google Docs] 模組，您必須有Google帳戶。

## [!DNL Google Docs] 模組及其欄位

設定時 [!DNL Google Docs] 模組， [!UICONTROL Workfront融合] 顯示下列欄位。 此外， [!DNL Google Docs] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 文件

* [[!UICONTROL 監視文檔]](#watch-documents)
* [[!UICONTROL 列出文檔]](#list-documents)
* [[!UICONTROL 獲取文檔內容]](#get-content-of-a-document)
* [[!UICONTROL 建立文檔]](#create-a-document)
* [[!UICONTROL 從模板建立文檔]](#create-a-document-from-a-template)
* [[!UICONTROL 在文檔中插入段落]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL 將影像插入文檔]](#insert-an-image-to-a-document)
* [[!UICONTROL 用新影像替換影像]](#replace-an-image-with-a-new-image)
* [[!UICONTROL 替換文檔中的文本]](#replace-text-in-a-document)
* [[!UICONTROL 下載檔案]](#download-a-document)
* [[!UICONTROL 刪除文檔]](#delete-a-document)

#### [!UICONTROL 監視文檔]

在所選資料夾中建立或修改新文檔時，此觸發模組將返回文檔詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch文檔]</td> 
   <td> <p style="color: #000000;">選擇要查看已建立（[!UICONTROL按建立日期]）或已修改（[!UICONTROL按修改日期]）的文檔。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要監視的驅動器類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要監視已建立或已修改文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要監視已建立或已修改文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要監視的共用驅動器。</p> <p>注意：如果您已選取 [!DNL Google Shared Drive] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>在一個執行週期中設定Workfront Fusion返回的最大文檔數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出文檔]

此動作模組會從選取的資料夾中擷取檔案清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要列出文檔的驅動器類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要列出文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要列出文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要列出文檔的共用驅動器。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>設定文檔的最大數量 [!DNL Workfront Fusion] 在一個執行週期中傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 獲取文檔內容]

此操作模組檢索指定的文檔。

您可能需要擴充權限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取文檔的內容]</td> 
   <td> <p>選擇是要映射文檔的文檔ID，還是從下拉菜單中手動選擇文檔。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇包含要檢索的文檔的驅動器類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇包含要檢索的文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇包含要檢索的文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇包含要檢索的文檔的共用驅動器。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL篩選器]</p> </td> 
   <td> <p>在模組的輸出中選擇要返回的對象。</p> 
    <ul> 
     <li>[!UICONTROL影像]（預設）</li> 
     <li>[!UICONTROL繪圖]</li> 
     <li>[!UICONTROL圖表]</li> 
    </ul> <p>備註:  <p>要進一步映射這些對象，請使用此模組輸出中的[!UICONTROL Inline Objects Array]值（而不是[!UICONTROL inlineObjects]）。</p> <p>[!UICONTROL內聯對象陣列]對象的排序順序與它們在文檔中的顯示順序相同。 這可讓任何進一步的處理更輕鬆。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立文檔]

此操作模組允許您在選定資料夾中建立新文檔。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入文檔的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內容]</td> 
   <td> <p>輸入文檔的內容。 支援HTML。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要建立文檔的驅動器類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要建立文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要建立文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要建立文檔的共用驅動器。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL插入標題]</td> 
   <td> <p> 啟用此選項可將標題插入文檔，然後輸入或映射標題的文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL插入頁尾] </td> 
   <td> <p>啟用此選項可將頁尾插入文檔，然後輸入或映射頁首的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從模板建立文檔]

此動作模組會建立現有範本檔案的復本，並取代任何標籤。 此模組也可讓使用者依URL以新影像取代影像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL從模板建立文檔]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL通過映射]</strong> <br>選擇此選項可映射文檔模板。</li> 
     <li><strong>[!UICONTROL依下拉式清單]</strong> <br>選擇此選項可從下拉菜單中選擇文檔模板。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇模板所在的驅動器類型。 如果您在上一個欄位中選取了[!UICONTROL依下拉式清單]，便可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選取範本所在的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選取範本所在的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇模板所在的共用驅動器。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL值]</p> </td> 
   <td> <p>輸入要輸入的值，而不是新文檔的變數。</p> 
    <ul> 
     <li><strong>[!UICONTROL標籤]</strong> <br>輸入文檔模板中包含的標籤。 請勿使用 <code>&#123;&#123;&#125;&#125;</code>. 範例：use <code>name</code> 而非 <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL已替換值]</strong><br>輸入標籤的值。</li> 
    </ul> <p>例如<code> &#123;&#123;name&#125;&#125;</code> 變數將顯示為此處的「名稱」欄位，可在此插入值，例如 <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL影像替換]</p> </td> 
   <td> <p>輸入將替換當前影像的[!UICONTROL影像對象ID]和[!UICONTROL影像URL]的連結。</p> <p>注意：您可以使用[!UICONTROL獲取文檔]模組檢索影像ID，其中ID包含在陣列[!UICONTROL內聯對象陣列]中。</p> <p>建議您將ALT文字新增至 [!DNL Google] 檔案。 </p> <p>向 [!DNL Google Docs] 影像：</p> 
    <ol> 
     <li value="1">以滑鼠右鍵按一下影像。</li> 
     <li value="2">選擇[!UICONTROL ALT文本]選項。</li> 
     <li value="3">在[!UICONTROL標題]欄位中輸入[!UICONTROL ALT文本]，然後按一下[!UICONTROL確定]。</li> 
    </ol> <p>將ALT文本添加到影像後，ALT文本將以括弧顯示在欄位名稱中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題] </td> 
   <td> <p>輸入新文檔的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇模板所在的驅動器類型。 如果您在上一個欄位中選取了[!UICONTROL依下拉式清單]，便可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要建立文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要建立文檔的資料夾。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要建立文檔的共用驅動器。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在文檔中插入段落]

此操作模組將新段落附加或插入到現有文檔中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL選擇文檔]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL通過映射]</strong> <br>選擇此選項可映射文檔。</li> 
     <li><strong>[!UICONTROL依下拉式清單]</strong> <br> 選擇此選項可從下拉菜單中選擇文檔。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要添加段落的文檔所在的驅動器類型。 如果您在上一個欄位中選取了[!UICONTROL依下拉式清單]，便可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要添加段落的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要添加段落的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要添加段落的文檔所在的共用驅動器，然後選擇該文檔。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL插入段落]</p> </td> 
   <td> <p>選擇要在文檔中插入新文本的方式。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL按位置規範]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL按索引]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL索引]</strong> </p> <p>輸入要插入文本的索引號。 您可以使用[!UICONTROL獲取文檔]模組檢索索引號。</p> <p>要顯示文檔中的所有字元（包括隱藏的字元），可以使用[!UICONTROL Show]附加元件。 您可以在[!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]下找到該附加元件。 搜索[!UICONTROL Show]並安裝[!UICONTROL Show]附加元件。</p> </li> 
         <li> <p><strong>[!UICONTROL插入的文本]</strong> </p> <p>輸入要插入到文檔的文本。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL依區段ID]</strong> </p> <p>選擇要插入文本內容的頁首和頁尾，並輸入要插入到相應欄位的文本。</p> <p>如果頁首或頁尾已包含文字，則會在現有文字之前新增新文字。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL通過附加到文檔的正文]</strong> </p> <p>在文檔正文內容的結尾附加輸入的文本。</p> <p>新段落的樣式將從當前插入索引的段落中複製，包括清單和項目符號。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL通過附加到段的結尾（頁首和頁尾）]</strong> </p> <p>選擇要插入文本內容的頁首和頁尾，並輸入要插入到相應欄位的文本。</p> <p>如果頁首或頁尾已包含文字，則會在現有文字之後新增新文字。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL附加文本]</td> 
   <td>輸入或映射要附加到文檔的文本</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將影像插入文檔]

此動作模組會將影像從URL插入檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL選擇文檔]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL通過映射]</strong> <br>選擇此選項可映射文檔模板。</li> 
     <li><strong>[!UICONTROL依下拉式清單]</strong> <br> 選擇此選項可從下拉菜單中選擇文檔。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要添加影像的文檔所在的驅動器類型。 如果您在上一個欄位中選取了[!UICONTROL依下拉式清單]，便可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要添加影像的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要添加影像的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要添加影像的文檔所在的共用驅動器，然後選擇該文檔。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL插入影像]</p> </td> 
   <td> <p>選擇要如何在文檔中插入新影像。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL按位置規範]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL按索引]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL索引]</strong> </p> <p>輸入要插入影像的索引號。 您可以使用[!UICONTROL獲取文檔]模組檢索[!UICONTROL索引號]。</p> <p>要顯示文檔中的所有字元（包括隱藏的字元），可以使用[!UICONTROL Show]附加元件。 您可以在[!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]下找到該附加元件。 搜索[!UICONTROL Show]並安裝[!UICONTROL Show]附加元件。</p> </li> 
         <li> <p><strong>[!UICONTROL影像URL]</strong> </p> <p>輸入要插入到文檔的影像的URL。</p> <p>最大影像大小為50 MB。 不能超過2500萬像素。 僅支援PNG、JPEG或GIF格式。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL依區段ID]</strong> </p> <p>選取您要插入影像的頁首與頁尾，然後輸入對應欄位的影像URL。</p> <p>最大影像大小為50 MB。 影像不得超過2500萬像素。 僅支援PNG、JPEG或GIF格式。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL通過附加到文檔的正文]</strong> </p> <p>在文檔正文內容的結尾附加特定影像。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL通過附加到段的結尾（頁首和頁尾）]</strong> </p> <p>選取要插入影像的頁首和頁尾，並輸入要插入至對應欄位的影像URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL點的高度模/點的寬度模]</p> </td> 
   <td> <p>定義插入影像的大小。 將保持外觀比例。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 用新影像替換影像]

此動作模組會取代現有影像。 將保持原始影像的長寬比。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL選擇文檔]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL通過映射]</strong> <br>選擇此選項可映射文檔模板。</li> 
     <li><strong>[!UICONTROL依下拉式清單]</strong> <br> 選擇此選項可從下拉菜單中選擇文檔。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要替換影像的文檔所在的驅動器類型。 如果您在上一個欄位中選取了[!UICONTROL依下拉式清單]，便可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要替換影像的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要替換影像的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要替換影像的文檔所在的共用驅動器，然後選擇該文檔。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL影像URL]</p> </td> 
   <td> <p>輸入或映射將替換現有影像的新影像的URL。</p> <p>影像按它們在文檔中的顯示順序列出。 例如， <code>Body: Image No. 1</code> 是文檔中的第一個影像。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 替換文檔中的文本]

此動作模組會取代檔案中的文字。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL選擇文檔]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL通過映射]</strong> <br>選擇此選項可映射文檔模板。</li> 
     <li><strong>[!UICONTROL依下拉式清單]</strong> <br> 選擇此選項可從下拉菜單中選擇文檔。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要添加文本的文檔所在的驅動器類型。 如果您在上一個欄位中選取了[!UICONTROL依下拉式清單]，便可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要添加文本的文檔所在的資料夾，然後選擇文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要添加文本的文檔所在的資料夾，然後選擇文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要添加文本的文檔所在的共用驅動器，然後選擇該文檔。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL替代文字]</p> </td> 
   <td> <p>新增您要取代的每個文字。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL要替換的舊文本]</strong> </p> <p>輸入要替換的文本。</p> </li> 
     <li> <p><strong>[!UICONTROL要插入的新文本]</strong> </p> <p>輸入新文本。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此操作模組將轉換和下載所選文檔。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要下載的文檔所在的驅動器類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要下載的文檔所在的資料夾，然後選擇文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要下載的文檔所在的資料夾，然後選擇文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要下載的文檔所在的共用驅動器，然後選擇該文檔。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL類型] </p> </td> 
   <td> <p>選擇下載文檔的目標檔案格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除文檔]

此動作模組會刪除檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要刪除的文檔所在的驅動器類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要刪除的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要刪除的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要刪除的文檔所在的共用驅動器，然後選擇該文檔。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL共用驅動器]</td> 
   <td> <p>選擇包含要下載的文檔的驅動器，然後選擇文檔。 如果您已選取，則此選項可供使用 [!DNL Google Docs] 在[!UICONTROL選擇驅動器]欄位中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文檔ID]</td> 
   <td> <p> 選擇或映射要在中替換一個或多個影像的文檔。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 使文檔中的所有連結都可點按]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL 進行API呼叫]

此動作模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>輸入相對於的路徑 <code>https://docs.googleapis.com/</code>. 範例: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 為您添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p> 輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**範例：** 下列API呼叫會擷取Google檔案中指定檔案的詳細資訊：

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZxB6aY

**方法:**

[!UICONTROL GET]

![](assets/api-call-example.png)

在模組的「輸出」下，可找到擷取檔案的詳細資訊 [!UICONTROL 捆綁] > [!UICONTROL 主體].

![](assets/api-output.png)

#### [!UICONTROL 使文檔中的所有連結都可點按]

此動作模組會找出檔案中的所有連結，並使其可點按。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL在文檔中建立所有連結]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL通過映射]</strong> <br>選擇此選項可映射文檔模板。</li> 
     <li><strong>[!UICONTROL依下拉式清單]</strong> <br> 選擇此選項可從下拉菜單中選擇文檔。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選擇要在中建立可點按連結的文檔所在的驅動器類型。 如果您在上一個欄位中選取了[!UICONTROL依下拉式清單]，便可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL我的驅動器]</strong> </p> <p>選擇要在中建立可點按連結的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL與我共用]</strong> </p> <p>選擇要在中建立可點按連結的文檔所在的資料夾，然後選擇該文檔。</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] 共用驅動器]</strong> (適用於 [!DNL G Suite] 僅限使用者)</p> <p>選擇是否要[!UICONTROL使用域管理員訪問]。 選擇[!UICONTROL是]會以域管理員身份發出請求，並返回請求者為管理員的所有共用驅動器。</p> <p>選擇要在中建立可點按連結的文檔所在的共用驅動器，然後選擇該文檔。</p> <p>注意：如果您已選取 [!DNL Google Docs] 選項，而您 [!DNL G Suite] 使用者，錯誤 <code>[400] Invalid Value</code> 的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL共用驅動器]</td> 
   <td> <p>選擇包含要更新中連結的文檔的驅動器，然後選擇文檔。 如果您已選取，則此選項可供使用 [!DNL Google Docs] 在[!UICONTROL選擇驅動器欄位]中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文檔ID]</td> 
   <td> <p> 選擇或映射要在中更新連結的文檔。</p> </td> 
  </tr> 
 </tbody> 
</table>
