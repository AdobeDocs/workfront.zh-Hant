---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 圖形模組
description: 使用 [!DNL Adobe Workfront Fusion] 圖形模組，您可以擷取註釋、檔案、檔案版本或專案的清單。 您也可以張貼註解或呼叫Figma API。
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2309'
ht-degree: 1%

---

# [!DNL Figma] 模組

使用 [!DNL Adobe Workfront Fusion] [!DNL Figma] 模組，您可以擷取註釋、檔案、檔案版本或專案的清單。 您也可以張貼註解或撥打電話至 [!DNL Figma] API。

如果您需要建立案例的說明，請參閱 [建立情境](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
      <td>
        <p>[！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
      <td>
        <p>[！UICONTROL計畫]，[！UICONTROL工作]</p>
      </td>
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

使用 [!DNL Figma] 模組，您必須擁有 [!DNL Figma] 帳戶。

## [!DNL Figma] 模組及其欄位

當您設定 [!DNL Figma] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Figma] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [評論](#comments)

* [專案和檔案](#projects-and-files)

* [元件和樣式](#components-and-styles)

* [其他](#other)


### 評論

* [刪除評論](#delete-a-comment)

* [列出註解](#list-comments)

* [發表評論](#post-a-comment)


#### [!UICONTROL 刪除評論]

此動作模組會從檔案中刪除單一註解。

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL檔案ID]</td>
      <td>輸入或對應您要新增或刪除註解的檔案的檔案ID。 </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL註解]</td>
      <td>輸入您要刪除的註解文字。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出註解]

此搜尋模組會列出所有附加至中單一檔案的註解 [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL檔案ID]</td>
      <td>
        <p>輸入或對應您要為其擷取註解的檔案的檔案ID。 </p>
        <ul>
          <li>
            <p>如果您不知道ID，請按一下 <b>[！UICONTROL尋找檔案]</b> 並輸入或對應與檔案相關聯的專案ID，然後選取檔案。</p>
          </li>
          <li>
            <p>如果您不知道專案的ID，請按一下 <b>[！UICONTROL尋找專案]</b> 並輸入或對應擁有該檔案關聯專案之團隊的ID，然後選取該專案，再選取該檔案。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>輸入或對應您希望模組在每個案例執行週期內傳回的最大註解數。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 發表評論]

此動作模組會將註解張貼至Figma檔案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[！UICONTROL檔案ID]</td>
      <td>
        <p>輸入或對應您要張貼註解的檔案的檔案ID。 </p>
        <ul>
          <li>
            <p>如果您不知道檔案的ID，請按一下 <b>[！UICONTROL尋找檔案]</b> 並輸入或對應與檔案相關聯的專案ID，然後選取檔案。</p>
          </li>
          <li>
            <p>如果您嘗試尋找檔案的ID但不知道專案的ID，請按一下 <b>[！UICONTROL尋找專案]</b> 並輸入或對應擁有檔案相關聯專案的團隊ID。 選取專案，然後選取檔案。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL註解]</td>
      <td>輸入註解的文字。</td>
    </tr>
  </tbody>
</table>


### 專案和檔案

* [取得檔案或影像](#get-a-file-or-image)

* [列出檔案版本記錄](#list-file-version-history)

* [列出專案檔案](#list-project-files)

* [列出專案](#list-projects)


#### [!UICONTROL 取得檔案或影像]

此動作模組會從Figma程式庫中擷取單一檔案或影像

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL物件型別]</td>
      <td>
        <p>選取您要擷取的物件型別。</p>
        <ul>
          <li>
            <p><b>[！UICONTROL檔案]</b>
            </p>
            <p>模組會傳回[！UICONTROL Key]參照的檔案作為JSON物件。 您可以從任何Figma檔案URL剖析檔案金鑰。</p>
            <p>如需欄位，請參閱 <a href="#Get2" class="MCXref xref" >[！UICONTROL取得檔案或影像：檔案]</a>.</p>
          </li>
          <li>
            <p><b>[！UICONTROL檔案節點]</b>
            </p>
            <p>傳回ID參照的節點作為JSON物件。 節點是從下列位置擷取： [!DNL Figma] 由[！UICONTROL Key]參考的檔案。</p>
            <p>如需欄位，請參閱 <a href="#Get3" class="MCXref xref" >[！UICONTROL取得檔案或影像：檔案節點]</a>.</p>
          </li>
          <li>
            <p><b>[！UICONTROL影像]</b>
            </p>
            <p>模組會從檔案轉譯影像。</p>
            <p>如需欄位，請參閱 <a href="#Get4" class="MCXref xref" >[！UICONTROL取得檔案或影像： Image]</a>.</p>
          </li>
          <li>
            <p><b>[！UICONTROL影像填色]</b>
            </p>
            <p>模組會傳回檔案中影像填色中所有影像的下載連結。 影像填色是如何 [!DNL Figma] 代表任何使用者提供的影像。 將影像拖曳到 [!DNL Figma]， [!DNL Figma] 使用單一填色來建立矩形，代表影像，且使用者可以變形矩形（和填色上的屬性）。</p>
            <p>如需欄位，請參閱 <a href="#Get5" class="MCXref xref" >[！UICONTROL取得檔案或影像：影像填色]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 取得檔案或影像：檔案]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL檔案索引鍵]</td>
      <td>選取您要傳回JSON的來源檔案。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL版本ID]</td>
      <td>輸入或對應您希望模組傳回的檔案版本。 對於目前的模組，請將此欄位留空。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL節點ID]</td>
      <td>
        <p>若只要傳回檔案的子集，請輸入您希望模組傳回的節點。 模組會傳回列出的節點、其子系，以及根節點與列出的節點之間的任何專案。</p>
        <p>針對您要傳回的每個節點，按一下 <b>[！UICONTROL新增]</b> 並輸入節點的文字。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL深度]</td>
      <td>
        <p>輸入或對應整數，該整數代表您要傳回結果的檔案樹狀結構深度。 </p>
        <div class="example"><span class="autonumber"><span><b>範例: </b></span></span>
          <ul>
            <li>
              <p>若要僅傳回頁面，請輸入 <code>1</code>.</p>
            </li>
            <li>
              <p>若要傳回頁面和頂層物件，請輸入 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>若要傳回所有節點，請將此欄位留空。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL幾何]</td>
      <td>若要傳回向量資料，請輸入 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL外掛程式資料]</td>
      <td>外掛程式ID和/或字串「[！UICONTROL shared]」的逗號分隔清單。 這些外掛程式所撰寫的檔案中的任何資料都會包含在的結果中， <code>pluginData</code> 和 <code>sharedPluginData</code> 屬性。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL分支資料]</td>
      <td>啟用此選項可傳回請求檔案的分支中繼資料。 如果檔案是分支，則主要檔案的金鑰會包含在傳回的回應中。 如果檔案有分支，則其中繼資料會包含在傳回的回應中。 預設: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 取得檔案或影像：檔案節點]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL檔案索引鍵]</td>
      <td>選取您要傳回JSON的來源檔案。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL節點ID]</td>
      <td>
        <p>輸入您希望模組傳回並轉換的節點</p>
        <p>針對您要傳回的每個節點，按一下 <b>[！UICONTROL新增]</b> 並輸入節點的文字。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL版本ID]</td>
      <td>輸入或對應您希望模組傳回的檔案版本。 對於目前的模組，請將此欄位留空。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL深度]</td>
      <td>
        <p>輸入或對應整數，該整數代表您要傳回結果的檔案樹狀結構深度。 </p>
        <div class="example"><span class="autonumber"><span><b>範例: </b></span></span>
          <ul>
            <li>
              <p>若要僅傳回頁面，請輸入 <code>1</code>.</p>
            </li>
            <li>
              <p>若要傳回頁面和頂層物件，請輸入 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>若要傳回所有節點，請將此欄位留空。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL幾何]</td>
      <td>若要傳回向量資料，請輸入 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL外掛程式資料]</td>
      <td>外掛程式ID和/或「共用」字串的逗號分隔清單。 由這些外掛程式撰寫的檔案中存在的任何資料，都會包含在pluginData和sharedPluginData屬性的結果中。</td>
    </tr>
  </tbody>
