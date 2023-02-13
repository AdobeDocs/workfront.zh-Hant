---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Figma模組
description: 使用 [!DNL Adobe Workfront Fusion] 圖模組，您可以檢索注釋、檔案、檔案版本或項目清單。 您也可以張貼留言或呼叫Figma API。
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 1%

---

# [!DNL Figma] 模組

使用 [!DNL Adobe Workfront Fusion] [!DNL Figma] 模組，您可以檢索注釋、檔案、檔案版本或項目清單。 您也可以張貼留言或呼叫 [!DNL Figma] API。

如果您需要建立案例的相關指示，請參閱 [建立藍本](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
      <td>
        <p>[!UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
      <td>
        <p>[!UICONTROL計畫]、[!UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合）</p>
      </td>
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

使用 [!DNL Figma] 模組，您必須 [!DNL Figma] 帳戶。

## [!DNL Figma] 模組及其欄位

設定時 [!DNL Figma] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Figma] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [註解](#comments)

* [專案和檔案](#projects-and-files)

* [元件和樣式](#components-and-styles)

* [其他](#other)


### 註解

* [刪除注釋](#delete-a-comment)

* [列出注釋](#list-comments)

* [張貼留言](#post-a-comment)


#### [!UICONTROL 刪除注釋]

此動作模組會從檔案中刪除單一註解。

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL檔案ID]</td>
      <td>輸入或映射要從中添加刪除注釋的檔案的檔案ID。 </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL注釋]</td>
      <td>輸入要刪除的注釋文本。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出注釋]

此搜尋模組會列出中附加至單一檔案的所有註解 [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL檔案ID]</td>
      <td>
        <p>輸入或映射要檢索注釋的檔案的檔案ID。 </p>
        <ul>
          <li>
            <p>如果您不知道ID，請按一下 <b>[!UICONTROL查找檔案]</b> 並輸入或映射與該檔案關聯的項目的ID，然後選擇該檔案。</p>
          </li>
          <li>
            <p>如果您不知道專案的ID，請按一下 <b>[!UICONTROL查找項目]</b> 輸入或映射擁有與檔案關聯的項目的團隊的ID，然後選擇項目，然後選擇該檔案。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大注釋數。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 張貼留言]

此動作模組會將註解發佈至Figma檔案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL檔案ID]</td>
      <td>
        <p>輸入或映射要發佈評論的檔案的檔案ID。 </p>
        <ul>
          <li>
            <p>如果您不知道檔案的ID，請按一下 <b>[!UICONTROL查找檔案]</b> 並輸入或映射與該檔案關聯的項目的ID，然後選擇該檔案。</p>
          </li>
          <li>
            <p>如果您嘗試尋找檔案的ID，但不知道專案的ID，請按一下 <b>[!UICONTROL查找項目]</b> 並輸入或映射擁有與檔案關聯的項目的團隊的ID。 選取專案，然後選取檔案。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL注釋]</td>
      <td>輸入注釋的文本。</td>
    </tr>
  </tbody>
</table>


### 專案和檔案

* [取得檔案或影像](#get-a-file-or-image)

* [列出檔案版本歷史記錄](#list-file-version-history)

* [列出項目檔案](#list-project-files)

* [列出專案](#list-projects)


#### [!UICONTROL 取得檔案或影像]

此動作模組會從Figma程式庫擷取單一檔案或影像

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL對象類型]</td>
      <td>
        <p>選擇要檢索的對象類型。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL檔案]</b>
            </p>
            <p>模組會傳回[!UICONTROL索引鍵]所參考的檔案，做為JSON物件。 可從任何Figma檔案URL中剖析檔案鍵值。</p>
            <p>如需欄位，請參閱 <a href="#Get2" class="MCXref xref" >[!UICONTROL獲取檔案或影像：檔案]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL檔案節點]</b>
            </p>
            <p>傳回ID作為JSON物件參考的節點。 節點會從 [!DNL Figma] [!UICONTROL密鑰]引用的檔案。</p>
            <p>如需欄位，請參閱 <a href="#Get3" class="MCXref xref" >[!UICONTROL獲取檔案或影像：檔案節點]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL影像]</b>
            </p>
            <p>模組從檔案轉譯影像。</p>
            <p>如需欄位，請參閱 <a href="#Get4" class="MCXref xref" >[!UICONTROL獲取檔案或影像：影像]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL影像填充]</b>
            </p>
            <p>該模組返回文檔中影像填充中所有影像的下載連結。 影像填充是 [!DNL Figma] 代表任何使用者提供的影像。 將影像拖曳至 [!DNL Figma], [!DNL Figma] 使用表示影像的單個填充建立一個矩形，用戶能夠轉換該矩形（和填充的屬性）。</p>
            <p>如需欄位，請參閱 <a href="#Get5" class="MCXref xref" >[!UICONTROL獲取檔案或影像：影像填充]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 獲取檔案或影像：檔案]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL檔案鍵]</td>
      <td>選取要傳回JSON的檔案。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL版本ID]</td>
      <td>輸入或映射要模組返回的檔案版本。 對於目前模組，將此欄位留空。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL節點ID]</td>
      <td>
        <p>要僅返回文檔的子集，請輸入希望模組返回的節點。 模組會傳回列出的節點、其子節點，以及根節點與列出節點之間的任何項目。</p>
        <p>針對您要傳回的每個節點，按一下 <b>[!UICONTROL添加]</b> 並輸入節點的文本。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL深度]</td>
      <td>
        <p>輸入或映射一個整數，該整數表示要在文檔樹中返回結果的深度。 </p>
        <div class="example"><span class="autonumber"><span><b>範例: </b></span></span>
          <ul>
            <li>
              <p>若要僅傳回頁面，請輸入 <code>1</code>.</p>
            </li>
            <li>
              <p>要返回頁面和頂級對象，請輸入 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>若要傳回所有節點，請將此欄位留空。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL幾何]</td>
      <td>若要傳回響量資料，請輸入 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL外掛程式資料]</td>
      <td>外掛程式ID和/或字串"[!UICONTROL shared]"的逗號分隔清單。 這些外掛程式所撰寫的檔案中出現的任何資料都會包含在 <code>pluginData</code> 和 <code>sharedPluginData</code> 屬性。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL分支資料]</td>
      <td>啟用此選項可返回所請求檔案的分支元資料。 如果檔案是分支，則主檔案的索引鍵會包含在傳回的回應中。 如果檔案有分支，則其中繼資料會包含在傳回的回應中。 預設: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 獲取檔案或影像：檔案節點]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL檔案鍵]</td>
      <td>選取要傳回JSON的檔案。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL節點ID]</td>
      <td>
        <p>輸入要模組返回和轉換的節點</p>
        <p>針對您要傳回的每個節點，按一下 <b>[!UICONTROL添加]</b> 並輸入節點的文本。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL版本ID]</td>
      <td>輸入或映射要模組返回的檔案版本。 對於目前模組，將此欄位留空。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL深度]</td>
      <td>
        <p>輸入或映射一個整數，該整數表示要在文檔樹中返回結果的深度。 </p>
        <div class="example"><span class="autonumber"><span><b>範例: </b></span></span>
          <ul>
            <li>
              <p>若要僅傳回頁面，請輸入 <code>1</code>.</p>
            </li>
            <li>
              <p>要返回頁面和頂級對象，請輸入 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>若要傳回所有節點，請將此欄位留空。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL幾何]</td>
      <td>若要傳回響量資料，請輸入 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL外掛程式資料]</td>
      <td>外掛程式ID和/或字串「共用」的逗號分隔清單。 這些外掛程式所撰寫的檔案中出現的任何資料都會包含在pluginData和sharedPluginData屬性中。</td>
    </tr>
  </tbody>
