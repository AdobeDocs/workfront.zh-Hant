---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google幻燈片模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1685'
ht-degree: 0%

---

# [!DNL Google Slides]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [Google投影片模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-slides-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

[!DNL Adobe Workfront Fusion] [!DNL Google Slides]模組可讓您建立、更新、列出和/或刪除簡報，並將影像上傳到您[!DNL Google Slides]帳戶中的簡報。

若要搭配[!DNL Workfront Fusion]使用[!DNL Google Slides]，必須有[!DNL Google]帳戶。 如果您還沒有[!DNL Google]帳戶，您可以在[!DNL Google]帳戶說明頁面建立一個帳戶。

您的[!DNL Google Drive]中還需要[!DNL Google Slides]。

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL Google Slides]模組，您必須有[!DNL Google]帳戶。

## Google投影片API資訊

Google幻燈片聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td> https://slides.googleapis.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.5.9</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Slides]模組及其欄位

當您設定[!DNL Google Slides]模組時，Workfront Fusion會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Google Slides]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [簡報](#presentation)
* [其他](#other)

### 簡報

* [[!UICONTROL 觀看Presentations]](#watch-presentations)
* [[!UICONTROL 列出Presentations]](#list-presentations)
* [[!UICONTROL 取得簡報]](#get-a-presentation)
* [[!UICONTROL 取得頁面/縮圖]](#get-a-pagethumbnail)
* [[!UICONTROL 從範本建立簡報]](#create-a-presentation-from-a-template)
* [[!UICONTROL 上傳影像至簡報]](#upload-an-image-to-a-presentation)
* [[!UICONTROL 重新整理圖表]](#refresh-a-chart)
* [[!UICONTROL 新增/刪除投影片]](#adddelete-a-slide)

#### [!UICONTROL 觀看Presentations]

建立或更新新簡報時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL手錶] </td> 
   <td> <p>選取觀看簡報的選項：</p> 
    <ul> 
     <li> <p>[！UICONTROL建立日期]</p> </li> 
     <li> <p>[！UICONTROL修改日期]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>Workfront Fusion應在一個情境執行週期內傳回的最大簡報數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出Presentations]

擷取所有簡報的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機位置]</td> 
   <td> <p>選取您要列出的簡報所在的[!DNL Google Drive]：</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
     <li>[！UICONTROL [!DNL Google]共用磁碟機]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾ID]</td> 
   <td> <p>選擇您要列出之簡報的資料夾位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>在一個案例執行週期中，[!DNL Workfront Fusion]應傳回的最大簡報數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得簡報]

取得指定簡報的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要列出的簡報所在的[!DNL Google Drive]：</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
     <li>[！UICONTROL [!DNL Google]共用磁碟機]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL簡報ID]</td> 
   <td> <p> 選取您要擷取的簡報。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得頁面/縮圖]

取得指定頁面或簡報中頁面縮圖的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL簡報ID]</td> 
   <td> <p> 選取您要擷取的簡報ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL頁面物件ID]</td> 
   <td> <p> 選取您要檢視頁面物件詳細資訊的幻燈片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示頁面縮圖]</td> 
   <td> <p> 如果您想要檢視頁面縮圖資訊，請選取核取方塊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從範本建立簡報]

使用提供的資料取代範本中所有標籤（例如`{{Name}}`、`{{Email}}`）來建立新的簡報。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標題] </td> 
   <td> <p>輸入新簡報的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL複製簡報]</td> 
   <td> <p> 如果要複製現有的簡報，請選取選項：</p> 
    <ul> 
     <li>[！UICONTROL By Mapping]</li> 
     <li>[！UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL現有簡報ID的復本]</td> 
   <td> <p> 輸入要複製之現有簡報的路徑或簡報ID。 如果您正在建立簡報[！UICONTROL By Mapping]，則會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要列出的簡報所在的[!DNL Google Drive]：</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
     <li>[！UICONTROL [!DNL Google]共用磁碟機]</li> 
    </ul> <p>如果您要建立簡報[！UICONTROL By Dropdown]，就會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL簡報ID]</td> 
   <td> <p> 選取要做為範本之簡報的「簡報ID」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值] </td> 
   <td> <p>新增值：</p> 
    <ul> 
     <li><strong>[！UICONTROL標籤]</strong>：在簡報中輸入您要取代的標籤。 例如， <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[！UICONTROL取代的值]</strong>：輸入要取代現有標籤的值。 例如，如果字串 <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name&#125;&#125;</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳影像至簡報]