</table>


##### 取得檔案或影像：影像

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL檔案索引鍵]</td>
      <td>選取您要傳回JSON的來源檔案。</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>節點識別碼]</td>
      <td>
        <p>輸入您希望模組呈現的節點。</p>
        <p>針對您要呈現的每個節點，按一下 <b>[！UICONTROL新增]</b> 並輸入節點的文字。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL縮放]</td>
      <td>若要縮放影像，請輸入或對應縮放比例。 此數字必須介於0.01和4之間。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL格式]</td>
      <td>
        <p>選取影像輸出的格式。</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROLSVG — 包含ID]</td>
      <td>啟用此選項可包含所有SVG元素的ID屬性。 預設： [！UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROLSVG — 簡化筆畫]</td>
      <td>啟用此選項可簡化內/外筆畫，並儘可能使用筆畫屬性，而非 &lt;mask&gt;. 預設： [！UICONTROL true]。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL使用絕對界限]</td>
      <td>啟用此選項可使用節點的完整尺寸，無論節點是否裁切或周圍空間為空白。 使用此項可匯出文位元組點而不進行裁切。 預設： [！UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL版本ID]</td>
      <td>輸入或對應您希望模組傳回的檔案版本。 對於目前的模組，請將此欄位留空。</td>
    </tr>
  </tbody>
</table>

