---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Google幻燈片模組
description: Adobe Workfront Fusion Google幻燈片模組允許您建立、更新、列出和/或刪除演示文稿，並將影像上傳到Google幻燈片帳戶中的演示文稿。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 0%

---

# [!DNL Google Slides] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Google Slides] 模組可讓您建立、更新、列出和/或刪除簡報，並將影像上傳至您中的簡報 [!DNL Google Slides] 帳戶。

為了使用 [!DNL Google Slides] with [!DNL Workfront Fusion]，則必須有 [!DNL Google] 帳戶。 如果你沒有 [!DNL Google] 帳戶，您可以在 [!DNL Google] 帳戶說明頁面。

您也需要 [!DNL Google Slides] 在 [!DNL Google Drive].

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

使用 [!DNL Google Slides] 模組，您必須 [!DNL Google] 帳戶。

## [!DNL Google Slides] 模組及其欄位

設定時 [!DNL Google Slides] 模組中，Workfront Fusion會顯示下列欄位。 此外， [!DNL Google Slides] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
* [[!UICONTROL 添加/刪除幻燈片]](#adddelete-a-slide)

#### [!UICONTROL 觀看Presentations]

建立或更新新簡報時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>選擇觀看演示文稿的選項：</p> 
    <ul> 
     <li> <p>[!UICONTROL建立日期]</p> </li> 
     <li> <p>[!UICONTROL修改日期]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>在一個案例執行週期中，應返回的演示Workfront Fusion最多次。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出Presentations]

檢索所有演示文稿的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器位置]</td> 
   <td> <p>選取 [!DNL Google Drive] 您希望列出的演示文稿的位置：</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
     <li>[!UICONTROL [!DNL Google] 共用驅動器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID]</td> 
   <td> <p>選擇要列出的演示文稿的資料夾位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>演示的最大數量 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得簡報]

獲取指定演示文稿的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選取 [!DNL Google Drive] 您希望列出的演示文稿的位置：</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
     <li>[!UICONTROL [!DNL Google] 共用驅動器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 選擇要檢索的演示文稿。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得頁面/縮圖]

獲取演示文稿中指定頁面或頁面縮圖的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 選擇要檢索的演示ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL頁面對象ID]</td> 
   <td> <p> 選擇要查看其頁面對象詳細資訊的幻燈片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示頁面縮圖]</td> 
   <td> <p> 如果要查看頁面縮圖資訊，請選取核取方塊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從範本建立簡報]

通過替換所有標籤(如 `{{Name}}`, `{{Email}}` 在範本中提供資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題] </td> 
   <td> <p>輸入新演示文稿的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL複製演示文稿]</td> 
   <td> <p> 如果要複製現有演示文稿，請選擇該選項：</p> 
    <ul> 
     <li>[!UICONTROL通過映射]</li> 
     <li>[!UICONTROL依下拉式清單]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL現有演示ID的副本]</td> 
   <td> <p> 輸入要複製的現有演示文稿的路徑或演示文稿ID。 如果要建立演示文稿[!UICONTROL通過映射]，則會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選取 [!DNL Google Drive] 您希望列出的演示文稿的位置：</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
     <li>[!UICONTROL [!DNL Google] 共用驅動器]</li> 
    </ul> <p>如果要建立演示文稿[!UICONTROL按下拉清單]，則會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 選擇要用作模板的演示文稿的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值] </td> 
   <td> <p>新增值：</p> 
    <ul> 
     <li><strong>[!UICONTROL標籤]</strong>:在演示文稿中輸入要替換的標籤。 例如， <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL已替換值]</strong>:輸入要用來替換現有標籤的值。 例如，如果字串 <code>&#123;&#123;Name}}</code><code>Sample</code></li></ul></td></tr><tr><td role="rowheader"></td><td><p></p><ul><li></li><li></li><li></li></ul></td></tr><tr><td role="rowheader"><p></p></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr></tbody></table>

#### [!UICONTROL 上傳影像至簡報]

