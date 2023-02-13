---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud Libraries模組
description: 使用 [!DNL Adobe Workfront Fusion Adobe Creative Cloud] 程式庫模組，您可以在建立或更新元素或程式庫時啟動案例。 您也可以上傳、擷取、封存或列出元素，或對 [!DNL Adobe Creative Cloud Libraries] API。
author: Becky
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# Adobe Creative Cloud Libraries模組

使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] 模組，您可以在建立或更新元素或程式庫時啟動案例。 您也可以上傳、擷取、封存或列出元素，或對 [!DNL Adobe Creative Cloud Libraries] API。

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

使用 [!DNL Adobe Creative Cloud Libraries] 模組，您必須 [!UICONTROL Adobe Creative Cloud] 帳戶。

## [!UICONTROL Adobe Creative Cloud Libraries] 模組及其欄位

設定時 [!UICONTROL Adobe Creative Cloud Libraries] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Adobe Creative Cloud Libraries] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [元素](#elements)

* [程式庫](#libraries)

* [其他](#other)


### 元素

* [[!UICONTROL 封存元素]](#archive-an-element)

* [[!UICONTROL 取得元素]](#get-an-element)

* [[!UICONTROL 清單元素]](#list-elements)

* [[!UICONTROL 上傳元素]](#upload-an-element)

* [!UICONTROL [在庫中觀看新元素]](#watch-new-element-in-library)

* [[!UICONTROL 觀看更新的元素]](#watch-updated-elements)


#### [!UICONTROL 封存元素]

此動作模組會封存程式庫中的元素。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL庫ID]</td>
      <td >選取包含您要封存之元素的程式庫。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL元素ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">選取您要封存的元素。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得元素]

此動作模組會從程式庫中傳回單一元素。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL庫ID]</td>
      <td >選取包含您要擷取之元素的程式庫。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL元素ID]</td>
      <td>輸入或對應您要擷取之元素的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL選擇器]</td>
      <td>
        <p>選取模組傳回的資訊類型。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL預設值]</b>
            </p>
            <p>基礎資料</p>
          </li>
          <li>
            <p><b>[!UICONTROL詳細資訊]</b>
            </p>
            <p>所有可用資料</p>
          </li>
          <li>
            <p><b>[!UICONTROL表示]</b>
            </p>
            <p>與程式庫元素相關聯的資產平面化清單</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 清單元素]

此動作模組會擷取程式庫中的元素清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL庫ID]</td>
      <td >選取要列出元素的程式庫。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL順序依]</td>
      <td>選擇要按名稱排序結果還是按上次修改元素的日期排序結果。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL類型]</td>
      <td >輸入MIME類型，將結果限制為以指定MIME類型標識的元素。 範例: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL選擇器]</td>
      <td>
        <p>選取模組傳回的資訊類型。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL預設值]</b>
            </p>
            <p>基礎資料</p>
          </li>
          <li>
            <p><b>[!UICONTROL詳細資訊]</b>
            </p>
            <p>所有可用資料</p>
          </li>
          <li>
            <p><b>[!UICONTROL表示]</b>
            </p>
            <p>與程式庫元素相關聯的資產平面化清單</p>
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

#### [!UICONTROL 上傳元素]

此動作模組會將小型檔案資產上傳至現有程式庫。 檔案大小上限為1 GB。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL庫ID]</td>
      <td >選取要列出元素的程式庫。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL調用模式]</td>
      <td>
        <p>選取處理模式，以使用叫用此請求處理。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL同步]</b>
            </p>
            <p>API呼叫會同步處理。 處理完成時會傳送回應（除非呼叫逾時）。</p>
          </li>
          <li>
            <p><b>[!UICONTROL非同步]</b>
            </p>
            <p>系統會立即傳回非同步監視回應，且以非同步方式處理要求。 呼叫負責輪詢端點直到完成。</p>
          </li>
          <li>
            <p><b>[!UICONTROL同步，async]</b> （預設）</p>
            <p>嘗試同步處理請求。 當處理延長超過5000毫秒時，會傳回非同步監視器回應。 在請求完成之前，應輪詢監視器URL。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL類型檔案]</td>
      <td >輸入或映射已上載檔案的MIME類型。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL源檔案]</td>
      <td>
        <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 在程式庫中觀看新元素]

元素新增至程式庫時，此觸發模組會啟動案例。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL庫ID]</td>
      <td >選取您要監看更新元素的程式庫。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 觀看更新的元素]

此觸發器模組會在程式庫中的元素更新時啟動案例。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL庫ID]</td>
      <td >選取您要監看新元素的程式庫。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td>
    </tr>
  </tbody>
</table>

### 程式庫

* [[!UICONTROL 觀看新程式庫]](#watch-new-libraries)

* [[!UICONTROL 觀看更新的程式庫]](#watch-updated-libraries)


#### [!UICONTROL 觀看新程式庫]

此觸發模組會在建立新程式庫時啟動案例。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 觀看更新的程式庫]

此觸發模組會在更新現有程式庫時啟動案例。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關連接 [!DNL Adobe Creative Cloud] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本說明。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td>
    </tr>
  </tbody>
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此模組會對 [!DNL Adobe Creative Cloud Libraries] API。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td> <p>如需將Adobe Creative Cloud帳戶連結至Workfront Fusion的指示，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本指示。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>輸入相對於的路徑 <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>例如 <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API版本]</td>
      <td>
        <p>選取 [!DNL Adobe Analytics] 您要連線的API。</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL方法]</td>
      <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL標題]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標題。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion會為您新增授權標頭。</p>
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
       <tr>
      <td role="rowheader">[!UICONTROL上載臨時文檔]</td>
      <td>
      <p>如果要上載臨時文檔，請輸入要上載的文檔的源檔案。</p>
      <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p>
    </td>
    </tr>

</tbody>
</table>
