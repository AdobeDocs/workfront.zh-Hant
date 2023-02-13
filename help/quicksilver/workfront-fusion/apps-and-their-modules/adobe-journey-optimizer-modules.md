---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Adobe Journey Optimizer]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] 模組

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Adobe Journey Optimizer]，並將其連接至多個協力廠商應用程式和服務。 [!DNL Adobe Journey Optimizer] 模組可讓您建立、讀取、更新或刪除記錄，或執行自訂API呼叫 [!DNL Adobe Journey Optimizer] API。


如果您需要建立案例的相關指示，請參閱 [建立藍本](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table>
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

您可以使用 [!DNL Adobe Journey Optimizer] 連接器，您必須確保符合下列必要條件：

* 您必須具有活動 [!DNL Adobe Journey Optimizer] 帳戶。

## 建立連線至 [!DNL Adobe Journey Optimizer]

為 [!DNL Adobe Journey Optimizer] 模組：

1. 在任何 [!DNL Adobe Journey Optimizer] 模組，按一下 **[!UICONTROL 新增]** 的下界。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL連接名]</td>
          <td>
            <p>輸入此連接的名稱。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL客戶端ID]</td>
          <td>輸入 [!DNL Adobe] [!UICONTROL客戶端ID]。 您可在 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL客戶端密碼]</td>
          <td>輸入 [!DNL Adobe] [!UICONTROL客戶端密碼]。 您可在 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL技術帳戶ID]</td>
          <td>輸入 [!DNL Adobe] [!UICONTROL技術帳戶ID]。 您可在 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL組織ID]</td>
          <td>輸入 [!DNL Adobe] [!UICONTROL組織ID]。 您可在 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL元作用域]</td>
          <td>
            輸入連接所需的任何元作用域。
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL私鑰]</td>
          <td>
            <p>在 [!DNL Adobe Developer Console]. </p>
            <p>若要擷取私密金鑰或憑證：</p>
            <ol>
              <li value="1">
                <p>按一下 <b>[!UICONTROL提取]</b>.</p>
              </li>
              <li value="2">
                <p>選取要擷取的檔案類型。</p>
              </li>
              <li value="3">
                <p>選取包含私密金鑰或憑證的檔案。</p>
              </li>
              <li value="4">
                <p>輸入檔案的密碼。</p>
              </li>
              <li value="5">
                <p>按一下 <b>[!UICONTROL保存]</b> 以解壓縮檔案並返回連接設定。</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## [!DNL Adobe Journey Optimizer] 模組及其欄位

設定時 [!DNL Adobe Journey Optimizer] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Adobe Journey Optimizer] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)

### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)

#### [!UICONTROL 建立記錄]

此動作模組會建立版位、決策規則、標籤、個人化優惠方案、集合或備援優惠方案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
     <td>有關建立連接的說明 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立連線至 [!DNL Adobe Journey Optimizer]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL記錄類型]
      </td>
      <td>
        選擇要建立的記錄類型
        <ul>
        <li><b>[!UICONTROL位置]</b>:繼續 <a href="#placement-fields" >[!UICONTROL位置]欄位</a>.</li>
        <li><b>[!UICONTROL決策規則]</b>:繼續 <a href="#decision-rule-fields" >[!UICONTROL決策規則]欄位</a>.</li>
        <li><b>[!UICONTROL決策]</b>:繼續 <a href="#decision-fields" >[!UICONTROL決策]欄位</a>.</li>
        <li><b>[!UICONTROL標籤]</b>:繼續 <a href="#tag-fields" >[!UICONTROL標籤]欄位</a>.</li>
        <li><b>[!UICONTROL集合]</b>:繼續 <a href="#collection-fields" >[!UICONTROL集合]欄位</a>.</li>
        <li><b>[!UICONTROL回退優惠方案]</b>:繼續 <a href="#fallback-offer-fields" >[!UICONTROL回退優惠方案]欄位</a>.</li>
        <li><b>[!UICONTROL個人化優惠方案]</b>:繼續 <a href="#personalized-offer-fields" >[!UICONTROL個人化優惠方案]欄位</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 版位] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
     <td>輸入或映射投放位置的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL描述]
      </td>
      <td>輸入或映射版位的說明。
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 決策規則] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
     <td>輸入或映射說明規則的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL描述]
      </td>
      <td>輸入或映射決策規則的說明。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL條件]
      </td>
      <td>輸入或對應決策規則的條件。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 決策] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
     <td>輸入或映射說明規則的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL狀態]</td>
      <td>選擇決策的狀態。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL開始日期]</td>
      <td><p>輸入或映射決策的開始日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL結束日期]</td>
      <td><p>輸入或映射決策的結束日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL版位]</td>
      <td>選取要新增至此決策的版位
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL集合]</td>
      <td>選取包含此決策將考慮之選件的選件集合。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL回退優惠方案]</td>
      <td>選取要呈現給不符合此決策規則之客戶的備援優惠方案。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 標籤] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
     <td>輸入或映射標籤的名稱。</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 集合] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
     <td>輸入或映射集合的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL篩選器類型]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL元素]
      </td>
      <td>選取要包含在集合中的標籤。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 備援優惠方案] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
     <td>輸入或對應備援優惠方案的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL狀態]
      </td>
      <td> 選取備援優惠方案的狀態。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL位置]
      </td>
      <td>輸入或對應備援優惠方案的版位。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 個人化優惠方案] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
     <td>輸入或映射說明規則的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL狀態]</td>
      <td>選擇決策的狀態。
      </td>
    </tr>
    <tr>
      <td role="rowheader">版位</td>
      <td>選取個人化優惠方案的版位。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL開始日期]</td>
      <td><p>輸入或對應個人化優惠方案的開始日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL結束日期]</td>
      <td><p>輸入或對應個人化優惠方案的結束日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL決策規則]</td>
      <td>選取要新增至此個人化優惠方案的決策規則。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL優先順序]</td>
      <td>選取此選件的優先順序。 優先順序會影響是否會呈現此選件，而非其他選件。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL限定約束]</td>
      <td>輸入或對應此選件的呈現次數。
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
     <td>有關建立連接的說明 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立連線至 [!DNL Adobe Journey Optimizer]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL記錄類型]
      </td>
      <td>
        選擇要刪除的記錄類型
        <ul>
        <li>[!UICONTROL位置]</li>
        <li>[!UICONTROL決策規則]</li>
        <li>[!UICONTROL決策]</li>
        <li>[!UICONTROL標籤]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL回退優惠方案]</li>
        <li>[!UICONTROL個人化優惠方案]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision Rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalizated offer]
      </td>
      <td>
        選擇要刪除的記錄。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 進行自訂API呼叫]