</table>


##### 獲取檔案或影像：影像

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL檔案鍵]</td>
      <td>選取要傳回JSON的檔案。</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>節點ID]</td>
      <td>
        <p>輸入要模組呈現的節點。</p>
        <p>對於要呈現的每個節點，按一下 <b>[!UICONTROL添加]</b> 並輸入節點的文本。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL比例]</td>
      <td>要縮放影像，請輸入或映射縮放因子。 此數字必須介於0.01和4之間。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL格式]</td>
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
      <td role="rowheader">[!UICONTROLSVG — 包含ID]</td>
      <td>啟用此選項可包含所有SVG元素的ID屬性。 預設值：[!UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROLSVG — 簡化描邊]</td>
      <td>啟用此選項可簡化內/外描邊，並盡可能使用描邊屬性，而非 &lt;mask&gt;. 預設值：[!UICONTROL true]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL使用絕對界]</td>
      <td>無論節點是否被裁切或周圍的空白為何，啟用此選項都可使用節點的完整維度。 使用它導出文本節點而不進行裁切。 預設值：[!UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL版本ID]</td>
      <td>輸入或映射要模組返回的檔案版本。 對於目前模組，將此欄位留空。</td>
    </tr>
  </tbody>
</table>

##### 獲取檔案或影像：影像填充

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL檔案鍵]</td>
      <td>選取要傳回JSON的檔案。</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL 列出檔案版本歷史記錄]

