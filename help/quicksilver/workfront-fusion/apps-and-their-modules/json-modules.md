---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON模組
description: Adobe Workfront Fusion JSON應用程式提供處理JSON格式資料的模組，讓Adobe Workfront Fusion可以進一步處理資料內容，或建立新的JSON內容。
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# [!UICONTROL JSON] 模組

此 [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] 應用程式會提供模組來處理JSON格式的資料，以便 [!DNL Adobe Workfront Fusion] 可進一步處理資料內容，或建立新的JSON內容。

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 若為工作自動化與整合]，[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
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

## 剖析JSON

* [資料結構](#data-structure)
* [集合與陣列](#collection-vs-array)

### 資料結構

資料結構說明JSON資料的組織方式，並可讓您將個別JSON專案對應至情境中的其他模組。 如果您未提供資料結構，可以手動執行模組並 [!DNL Workfront Fusion] 將會從提供的JSON建置結構：

1. 新增 [!UICONTROL 剖析JSON] 模組至案例。
1. 在 **[!UICONTROL JSON字串]** 欄位中，輸入您要建立資料結構的JSON。
1. 請勿將其他模組連線至 [!UICONTROL 剖析JSON] 模組尚未完成。 因為 [!DNL Workfront Fusion] 尚不瞭解JSON資料的結構，因此尚無法對映以下專案中的資料： [!UICONTROL 剖析JSON] 模組到場景中的其他模組。
1. 手動執行情境。 這允許 [!UICONTROL 剖析JSON] 模組，用於從您提供的JSON中識別JSON結構。
1. 您現在可以連線下列模組。 剖析JSON模組中的專案現在可用於對應。

如需詳細資訊，請參閱 [中的資料結構 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### 集合與陣列

如果JSON字串欄位包含集合 `{ ... }`，輸出是包含集合專案的單一組合。

>[!INFO]
>
>**範例:**
>
>```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

如果JSON字串欄位包含陣列 `[ ... ]`，則輸出為一系列組合。 每個組合都包含陣列的一個元素。

>[!INFO]
>
>**範例:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] 模組及其欄位

當您設定 [!DNL JSON] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除此之外，可能還會顯示其他JSON欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [彙總至JSON](#aggregate-to-json)
* [將JSON轉換為XML](#convert-json-to-xml)
* [剖析JSON](#parse-json)
* [建立JSON](#create-json)
* [轉換JSON](#transform-json)

### [!UICONTROL 彙總至JSON]

此彙總模組會將先前模組的輸出彙總至JSON。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL來源模組] </td> 
   <td> <p>選取輸出您要彙總至JSON之資料的模組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料結構]</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 資料結構會決定此模組中有哪些其他欄位可用。 如需詳細資訊，請參閱 <a href="#data-structure" class="MCXref xref">資料結構</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL縮排]</td> 
   <td> <p> 選取您要使用定位字元、兩個空格或四個空格縮排JSON。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Group by]</td> 
   <td>定義要將彙總輸出分組依據的運算式。 此運算式可包含一或多個對應專案。 然後使用此運算式的值將彙總的資料分隔成群組。 每個群組都會輸出為個別的組合，其中包含索引鍵（評估過的運算式）和值（彙總文字）。 您可以在後續模組中將該索引鍵當作篩選條件使用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL在空白彙總後停止處理]</td> 
   <td>啟用此選項可在沒有結果時停止情境。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 將JSON轉換為XML]

此動作模組會將JSON字串轉換為XML。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL JSON字串] </td> 
   <td> <p>輸入或對應您要轉換成XML的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 剖析JSON]

此動作模組會將JSON字串剖析為資料結構，好讓您存取JSON字串內的資料。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料結構]</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 如需詳細資訊，請參閱 <a href="#data-structure" class="MCXref xref">資料結構</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL JSON字串] </td> 
   <td> <p>輸入或對應您要剖析的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 建立JSON]

此動作模組會從資料結構建立JSON。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">資料結構</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 如需詳細資訊，請參閱 <a href="#data-structure" class="MCXref xref">資料結構</a> 本文章內容。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 轉換JSON]

此動作模組會將物件轉換為JSON字串。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL物件]</td> 
   <td> <p>輸入或對應您要轉換為JSON的物件。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 將資料記錄轉換為JSON

>[!INFO]
>
>**範例：** 下列範例說明如何轉換資料記錄 [!DNL Google Sheets] 轉換為JSON格式：
>
>1. 放置 [!DNL Google Sheets] > [!UICONTROL 選取列] 模組，用以擷取資料。 設定模組以從 [!DNL Google] 試算表。 設定&#x200B;**[!UICONTROL 傳回資料列的最大數量]** 數量較少，但因測試目的而大於一（例如，三個）。 執行 [!DNL Google Sheets] 以滑鼠右鍵按一下模組，然後選擇「**[!UICONTROL 僅執行此模組]**.」 驗證模組的輸出。
>
1. 連線 [!UICONTROL 陣列彙總] 之後的模組 [!DNL Google Sheets] 模組。 在模組的設定中，選擇 [!DNL Google Sheets] 中的模組 **[!UICONTROL 來源節點]** 欄位。 暫時保留其他欄位。
>
1. Connect [!UICONTROL JSON] > [!UICONTROL 建立JSON] 之後的模組 [!UICONTROL 陣列彙總] 模組。 模組的設定需要說明JSON格式的資料結構。 按一下 **[!UICONTROL 新增]** 以開啟「資料結構」設定。 建立此資料結構的最簡單方式，是自動從JSON範例產生此資料結構。 按一下 **[!UICONTROL 產生器]** 並將JSON範例貼到 **[!UICONTROL 範例資料]** 欄位：
>
**範例:**
>   
```
{

"books": [

{

"id": "ID",

"title": "Title",

"author": "Author"

}

]

}
```
>
1. 按一下&#x200B;**[!UICONTROL 儲存]**。此 [!UICONTROL 規格] 資料結構中的欄位現在包含產生的結構。
1. 將資料結構的名稱變更為更具體的名稱，然後按一下 **[!UICONTROL 儲存]**. 對應至根陣列屬性的欄位會顯示為JSON模組設定中的可對應欄位。
>
1. 按一下 **[!UICONTROL 地圖]** 欄位旁的按鈕，並對應 `Array[]` Array彙總器輸出中的專案。
>
1. 按一下 **[!UICONTROL 確定]** 以關閉 [!UICONTROL JSON] 模組的設定。
>
1. 開啟的設定 [!UICONTROL 陣列彙總] 模組。 變更 **[!UICONTROL 目標結構]** 從 [!UICONTROL 自訂] 至 [!UICONTROL JSON] 與根陣列屬性對應的模組欄位。 從以下位置對應專案： [!DNL Google Sheets] 模組至適當的欄位。
>
1. 按一下 **[!UICONTROL 確定]** 以關閉 [!UICONTROL 陣列彙總] 模組的設定。
>
1. 執行情境。
>
此 [!UICONTROL JSON] 模組輸出正確的JSON格式。
>
1. 開啟的設定 [!DNL Google Sheets] 模組並增加 [!UICONTROL 傳回資料列的最大數量] 數字大於試算表中的列數，以便處理所有資料。

## 疑難排解

### 無法從以下位置對應資料： [!UICONTROL 剖析JSON] 模組

請確定JSON內容已正確對應至 [!UICONTROL 剖析JSON] 模組，並確認資料結構已正確定義。 如需詳細資訊，請參閱 [將資料記錄轉換為JSON](#transforming-data-records-to-json) 本文章內容。

### 在JSON中使用條件陳述式時，模組失敗

使用條件陳述式時，例如 `if` 在JSON中，將引號放在條件陳述式之外。

>[!INFO]
>
**範例:**
>
![](assets/quotes-in-json-350x120.png)
