---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer模組
description: 在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Adobe Journey Optimizer]，並連結至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] 模組

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Adobe Journey Optimizer]，並連結至多個協力廠商應用程式和服務。 [!DNL Adobe Journey Optimizer] 模組可讓您建立、讀取、更新或刪除記錄，或執行自訂API呼叫至 [!DNL Adobe Journey Optimizer] API。


如果您需要有關建立情境的指示，請參閱 [建立情境](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table>
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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td>
    </tr>
  </tbody>
</table>


若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

開始使用 [!DNL Adobe Journey Optimizer] 聯結器時，您必須確定符合下列先決條件：

* 您必須擁有使用中 [!DNL Adobe Journey Optimizer] 帳戶。

## 建立與的連線 [!DNL Adobe Journey Optimizer]

若要為建立連線，請執行下列步驟： [!DNL Adobe Journey Optimizer] 模組：

1. 在任何 [!DNL Adobe Journey Optimizer] 模組，按一下 **[!UICONTROL 新增]** ，位於「連線」方塊旁。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[！UICONTROL連線名稱]</td>
          <td>
            <p>輸入此連線的名稱。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者端ID]</td>
          <td>輸入您的 [!DNL Adobe] [！UICONTROL使用者端識別碼]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者端密碼]</td>
          <td>輸入您的 [!DNL Adobe] [！UICONTROL使用者端密碼]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL技術帳戶ID]</td>
          <td>輸入您的 [!DNL Adobe] [！UICONTROL技術帳戶ID]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL組織ID]</td>
          <td>輸入您的 [!DNL Adobe] [！UICONTROL組織識別碼]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL中繼範圍]</td>
          <td>
            輸入連線所需的任何中繼範圍。
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL私密金鑰]</td>
          <td>
            <p>輸入在中建立您的認證時產生的私密金鑰 [!DNL Adobe Developer Console]. </p>
            <p>若要擷取您的私密金鑰或憑證：</p>
            <ol>
              <li value="1">
                <p>按一下 <b>[！UICONTROL Extract]</b>.</p>
              </li>
              <li value="2">
                <p>選取要解壓縮的檔案型別。</p>
              </li>
              <li value="3">
                <p>選取包含私密金鑰或憑證的檔案。</p>
              </li>
              <li value="4">
                <p>輸入檔案的密碼。</p>
              </li>
              <li value="5">
                <p>按一下 <b>[！UICONTROL儲存]</b> 以擷取檔案並返回連線設定。</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## [!DNL Adobe Journey Optimizer] 模組及其欄位

當您設定 [!DNL Adobe Journey Optimizer] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Adobe Journey Optimizer] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)

### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)

#### [!UICONTROL 建立記錄]

