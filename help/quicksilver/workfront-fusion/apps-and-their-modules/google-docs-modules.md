---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google檔案模組
description: Adobe Workfront Fusion [!DNL Google Docs] 模組可讓您監視、建立、編輯和擷取 [!DNL Google Docs] 和 [!DNL Google Docs]  （適用於 [!DNL Google Workspace] 位使用者）中的檔案。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '4085'
ht-degree: 0%

---

# [!DNL Google Docs]模組

[!DNL Adobe Workfront Fusion] [!DNL Google Docs]模組可讓您監視、建立、編輯和擷取[!DNL Google Docs]和[!DNL Google Docs] （針對[!DNL Google Workspace]位使用者）中的檔案。

若要搭配[!DNL Adobe Workfront Fusion]使用[!DNL Google Docs]，必須有[!DNL Google]帳戶。 如果您還沒有[!DNL Google]帳戶，您可以在[!DNL Google]帳戶說明頁面建立一個帳戶。

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

若要使用[!DNL Google Docs]模組，您必須擁有Google帳戶。

## [!DNL Google Docs]模組及其欄位

當您設定[!DNL Google Docs]模組時，[!UICONTROL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Google Docs]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

### 文件

* [[!UICONTROL 觀看檔案]](#watch-documents)
* [[!UICONTROL 列出檔案]](#list-documents)
* [[!UICONTROL 取得檔案的內容]](#get-content-of-a-document)
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Watch Documents]</td> 
   <td> <p style="color: #000000;">選取您要觀看已建立的([！UICONTROL By Created Date])或已修改的([！UICONTROL By Modified Date])檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要監視的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取要監視已建立或已修改檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取要監視已建立或已修改檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要觀看的共用磁碟機。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Shared Drive]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>設定Workfront Fusion在一個執行週期中傳回的最大檔案數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出檔案]

此動作模組會從選取的資料夾擷取檔案清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要列出檔案的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要列出檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要列出檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取要列出檔案的共用磁碟機。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>設定在一個執行週期內傳回的最大檔案數[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案的內容]

此動作模組會擷取指定的檔案。

您可能需要擴充許可權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得檔案的內容]</td> 
   <td> <p>選取是否要對應檔案的檔案ID，或從下拉式選單中手動選取檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取包含您要擷取之檔案的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取包含您要擷取之檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取包含您要擷取之檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取包含您要擷取之檔案的共用磁碟機。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL篩選器]</p> </td> 
   <td> <p>選取您要在模組輸出中傳回的物件。</p> 
    <ul> 
     <li>[！UICONTROL Image] （預設）</li> 
     <li>[！UICONTROL Drawing]</li> 
     <li>[！UICONTROL圖表]</li> 
    </ul> <p>注意：  <p>若要進一步對應這些物件，請在此模組的輸出中使用[！UICONTROL Inline Objects Array]值（而非[！UICONTROL inlineObjects]）。</p> <p>[！UICONTROL Inline Objects Array]物件會以它們在檔案中的顯示順序排序。 如此一來，任何進一步處理作業都會更輕鬆。</p> </p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱] </td> 
   <td> <p>輸入檔案的名稱。</p> </td> 
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
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要建立檔案的共用磁碟機。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入頁首]</td> 
   <td> <p> 啟用此選項可將頁首插入檔案，然後輸入或對應頁首的文字。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入頁尾] </td> 
   <td> <p>啟用此選項可將頁尾插入檔案，然後輸入或對映頁首的文字。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從範本建立檔案]

