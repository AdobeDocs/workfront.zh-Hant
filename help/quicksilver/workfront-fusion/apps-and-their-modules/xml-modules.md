---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: XML應用程式可讓您透過XML &gt；剖析XML模組來剖析XML格式文字，並將其轉換成組合，讓其他模組可以使用資料。 您也可以透過XML &gt；建立XML模組將組合轉換為XML格式文字
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 2%

---

# XML

此 [!UICONTROL XML] 應用程式可讓您透過 [!UICONTROL XML] > [!UICONTROL 剖析XML] 模組，並將其轉換為套件組合，使資料可供其他模組使用。 您也可以透過以下方式將組合轉換為XML格式文字： [!UICONTROL XML] > [!UICONTROL 建立XML] 模組

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

## [!UICONTROL 剖析XML]

此 [!UICONTROL XML] > [!UICONTROL 剖析XML] 模組會剖析XML格式文字，並輸出包含從XML擷取之所有資訊的單一組合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL資料結構]</p> </td> 
   <td> <p>資料結構說明XML的結構，以使模組輸出可在對應面板中用於下列模組。</p> <p>如果您有想要剖析的XML範例，可以使用它來產生資料結構：</p> 
    <ol> 
     <li value="1">按一下 <strong>[！UICONTROL新增]</strong> 按鈕。</li> 
     <li value="2">按一下 <strong>[！UICONTROL Generator]</strong> 按鈕。</li> 
     <li value="3">將XML範例複製並貼到 <strong>[！UICONTROL範例資料]</strong> 欄位。</li> 
     <li value="4">按一下 <strong>[！UICONTROL儲存]</strong>.</li> 
     <li value="5">確認已成功產生資料結構。</li> 
     <li value="6"> <p>按一下 <strong>[！UICONTROL儲存]</strong> 按鈕以儲存資料結構。</p> <p>您可以略過步驟2至5，提供空白的資料結構。 如果資料結構是空的，至少執行一次模組後，才能在對應面板中取得模組的輸出。</p> </li> 
    </ol> <p>如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">中的資料結構 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL保留數字為文字]</td> 
   <td>啟用此選項以確保數字保持為文字（字串）值。 否則，數字會轉換為數字值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL XML]</p> </td> 
   <td> <p>輸入或對應您要剖析的XML格式文字。</p> <p>如果您使用公式，請確定其結果值型別是（或可自動強製為）[！UICONTROL Text]資料型別。 </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>如果結果值型別為[！UICONTROL Buffer] （二進位資料），則使用 <code>toString()</code> 函式以將其轉換為Text資料型別。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a> 和 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">[！UICONTROL Adobe Workfront Fusion]中的專案資料型別</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 若要從URL下載XML檔案並剖析其內容：