##### 取得檔案或影像：影像填色

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL檔案索引鍵]</td>
      <td>選取您要傳回JSON的來源檔案。</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL 列出檔案版本記錄]

此搜尋模組會傳回中單一檔案的版本記錄 [!UICONTROL 圖].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    <tr>
      <td role="rowheader">[！UICONTROL檔案ID]</td>
      <td>
        <p>輸入或對應您要擷取版本記錄的檔案的檔案ID。 </p>
        <ul>
          <li>
            <p>如果您不知道檔案的ID，請按一下 <b>[！UICONTROL尋找檔案]</b> 並輸入或對應與檔案相關聯的專案ID，然後選取檔案。</p>
          </li>
          <li>
            <p>如果您嘗試尋找檔案的ID但不知道專案的ID，請按一下 <b>[！UICONTROL尋找專案]</b> 並輸入或對應擁有檔案相關聯專案的團隊ID。 選取專案，然後選取檔案。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出專案檔案]

此搜尋模組會傳回指定專案中所有檔案的清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL檔案ID]</td>
      <td>
        <p>輸入或對映您要擷取檔案的專案ID。 </p>
        <ul>
          <li>
            <p>如果您不知道專案的ID，請按一下 <b>[！UICONTROL尋找專案]</b> 並輸入或對應專案相關團隊的ID，然後選取專案。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出專案]

此搜尋模組會傳回指定團隊中所有專案的清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL團隊ID]</td>
      <td>輸入或對應您要擷取檔案的專案ID。 團隊ID可在菲格瑪團隊頁面的URL中找到</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</td>
    </tr>
  </tbody>
</table>


### 元件和樣式

#### [!UICONTROL 取得樣式或元件]

此動作模組會擷取單一樣式或元件，或一組樣式或元件。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[！UICONTROL Object&gt;鍵]</td>
      <td>輸入您要擷取之物件的金鑰（唯一識別碼）。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL團隊ID]</td>
      <td>輸入或對應與一個或多個記錄相關聯的團隊ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL頁面大小]</td>
      <td>輸入或對應每頁要傳回的數目或結果。 預設值： 30。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL After]</td>
      <td>
        <p>輸入或對映結果編號，之後開始擷取結果。 這可以與[！UICONTROL頁面大小]欄位結合以分頁結果。</p>
        <p>此值未對應至物件ID。</p>
        <p>此欄位不能與[！UICONTROL Before]欄位結合使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Before]</td>
      <td>
        <p>輸入或對應開始擷取結果之前的結果編號。 這可以與[！UICONTROL頁面大小]欄位結合以分頁結果。</p>
        <p>此值未對應至物件ID。</p>
        <p>此欄位不能與[！UICONTROL After]欄位結合使用。</p>
      </td>
    </tr>
  </tbody>
</table>


### 其他

* [進行API呼叫](#make-an-api-call)

* [觀看活動](#watch-events)


#### [!UICONTROL 進行API呼叫]

此動作模組可讓您對Figma API發出自訂的已驗證呼叫，而不需思考驗證問題。 如此一來，您就可以建立其他Figma模組無法完成的資料流程自動化。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL連線]</td>
      <td> <p>如需有關連線您的電腦的指示， [!DNL Figma] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>輸入相對於 <code>https://api.figma.com/v1/</code>.</p>
        <p>例如： <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL方法]</td>
      <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL標頭]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 為您新增授權標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查詢字串]</td>
      <td>
        <p>以標準JSON物件的形式新增API呼叫的查詢。</p>
        <p>例如： <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL內文]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 觀看活動]

當您的團隊的特定團隊發生下列其中一項事件時，此觸發模組就會啟動一個案例： [!DNL Figma] 團隊空間

* 檔案更新

* 檔案版本更新

* 檔案刪除

* 程式庫發佈

* 檔案註解

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Webhook]</td>
      <td>
        <p>選取模組要監視的webhook。</p>
        <p>若要新增新的webhook：</p>
        <ol>
          <li value="1">
            <p>按一下 <b>[！UICONTROL新增]</b> [！UICONTROL Webhook]欄位旁邊。</p>
          </li>
          <li value="2">
            <p>選取您要用於此webhook的連線。 如需有關連線您的電腦的指示， [!DNL Figma] [！UICONTROL Workfront Fusion]的帳戶，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[！UICONTROL Adobe Workfront Fusion]的連線 — 基本指示。</a></p>
          </li>
          <li value="3">
            <p>選取您要模組觀看的事件型別。</p>
          </li>
          <li value="4">
            <p>輸入您希望webhook觀看其事件的團隊ID。</p>
          </li>
          <li value="5">
            <p>輸入您希望webhook觀看的事件的[！UICONTROL狀態]或[！UICONTROL說明]。</p>
          </li>
          <li value="6">
            <p>按一下 <b>[！UICONTROL儲存]</b> 以儲存webhook並返回模組。</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