上傳含有提供資料的影像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇演示文稿]</td> 
   <td> <p>選擇要如何選擇將影像上載到的演示文稿。</p> 
    <ul> 
     <li>[!UICONTROL通過映射]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選取 [!DNL Google Drive] 您希望列出的演示文稿的位置：</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
     <li>[!UICONTROL [!DNL Google] 共用驅動器]</li> 
    </ul> <p>如果要建立演示文稿[!UICONTROL按下拉清單]，則會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 選擇要上載影像的演示文稿的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td> <p>值新增值：</p> 
    <ul> 
     <li><strong>[!UICONTROL標籤]</strong>:輸入要新增URL的標籤。</li> 
     <li><strong>[!UICONTROL影像URL]</strong>:輸入要上傳之影像的路徑或URL。</li> 
    </ul> <p>注意：影像的大小必須小於50MB，不能超過2500萬像素，且必須為PNG、JPEG或GIF格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新整理圖表]

刷新儲存在由ID指定的演示文稿中的圖表資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選取 [!DNL Google Drive] 您希望列出的演示文稿的位置：</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
     <li>[!UICONTROL [!DNL Google] 共用驅動器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p>選擇要刷新的圖表的演示的演示ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL圖表對象ID]</td> 
   <td> <p> 選擇要刷新的圖表。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加/刪除幻燈片]

建立空白幻燈片或刪除指定演示文稿上的現有幻燈片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇方法]</td> 
   <td> <p>選擇要添加新幻燈片還是刪除幻燈片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>選擇要添加或刪除幻燈片的演示文稿的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL預定義佈局類型]</td> 
   <td> <p> 選取您要新增的投影片要使用的預先定義投影片版面。 指定任何其他欄位的值（例如[!UICONTROL標題]）。</p> 
    <ul> 
     <li>[!UICONTROL空白佈局，無佔位符]</li> 
     <li>[!UICONTROL佈局，底部帶有註解]</li> 
     <li>[！帶標題和副標題的UICONTROL佈局]</li> 
     <li>[!UICONTROL佈局，帶標題和正文]</li> 
     <li>[!UICONTROL佈局，帶標題和兩列]</li> 
     <li>[!UICONTROL佈局，僅帶標題]</li> 
     <li>[!UICONTROL佈局，帶節標題]</li> 
     <li>[!UICONTROL佈局，一側帶有標題和副標題，另一側帶有描述]</li> 
     <li>[!UICONTROL佈局，以單列排列，具有一個標題和一個正文]</li> 
     <li>[!UICONTROL佈局，主點]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>如果您選擇添加幻燈片，則此欄位可用。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 在演示文稿中插入連結]](#insert-links-in-a-presentation)

#### [!UICONTROL 進行API呼叫]

執行任意授權的API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>輸入相對於https://developers.google.com/slides/的路徑。 例如，演示。</p> <p>如需可用端點的清單，請參閱 <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API檔案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>輸入所需的請求標題。 您不需要新增授權標題。</p> </td> 
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

>[!INFO]
>
>**範例：** 使用API呼叫，您就能取得您輸入之簡報ID的簡報詳細資訊。 在中開啟簡報時，您可以在URL中找到簡報ID [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>下列API呼叫會傳回簡報詳細資料：
>
>![](assets/presentation-details.png)
>
>如需搜尋的相符項目，請在模組的「輸出」下方找到 [!UICONTROL 捆綁] > [!UICONTROL 主體] > [!UICONTROL presentationId].
>
>在我們的示例中，返回了請求的演示詳細資訊：
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL 在演示文稿中插入連結]

此模組可點按演示文稿中的所有連結，或將連結插入所有匹配的輸入文本中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Slides] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇演示文稿]</td> 
   <td> <p>選擇要如何選擇將影像上載到的演示文稿。</p> 
    <ul> 
     <li>[!UICONTROL通過映射]</li> 
     <li>[!UICONTROL依下拉式清單]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇驅動器]</td> 
   <td> <p>選取 [!DNL Google Drive] 您希望列出的演示文稿的位置：</p> 
    <ul> 
     <li>[!UICONTROL我的驅動器]</li> 
     <li>[!UICONTROL與我共用]</li> 
     <li>[!UICONTROL [!DNL Google] 共用驅動器]</li> 
    </ul> <p>如果要建立演示文稿[!UICONTROL按下拉清單]，則會顯示此欄位。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p>選擇要列出的演示文稿的資料夾位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇]</td> 
   <td> <p>選擇是要讓簡報中的所有連結都可點按，還是要將連結插入所有匹配的輸入文本中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文本輸入]</td> 
   <td>針對您要新增連結的每個文字項目，新增項目及其相關連結至清單。 每次項目出現在簡報中時，就會自動連結至指定的網站。</td> 
  </tr> 
 </tbody> 
</table>