此動作模組會建立位置、決定規則、標籤、個人化優惠、系列或遞補優惠。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有關建立與的連線的指示 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與的連線 [!DNL Adobe Journey Optimizer]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL記錄型別]
      </td>
      <td>
        選取您要建立的記錄型別
        <ul>
        <li><b>[！UICONTROL位置]</b>：繼續至 <a href="#placement-fields" >[！UICONTROL位置]欄位</a>.</li>
        <li><b>[！UICONTROL決定規則]</b>：繼續至 <a href="#decision-rule-fields" >[！UICONTROL決定規則]欄位</a>.</li>
        <li><b>[！UICONTROL決定]</b>：繼續至 <a href="#decision-fields" >[！UICONTROL決定]欄位</a>.</li>
        <li><b>[！UICONTROL標籤]</b>：繼續至 <a href="#tag-fields" >[！UICONTROL標籤]欄位</a>.</li>
        <li><b>[！UICONTROL集合]</b>：繼續至 <a href="#collection-fields" >[！UICONTROL集合]欄位</a>.</li>
        <li><b>[！UICONTROL遞補優惠]</b>：繼續至 <a href="#fallback-offer-fields" >[！UICONTROL遞補優惠]欄位</a>.</li>
        <li><b>[！UICONTROL個人化優惠]</b>：繼續至 <a href="#personalized-offer-fields" >[！UICONTROL個人化優惠]欄位</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 刊登] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
     <td>輸入或對映位置的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL說明]
      </td>
      <td>輸入或對映位置的說明。
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 決定規則] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
     <td>輸入或對應說明規則的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL說明]
      </td>
      <td>輸入或對應決定規則的說明。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL條件]
      </td>
      <td>輸入或對映決策規則的條件。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 決定] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
     <td>輸入或對應說明規則的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL狀態]</td>
      <td>選取決定的狀態。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL開始日期]</td>
      <td><p>輸入或對應決定的開始日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL結束日期]</td>
      <td><p>輸入或對應決定的結束日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL Placements]</td>
      <td>選取要新增至此決定的刊登版位
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL集合]</td>
      <td>選取包含此決定會考慮之優惠的優惠方案集合。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL遞補優惠]</td>
      <td>選取將向不符合此決定規則的客戶呈現的遞補優惠。
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
      <td role="rowheader">[！UICONTROL名稱]</td>
     <td>輸入或對應標籤的名稱。</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 集合] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
     <td>輸入或對映集合的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL篩選器型別]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL Elements]
      </td>
      <td>選取要包含在集合中的標籤。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 遞補優惠] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
     <td>輸入或對應遞補優惠的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL狀態]
      </td>
      <td> 選取遞補優惠的狀態。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL位置]
      </td>
      <td>輸入或對應遞補優惠的位置。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 個人化優惠] 欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
     <td>輸入或對應說明規則的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL狀態]</td>
      <td>選取決定的狀態。
      </td>
    </tr>
    <tr>
      <td role="rowheader">位置</td>
      <td>選取個人化優惠的位置。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL開始日期]</td>
      <td><p>輸入或對應個人化優惠方案的開始日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL結束日期]</td>
      <td><p>輸入或對應個人化優惠方案的結束日期。</p><p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL決定規則]</td>
      <td>選取要新增至此個人化優惠的決定規則。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL優先順序]</td>
      <td>選取此優惠方案的優先順序。 優先順序會影響此選件是否會出現，而非其他選件。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[！UICONTROL上限條件約束]</td>
      <td>輸入或對應此選件出現的次數。
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除中的單一記錄 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有關建立與的連線的指示 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與的連線 [!DNL Adobe Journey Optimizer]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL記錄型別]
      </td>
      <td>
        選取您要刪除的記錄型別
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL決定規則]</li>
        <li>[！UICONTROL決定]</li>
        <li>[！UICONTROL標籤]</li>
        <li>[！UICONTROL集合]</li>
        <li>[！UICONTROL遞補優惠]</li>
        <li>[！UICONTROL個人化優惠]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Placement]/[！UICONTROL Decision rule]/[！UICONTROL Decision]/[！UICONTROL Tag]/[！UICONTROL Collection]/[！UICONTROL遞補優惠]/[！UICONTROL個人化優惠]
      </td>
      <td>
        選取您要刪除的記錄。
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
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有關建立與的連線的指示 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與的連線 [!DNL Adobe Journey Optimizer]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入相對於 {baseURL} 開始使用<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
      <td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion會自動新增授權標題和x-api-key標題。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查詢字串]  </td>
      <td>
        <p>輸入請求查詢字串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入您希望模組在一個執行週期內傳回的結果數目上限。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除中的單一記錄 [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有關建立與的連線的指示 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與的連線 [!DNL Adobe Journey Optimizer]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL記錄型別]
      </td>
      <td>
        選取您要刪除的記錄型別
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL決定規則]</li>
        <li>[！UICONTROL決定]</li>
        <li>[！UICONTROL標籤]</li>
        <li>[！UICONTROL集合]</li>
        <li>[！UICONTROL遞補優惠]</li>
        <li>[！UICONTROL個人化優惠]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Placement]/[！UICONTROL Decision rule]/[！UICONTROL Decision]/[！UICONTROL Tag]/[！UICONTROL Collection]/[！UICONTROL遞補優惠]/[！UICONTROL個人化優惠]
      </td>
      <td>
        選取您要刪除的記錄。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL 更新記錄]

此動作模組會建立位置、決定、決定規則、標籤、個人化優惠、系列或遞補優惠。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有關建立與的連線的指示 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與的連線 [!DNL Adobe Journey Optimizer]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL記錄型別]
      </td>
      <td>
        選取您要更新的記錄型別
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL決定規則]</li>
        <li>[！UICONTROL決定]</li>
        <li>[！UICONTROL標籤]</li>
        <li>[！UICONTROL集合]</li>
        <li>[！UICONTROL遞補優惠]</li>
        <li>[！UICONTROL個人化優惠]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Placement]/[！UICONTROL Decision rule]/[！UICONTROL Decision]/[！UICONTROL Tag]/[！UICONTROL Collection]/[！UICONTROL遞補優惠]/[！UICONTROL個人化優惠]
      </td>
      <td>
        選取要更新的記錄。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [！UICONTROL欄位]
      </td>
      <td>針對您要更新的每個欄位：
      <ol>
      <li>按一下 <b>[！UICONTROL新增]</b>.</li>
      <li>選取您要新增、取代還是移除值。</li>
      <li>輸入要更新的欄位。</li>
      <li>輸入欄位的新值。</li>
      </td>
    </tr>

</tbody>
</table>


### 搜尋

#### [!UICONTROL 清單記錄]

此搜尋模組會列出所選型別的記錄，並根據您指定的條件傳回結果。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有關建立與的連線的指示 [!DNL Adobe Journey Optimizer]，請參閱 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與的連線 [!DNL Adobe Journey Optimizer]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL記錄型別]</p>
      </td>
      <td>
        <p>選取您要列出的記錄型別。</p>
        <ul>
        <li>[！UICONTROL位置]</li>
        <li>[！UICONTROL決定規則]</li>
        <li>[！UICONTROL決定]</li>
        <li>[！UICONTROL標籤]</li>
        <li>[！UICONTROL集合]</li>
        <li>[！UICONTROL遞補優惠]</li>
        <li>[！UICONTROL個人化優惠]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL查詢運運算元]</p>
      </td>
      <td>
        <p>選取要套用至查詢中引數的運運算元</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL欄位]</td>
      <td><p>如果要將搜尋限制在特定欄位，請輸入欄位。 針對您想要限制搜尋的每個欄位，按一下[！UICONTROL新增專案]並輸入欄位名稱。</p><p>路徑運算式採用點分隔路徑的形式，例如 <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Order by] </td>
      <td>輸入或對應您要排序結果的屬性。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL順序方向]</td>
   <td>選取您要依遞增或遞減方向排序結果。
    </td>
     </tr>
  </tbody>
</table>