此動作模組會建立現有範本檔案的復本，並取代任何標籤。 此模組也允許使用者透過URL將影像更換為新影像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL從範本建立檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL依對應]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>選取此選項，從下拉式功能表中選擇檔案範本。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取範本所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown] ，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取範本所在的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取範本所在的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取範本所在的共用磁碟機。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL值]</p> </td> 
   <td> <p>輸入將輸入的值，而不是新檔案的變數。</p> 
    <ul> 
     <li><strong>[！UICONTROL標籤]</strong> <br>請輸入檔案範本中包含的標籤。 請勿使用<code>&#123;&#123;&#125;&#125;</code>。 範例：使用<code>name</code>而非<code>&#123;&#123;name&#125;&#125;</code>。</li> 
     <li><strong>[！UICONTROL取代的值]</strong><br>請輸入標籤的值。</li> 
    </ul> <p>例如，來原始檔中的<code> &#123;&#123;name&#125;&#125;</code>變數將顯示為此處的name欄位，可插入值，例如<code>John</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL影像取代]</p> </td> 
   <td> <p>輸入要取代目前影像的[！UICONTROL影像物件ID]與[！UICONTROL影像URL]連結。</p> <p>注意：您可以使用[！UICONTROL Get a Document]模組擷取影像ID，其中ID包含在陣列[！UICONTROL Inline Object Array]中。</p> <p>建議您將ALT文字新增至[!DNL Google]檔案中的影像。 </p> <p>若要將ALT文字新增至[!DNL Google Docs]影像：</p> 
    <ol> 
     <li value="1">在影像上按一下右鍵。</li> 
     <li value="2">選取[！UICONTROL替代文字]選項。</li> 
     <li value="3">在[！UICONTROL標題]欄位中輸入[！UICONTROL替代文字]，然後按一下[！UICONTROL確定]。</li> 
    </ol> <p>將ALT文字加入影像後，ALT文字會顯示在括弧內的欄位名稱中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標題] </td> 
   <td> <p>輸入新檔案的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取範本所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown] ，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要建立檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要建立檔案的資料夾。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要建立檔案的共用磁碟機。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在檔案中插入段落]

此動作模組會將新段落附加或插入現有檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>選取此選項以對應檔案。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>選取此選項，從下拉式功能表中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要新增段落的檔案所在位置的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown] ，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要新增段落的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要新增段落的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要新增段落的檔案所在的共用磁碟機，然後選取檔案。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
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
         <li> <p><strong>[！UICONTROL插入文字]</strong> </p> <p>輸入要插入檔案的文字。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL （依區段識別碼）]</strong> </p> <p>選取您要插入文字內容的頁首與頁尾，並輸入要插入至對應欄位的文字。</p> <p>如果頁首或頁尾已包含文字，則新文字會新增到現有文字之前。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL藉由附加至檔案內文]</strong> </p> <p>在檔案內文內容的結尾附加輸入的文字。</p> <p>新段落的樣式將從目前插入索引處的段落複製，包括清單和專案符號。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，藉由附加至區段（頁首和頁尾）的結尾]</strong> </p> <p>選取您要插入文字內容的頁首與頁尾，並輸入要插入至對應欄位的文字。</p> <p>如果頁首或頁尾已包含文字，則新文字會新增至現有文字之後。</p> </li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL依對應]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>選取此選項，從下拉式功能表中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要新增影像的檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown] ，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要新增影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要新增影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要新增影像的檔案所在的共用磁碟機，然後選取檔案。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
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
         <li> <p><strong>[！UICONTROL索引]</strong> </p> <p>輸入要插入影像的索引編號。 您可以使用[！UICONTROL Get a Document]模組來擷取[！UICONTROL索引編號]。</p> <p>若要顯示檔案中的所有字元（包括隱藏字元），您可以使用[！UICONTROL Show]附加元件。 您可以在[！UICONTROL Add-ons] &gt; [！UICONTROL Get add-ons]下找到附加元件。 搜尋[！UICONTROL Show]並安裝[！UICONTROL Show]附加元件。</p> </li> 
         <li> <p><strong>[！UICONTROL影像URL]</strong> </p> <p>輸入要插入檔案的影像URL。</p> <p>影像大小上限為50 MB。 不得超過2500萬畫素。 僅支援PNG、JPEG或GIF格式。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL （依區段識別碼）]</strong> </p> <p>選取您要插入影像的頁首與頁尾，並將影像URL輸入至對應的欄位。</p> <p>影像大小上限為50 MB。 影像不得超過2500萬畫素。 僅支援PNG、JPEG或GIF格式。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL藉由附加至檔案內文]</strong> </p> <p>在檔案內文內容的結尾附加特定影像。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，藉由附加至區段（頁首和頁尾）的結尾]</strong> </p> <p>選取您要插入影像的頁首與頁尾，並輸入要插入至對應欄位的影像URL。</p> </li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL依對應]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>選取此選項，從下拉式功能表中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要取代影像之檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown] ，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要取代影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要取代影像的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要取代影像之檔案所在的共用磁碟機，然後選取檔案。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL影像URL]</p> </td> 
   <td> <p>輸入或對映將取代現有影像之新影像的URL。</p> <p>影像會以它們在檔案中的顯示順序列出。 例如，<code>Body: Image No. 1</code>是檔案中的第一個影像。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL選取檔案]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL依對應]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>選取此選項，從下拉式功能表中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要新增文字的檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown] ，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要新增文字的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要新增文字的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要新增文字的檔案所在的共用磁碟機，然後選取檔案。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL取代文字]</p> </td> 
   <td> <p>新增您想要取代的每一個文字。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL要取代的舊文字]</strong> </p> <p>輸入要取代的文字。</p> </li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要下載的檔案所在的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要下載的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要下載的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要下載的檔案所在的共用磁碟機，然後選取檔案。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要刪除的檔案所在的磁碟機型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您要刪除的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您要刪除的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您要刪除的檔案所在的共用磁碟機，然後選取檔案。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共用磁碟機]</td> 
   <td> <p>選取包含您要下載之檔案的磁碟機，然後選取檔案。 如果您已在[！UICONTROL選擇磁碟機]欄位中選取[!DNL Google Docs]，則此選項可供使用。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>輸入相對於<code>https://docs.googleapis.com/</code>的路徑。 範例： <code>/v1/documents/{presentationID}</code>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP要求方法。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增要求的標頭。例如，<code>{"Content-type":"application/json"}</code>。 [!DNL Workfront Fusion]為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**範例：**&#x200B;下列API呼叫會擷取Google檔案中指定檔案的詳細資料：