此搜尋模組會傳回中單一檔案的版本記錄 [!UICONTROL 菲格馬].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL檔案ID]</td>
      <td>
        <p>輸入或映射要檢索版本歷史記錄的檔案的檔案ID。 </p>
        <ul>
          <li>
            <p>如果您不知道檔案的ID，請按一下 <b>[!UICONTROL查找檔案]</b> 並輸入或映射與該檔案關聯的項目的ID，然後選擇該檔案。</p>
          </li>
          <li>
            <p>如果您嘗試尋找檔案的ID，但不知道專案的ID，請按一下 <b>[!UICONTROL查找項目]</b> 並輸入或映射擁有與檔案關聯的項目的團隊的ID。 選取專案，然後選取檔案。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出項目檔案]

此搜索模組返回指定項目中所有檔案的清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL檔案ID]</td>
      <td>
        <p>輸入或映射要檢索檔案的項目ID。 </p>
        <ul>
          <li>
            <p>如果您不知道專案的ID，請按一下 <b>[!UICONTROL查找項目]</b> 並輸入或映射項目關聯的團隊的ID，然後選擇項目。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出專案]

此搜索模組返回指定團隊內所有項目的清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL團隊ID]</td>
      <td>輸入或映射要檢索檔案的項目的項目ID。 可在團隊頁面的URL（圖表）中找到團隊ID</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td>
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
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL對象&gt;鍵]</td>
      <td>輸入要檢索的對象的鍵（唯一標識符）。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL團隊ID]</td>
      <td>輸入或映射與記錄或記錄關聯的團隊的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL頁面大小]</td>
      <td>輸入或映射每頁要返回的數字或結果。 預設值：30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>輸入或映射結果的編號，在此編號之後開始檢索結果。 這可以與[!UICONTROL頁面大小]欄位結合，以分頁結果。</p>
        <p>此值與物件ID不對應。</p>
        <p>此欄位不能與[!UICONTROL Before]欄位組合使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL之前]</td>
      <td>
        <p>輸入或映射要開始檢索結果的結果編號。 這可以與[!UICONTROL頁面大小]欄位結合，以分頁結果。</p>
        <p>此值與物件ID不對應。</p>
        <p>此欄位不能與[!UICONTROL After]欄位組合使用。</p>
      </td>
    </tr>
  </tbody>
</table>


### 其他

* [進行API呼叫](#make-an-api-call)

* [觀看事件](#watch-events)


#### [!UICONTROL 進行API呼叫]

此動作模組可讓您對Figma API進行自訂已驗證呼叫，而無須考慮驗證。 這樣，您可以建立資料流自動化，而其他Figma模組無法完成此操作。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>有關連接 [!DNL Figma] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>輸入相對於的路徑 <code>https://api.figma.com/v1/</code>.</p>
        <p>例如： <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL方法]</td>
      <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL標題]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標題。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 為您添加授權標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL查詢字串]</td>
      <td>
        <p>以標準JSON物件的形式新增API呼叫的查詢。</p>
        <p>例如： <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL正文]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 觀看事件]

此觸發模組會在您的 [!DNL Figma] 團隊空間

* 檔案更新

* 檔案版本更新

* 檔案刪除

* 程式庫發佈

* 檔案注釋

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>選取模組監視的網頁連結。</p>
        <p>要添加新網頁鈎點：</p>
        <ol>
          <li value="1">
            <p>按一下 <b>[!UICONTROL添加]</b> 欄位旁邊。</p>
          </li>
          <li value="2">
            <p>選擇要用於此Webhook的連接。 有關連接 [!DNL Figma] 帳戶至[!UICONTROL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!UICONTROL Adobe Workfront Fusion]的連線 — 基本說明。</a></p>
          </li>
          <li value="3">
            <p>選取您要模組監看的事件類型。</p>
          </li>
          <li value="4">
            <p>輸入您希望Webhook監視其事件的團隊的ID。</p>
          </li>
          <li value="5">
            <p>輸入希望Webhook監視的事件的[!UICONTROL狀態]或[!UICONTROL描述]。</p>
          </li>
          <li value="6">
            <p>按一下 <b>[!UICONTROL保存]</b> 儲存webhook並返回模組。</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