上傳含有所提供資料的影像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇簡報]</td> 
   <td> <p>選擇您要如何選取要上傳影像的簡報。</p> 
    <ul> 
     <li>[！UICONTROL By Mapping]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要列出的簡報所在的[!DNL Google Drive]：</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
     <li>[！UICONTROL [!DNL Google]共用磁碟機]</li> 
    </ul> <p>如果您要建立簡報[！UICONTROL By Dropdown]，就會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL簡報ID]</td> 
   <td> <p> 選取您要上傳影像的目標簡報的簡報ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td> <p>值新增值：</p> 
    <ul> 
     <li><strong>[！UICONTROL標籤]</strong>：輸入要新增URL的標籤。</li> 
     <li><strong>[！UICONTROL影像URL]</strong>：輸入要上傳的影像的路徑或URL。</li> 
    </ul> <p>注意：影像大小必須小於50MB、不能超過2500萬畫素，且必須是PNG、JPEG或GIF格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新整理圖表]

重新整理儲存在ID所指定簡報中的圖表資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要列出的簡報所在的[!DNL Google Drive]：</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
     <li>[！UICONTROL [!DNL Google]共用磁碟機]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL簡報ID]</td> 
   <td> <p>選取簡報的「簡報ID」，其中包含您要重新整理的圖表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL圖表物件ID]</td> 
   <td> <p> 選取您要重新整理的圖表。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增/刪除投影片]

建立空白投影片或刪除指定簡報上的現有投影片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取方法]</td> 
   <td> <p>選擇您要新增幻燈片或刪除幻燈片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>選取您要新增或刪除幻燈片的簡報的「簡報ID」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL預先定義的配置型別]</td> 
   <td> <p> 選取您要新增的幻燈片使用的預先定義幻燈片版面配置。 指定任何其他欄位的值（例如[！UICONTROL Title]）。</p> 
    <ul> 
     <li>[！UICONTROL空白版面，無預留位置]</li> 
     <li>[！UICONTROL佈局，底部有標題]</li> 
     <li>[！UICONTROL含標題和副標題的佈局]</li> 
     <li>[！UICONTROL佈局，含標題和內文]</li> 
     <li>[！UICONTROL具有標題和兩欄的佈局]</li> 
     <li>[！UICONTROL僅含標題的佈局]</li> 
     <li>[！UICONTROL版面配置含區段標題]</li> 
     <li>[！UICONTROL版面配置，標題和副標題為一側，說明為另一側]</li> 
     <li>[！UICONTROL版面配置有一個標題和一個內文，以單一欄排列]</li> 
     <li>具有主點的[！UICONTROL版面]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>如果您選取新增幻燈片，則可使用此欄位。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 在簡報中插入連結]](#insert-links-in-a-presentation)

#### [!UICONTROL 進行API呼叫]

執行任意授權的API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>輸入相對於https://developers.google.com/slides/的路徑。 例如，簡報。</p> <p>如需可用端點的清單，請參閱<a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API檔案</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>輸入所需的請求標頭。 您不需要新增授權標頭。</p> </td> 
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

>[!INFO]
>
>**範例：**&#x200B;您可以使用API呼叫取得您輸入的簡報ID的簡報詳細資料。 當您在[!DNL Google Slides]中開啟簡報時，可以在URL中找到簡報ID。
>
>![](assets/api-call-350x13.png)
>
>以下API呼叫會傳回簡報詳細資料：
>
>![](assets/presentation-details.png)
>
>在[!UICONTROL 組合] > [!UICONTROL 內文] > [!UICONTROL presentationId]下的模組輸出中，可找到搜尋的相符專案。
>
>在我們的範例中，已傳回要求的簡報詳細資料：
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL 在簡報中插入連結]

此模組可讓簡報中的所有連結可點按，或將連結插入所有相符的輸入文字中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Slides]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇簡報]</td> 
   <td> <p>選擇您要如何選取要上傳影像的簡報。</p> 
    <ul> 
     <li>[！UICONTROL By Mapping]</li> 
     <li>[！UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇磁碟機]</td> 
   <td> <p>選取您要列出的簡報所在的[!DNL Google Drive]：</p> 
    <ul> 
     <li>[！UICONTROL我的磁碟機]</li> 
     <li>[！UICONTROL與我共用]</li> 
     <li>[！UICONTROL [!DNL Google]共用磁碟機]</li> 
    </ul> <p>如果您要建立簡報[！UICONTROL By Dropdown]，就會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL簡報ID]</td> 
   <td> <p>選擇您要列出之簡報的資料夾位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取]</td> 
   <td> <p>選取您是否要將簡報中的所有連結設為可點按，或者是否要將連結插入所有相符的輸入文字中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文字輸入]</td> 
   <td>對於您想要新增連結的每個文字專案，請在清單中新增專案及其關聯的連結。 每次專案出現在簡報中時，它都會自動連結到指定的網站。</td> 
  </tr> 
 </tbody> 
</table>