**URL：**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**方法：**

[!UICONTROL GET]

![](assets/api-call-example.png)

在[!UICONTROL 套件] > [!UICONTROL 內文]下的模組輸出中，可找到擷取檔案的詳細資料。

![](assets/api-output.png)

#### [!UICONTROL 使檔案中的所有連結都可點按]

此動作模組會尋找檔案中的所有連結，並讓這些連結可供點按。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Make All Links in a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL依對應]</strong> <br>選取此選項以對應檔案範本。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>選取此選項，從下拉式功能表中選擇檔案。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您想讓連結可點選的檔案所在的磁碟機型別。 如果您在上一個欄位中選取[！UICONTROL By Dropdown] ，即可使用此選項。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的磁碟機]</strong> </p> <p>選取您想讓連結可點選的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL與我共用]</strong> </p> <p>選取您想讓連結可點選的檔案所在的資料夾，然後選取檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共用磁碟機]</strong> （僅適用於[!DNL Google Workspace]位使用者）</p> <p>選取您是否要[！UICONTROL使用網域管理存取權]。 選取[！UICONTROL是]會以網域管理員身分發出請求，並傳回請求者身為管理員的所有共用磁碟機。</p> <p>選取您想讓連結可點選的檔案所在的共用磁碟機，然後選取檔案。</p> <p>注意：如果您已在此欄位中選取[!DNL Google Docs]選項，而且您不是[!DNL Google Workspace]使用者，則會傳回錯誤<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共用磁碟機]</td> 
   <td> <p>選取包含您要更新連結之檔案的磁碟機，然後選取檔案。 如果您已在[！UICONTROL選擇磁碟機欄位]中選取[!DNL Google Docs]，則此選項可供使用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td> <p> 選取或對應您要更新連結的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>