此模組會對 [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL連接]</td>
     <td>有關建立連接的說明 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立連線至 [!DNL Adobe Journey Optimizer]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入與{baseURL}相對的路徑，開頭為<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL方法]</p>
      </td>
      <td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL標題]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標題。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion會自動新增授權標頭和x-api金鑰標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL查詢字串]  </td>
      <td>
        <p>輸入請求查詢字串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL正文]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>輸入希望模組在一個執行週期中返回的最大結果數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL連接]</td>
     <td>有關建立連接的說明 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立連線至 [!DNL Adobe Journey Optimizer]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL記錄類型]
      </td>
      <td>
        選擇要刪除的記錄類型
        <ul>
        <li>[!UICONTROL位置]</li>
        <li>[!UICONTROL決策規則]</li>
        <li>[!UICONTROL決策]</li>
        <li>[!UICONTROL標籤]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL回退優惠方案]</li>
        <li>[!UICONTROL個人化優惠方案]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision Rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalizated offer]
      </td>
      <td>
        選擇要刪除的記錄。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 更新記錄]

此動作模組會建立版位、決策、決策規則、標籤、個人化優惠方案、集合或備援優惠方案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL連接]</td>
     <td>有關建立連接的說明 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立連線至 [!DNL Adobe Journey Optimizer]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL記錄類型]
      </td>
      <td>
        選擇要更新的記錄類型
        <ul>
        <li>[!UICONTROL位置]</li>
        <li>[!UICONTROL決策規則]</li>
        <li>[!UICONTROL決策]</li>
        <li>[!UICONTROL標籤]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL回退優惠方案]</li>
        <li>[!UICONTROL個人化優惠方案]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision Rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalizated offer]
      </td>
      <td>
        選擇要更新的記錄。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL欄位]
      </td>
      <td>針對您要更新的每個欄位：
      <ol>
      <li>按一下 <b>[!UICONTROL添加]</b>.</li>
      <li>選取您要新增、取代或移除值。</li>
      <li>輸入要更新的欄位。</li>
      <li>輸入欄位的新值。</li>
      </td>
    </tr>

</tbody>
</table>


### 搜尋

#### [!UICONTROL 清單記錄]

此搜尋模組會列出所選類型的記錄，並根據您指定的條件傳回結果。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL連接]</td>
     <td>有關建立連接的說明 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立連線至 [!DNL Adobe Journey Optimizer]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL記錄類型]</p>
      </td>
      <td>
        <p>選擇要列出的記錄類型。</p>
        <ul>
        <li>[!UICONTROL位置]</li>
        <li>[!UICONTROL決策規則]</li>
        <li>[!UICONTROL決策]</li>
        <li>[!UICONTROL標籤]</li>
        <li>[!UICONTROL集合]</li>
        <li>[!UICONTROL回退優惠方案]</li>
        <li>[!UICONTROL個人化優惠方案]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL查詢運算子]</p>
      </td>
      <td>
        <p>選取要套用至查詢中參數的運算子</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL欄位]</td>
      <td><p>如果要將搜索限制為特定欄位，請輸入欄位。 對於要限制搜索的每個欄位，按一下[!UICONTROL添加項]並輸入欄位的名稱。</p><p>路徑運算式是以點分隔路徑的形式，例如 <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL順序依] </td>
      <td>輸入或映射要按其排序結果的屬性。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL順序方向]</td>
   <td>選擇要按升序還是降序排序結果。
    </td>
     </tr>
  </tbody>
</table>