>
>1. 建立新情境。
>1. 插入 [!UICONTROL HTTP] > [!UICONTROL 取得檔案] 模組
>1. 開啟模組的設定，並依照以下方式設定：
>
>   **URL**： XML檔案的URL (例如 `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. 按一下 **[!UICONTROL 確定]**&#x200B;以&#x200B;儲存並關閉模組的設定。
1. 新增 [!UICONTROL XML] > [!UICONTROL 剖析XML] 模組，將其連線在 [!UICONTROL HTTP] > [!UICONTROL 取得檔案] 模組，並依照以下方式設定：
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[！UICONTROL資料結構]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">按一下 <strong>[！UICONTROL新增]</strong> 按鈕。</li> 
&gt;        <li value="2">按一下 <strong>[！UICONTROL Generator]</strong> 按鈕。</li> 
&gt;        <li value="3">在網頁瀏覽器中，開啟新的標籤或視窗。</li> 
&gt;        <li value="4">將您第三個步驟中使用的URL放在位址列中，並擷取XML檔案。</li> 
&gt;        <li value="5">選取所有XML文字，並將其複製到剪貼簿中。</li> 
&gt;        <li value="6">關閉標籤或視窗，並返回您的案例。</li> 
&gt;        <li value="7">將複製的XML文字貼到「範例資料」欄位中。</li> 
&gt;        <li value="8">按一下 <strong>[！UICONTROL儲存]</strong>.</li> 
&gt;        <li value="9">確認已成功產生資料結構。</li> 
&gt;        <li value="10">按一下 <strong>[！UICONTROL儲存]</strong> 以儲存資料結構。</li> 
&gt;       </ol> <p>您可以略過步驟2到9，以提供空白的資料結構。 如果資料結構是空的，至少執行一次模組後，才能在對應面板中取得模組的輸出。</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[！UICONTROL XML]</td> 
&gt;      <td> <p>對應 <code>Data </code>[！UICONTROL HTTP] &gt; [！UICONTROL取得檔案]模組的輸出中的專案放入欄位中。 使用 <code>toString()</code> 函式來將其值從[！UICONTROL Buffer] （二進位資料）型別轉換為[！UICONTROL Text]資料型別。</p> <p>您可以將公式的程式碼複製並貼到欄位中： <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>如需有關「緩衝區」和「文字」資料型別的詳細資訊，請參閱 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion中的專案資料型別</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL 剖析XML屬性]

根據預設， [!UICONTROL XML] > [!UICONTROL 剖析XML] 模組將屬性放入特殊集合中 `_attributes` 作為具有這些屬性的節點的子系。 如果節點是文位元組點且有屬性，則會新增兩個特殊屬性： `_attributes` 屬性和 `_value` 用於節點的文字內容。

>[!INFO]
>
**範例：** 此XML：

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

會轉換為此套件組合：

![](assets/xml-converted-to-bundle.png)

## 建立XML

此 [!UICONTROL XML] > [!UICONTROL 建立XML] 模組會將組合轉換為XML格式的文字。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL資料結構]</p> </td> 
   <td> <p>資料結構描述產生的XML的結構。 如果您有想要建立的XML範例，可以使用它來產生資料結構：</p> 
    <ol> 
     <li value="1">按一下 <strong>[！UICONTROL新增]</strong> 按鈕。</li> 
     <li value="2">按一下 <strong>[！UICONTROL Generator]</strong> 按鈕。</li> 
     <li value="3">將XML範例複製並貼到「範例資料」欄位中。</li> 
     <li value="4">按一下 <strong>[！UICONTROL儲存]</strong> 按鈕。</li> 
     <li value="5">確認已成功產生資料結構。</li> 
     <li value="6">按一下 <strong>[！UICONTROL儲存]</strong> 以儲存資料結構。</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL根元素名稱]</td> 
   <td>輸入XML根元素的名稱。 預設值為 <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Doctype系統ID]</td> 
   <td>輸入檔案名稱，以用於<code> !DOCTYPE SYSTEM</code> 宣告</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Doctype公共ID]</td> 
   <td>輸入檔案名稱，以用於<code> !DOCTYPE PUBLIC</code> 宣告</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL長條Xml宣告]</td> 
   <td>啟用此選項以移除XML宣告 <code>&lt;?xml ... ?&gt;</code> 和 <code>&lt;!DOCTYPE ... &gt;</code>和僅保留XML根元素及其內容。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**範例:**
>
典型的使用案例是將資料從 [!DNL Google] >試算表轉換為XML。
>
1. 放置 [!DNL Google Sheets] > [!UICONTROL 選取列] 模組，用以擷取資料。 設定模組以從 [!DNL Google] 試算表。 設定&#x200B;**[!UICONTROL 傳回資料列的最大數量]** 數量較少，但因測試目的而大於一（例如，三個）。 執行 [!DNL Google Sheets] 以滑鼠右鍵按一下模組，然後選擇「**[!UICONTROL 僅執行此模組]**.」 驗證模組的輸出。
1. 連線 [!UICONTROL 陣列彙總] 之後的模組 [!DNL Google Sheets] 模組。 在模組的設定中，選擇 [!DNL Google Sheets] 中的模組 **[!UICONTROL 來源節點]** 欄位。 暫時保留其他欄位。
1. 連線 [!UICONTROL XML] > [!UICONTROL 建立XML] 之後的模組 [!UICONTROL 陣列彙總] 模組。
>
模組的設定需要說明XML輸出結構的資料結構。 按一下 **[!UICONTROL 新增]** 按鈕以開啟資料結構設定。 建立此資料結構的最簡單方法是從XML範例自動產生它。
>
1. 按一下 **[!UICONTROL 產生器]** 按鈕並將XML範例貼到 [!UICONTROL 範例資料] 欄位：
>
![](assets/sample-data-field-350x146.png)
>
1. 按一下&#x200B;**[!UICONTROL 儲存]**。「資料結構」中的「規格」欄位現在包含產生的結構。
1. 將資料結構的名稱變更為更具體的名稱，然後按一下 **[!UICONTROL 儲存]**. 對應至根陣列屬性的欄位會顯示為JSON模組設定中的可對應欄位。
1. 按一下 **[!UICONTROL 地圖]** 欄位旁的按鈕，並對應 `Array[]` 專案來自 [!UICONTROL 陣列彙總] 輸出至其中：
1. 按一下 **[!UICONTROL 確定]** 關閉XML模組的設定。
1. 開啟的設定 [!UICONTROL 陣列彙總] 模組。 變更 **[!UICONTROL 目標結構]** 從自訂對應至與上層XML元素相對應的XML模組欄位。從對應專案 [!DNL Google Sheets] 模組至適當的欄位。
1. 按一下 **[!UICONTROL 確定]** 以關閉Array Aggregator模組的設定。
1. 執行情境。
>
XML模組會輸出正確的XML檔案。
>
1. 開啟的設定 [!DNL Google Sheets] 模組並增加 [!UICONTROL 傳回資料列的最大數量] 數字大於試算表中的列數，以便處理所有資料。
>
產生的XML可以儲存到 [!DNL Dropbox]，透過電子郵件以附件形式傳送、透過FTP上傳至伺服器，等等。

## 新增XML屬性

如果您想要將屬性新增至複雜節點（包含其他節點的節點），則必須以名稱新增集合 `_attributes` 適用於自訂資料結構中的複雜附註。 此集合將會對應至節點屬性。 如果您想要將屬性新增至文位元組點(例如： `<node attr="1">abc</node>`)，您必須新增集合 `_attributes` 屬性和text屬性 `_value` （自訂資料結構中此節點的節點值）。

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## 疑難排解：無法從以下位置對應資料： [!UICONTROL 剖析XML] 模組

請確定資料結構的定義正確。 或者，您可以使用空的資料結構並至少執行一次模組以處理XML輸入。
