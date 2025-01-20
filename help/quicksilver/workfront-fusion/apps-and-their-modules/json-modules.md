---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON 模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1256'
ht-degree: 0%

---

# [!UICONTROL JSON]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [JSON模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/json-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

[!DNL Adobe Workfront Fusion] [!UICONTROL JSON]應用程式提供模組以處理JSON格式的資料，讓[!DNL Adobe Workfront Fusion]可以進一步處理資料內容，或建立新的JSON內容。

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 剖析JSON

* [資料結構](#data-structure)
* [集合與陣列](#collection-vs-array)

### 資料結構

資料結構說明JSON資料的整理方式，並可讓您將個別JSON專案對應至情境中的其他模組。 如果您未提供資料結構，您可以手動執行模組，而[!DNL Workfront Fusion]將會從提供的JSON建置結構：

1. 將[!UICONTROL 剖析JSON]模組新增至案例。
1. 在&#x200B;**[!UICONTROL JSON字串]**&#x200B;欄位中，輸入您要建置資料結構的JSON。
1. 請勿將其他模組連線到[!UICONTROL 剖析JSON]模組。 由於[!DNL Workfront Fusion]尚不瞭解JSON資料的結構，因此尚無法將[!UICONTROL 剖析JSON]模組的資料對應到情境中的其他模組。
1. 手動執行情境。 這可讓[!UICONTROL 剖析JSON]模組從您提供的JSON中識別JSON結構。
1. 您現在可以連線下列模組。 剖析JSON模組中的專案現在可用於對應。

如需詳細資訊，請參閱[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md)中的[資料結構。

### 集合與陣列

如果JSON字串欄位包含集合`{ ... }`，則輸出是包含集合專案的單一組合。

>[!INFO]
>
>**範例：**
>
>```
>{
>       "name" : "Peter",
>
>    
>   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

如果JSON字串欄位包含陣列`[ ... ]`，則輸出是一系列組合。 每個組合都包含陣列的一個元素。

>[!INFO]
>
>**範例：**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
> {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON]模組及其欄位

當您設定[!DNL JSON]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除此之外，可能會顯示其他JSON欄位，實際取決於您應用程式或服務中的存取層級等因素。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [將JSON轉換為XML](#convert-json-to-xml)
* [剖析JSON](#parse-json)
* [建立JSON](#create-json)
* [轉換JSON](#transform-json)

### 彙總

#### [!UICONTROL 彙總至JSON]

此彙總模組會將先前模組的輸出彙總至JSON。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組] </td> 
   <td> <p>選取輸出您要彙總至JSON之資料的模組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料結構]</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 資料結構會決定此模組中有哪些其他欄位可用。 如需詳細資訊，請參閱本文中的<a href="#data-structure" class="MCXref xref">資料結構</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL縮排]</td> 
   <td> <p> 選取您要使用定位字元、兩個空格或四個空格縮排JSON。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Group by]</td> 
   <td>定義要將彙總輸出分組依據的運算式。 此運算式可包含一或多個對應專案。 接著，會使用此運算式的值，將彙總資料分隔成群組。 每個群組會輸出一個單獨的組合，內含索引鍵（運算式）和值（彙總文字）。 您可以在後續模組中使用該索引鍵作為篩選條件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL在空白彙總後停止處理]</td> 
   <td>啟用此選項可在沒有結果時停止情境。</td> 
  </tr> 
 </tbody> 
</table>

### 轉換器

* [將JSON轉換為XML](#convert-json-to-xml)
* [建立JSON](#create-json)
* [剖析JSON](#parse-json)
* [轉換JSON](#transform-json)

#### [!UICONTROL 將JSON轉換為XML]

此動作模組會將JSON字串轉換為XML。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL JSON string] </td> 
   <td> <p>輸入或對應您要轉換成XML的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立JSON]

此動作模組會從資料結構建立JSON。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">資料結構</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 如需詳細資訊，請參閱本文中的<a href="#data-structure" class="MCXref xref">資料結構</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 剖析JSON]

此動作模組會將JSON字串剖析為資料結構，好讓您存取JSON字串內的資料。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料結構]</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 如需詳細資訊，請參閱本文中的<a href="#data-structure" class="MCXref xref">資料結構</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL JSON string] </td> 
   <td> <p>輸入或對應您要剖析的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 轉換JSON]

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
>**範例：**&#x200B;下列範例說明如何將資料記錄從[!DNL Google Sheets]轉換為JSON格式：
>
>1. 將[!DNL Google Sheets] > [!UICONTROL 選取情境中的列]模組以擷取資料。 設定模組以從[!DNL Google]試算表中擷取列。 將&#x200B;**[!UICONTROL 傳回資料列數目上限]**&#x200B;設定為小數，但大於一個以供測試之用（例如，三個）。 執行[!DNL Google Sheets]模組，方法為用滑鼠右鍵按一下該模組，然後選擇&#x200B;**[!UICONTROL 僅執行此模組]**。 驗證模組的輸出。
>
1. 在[!DNL Google Sheets]模組之後連線[!UICONTROL 陣列彙總]模組。 在模組的設定中，選擇&#x200B;**[!UICONTROL Source節點]**&#x200B;欄位中的[!DNL Google Sheets]模組。 讓其他欄位維持目前的狀態。
>
1. 在[!UICONTROL 陣列彙總]模組之後連線[!UICONTROL JSON] > [!UICONTROL 建立JSON]模組。 模組的設定需要說明JSON格式的資料結構。 按一下&#x200B;**[!UICONTROL 新增]**&#x200B;以開啟資料結構設定。 建立此資料結構的最簡單方法是，自動從JSON範例產生此資料結構。 按一下&#x200B;**[!UICONTROL 產生器]**&#x200B;並將您的JSON範例貼到&#x200B;**[!UICONTROL 範例資料]**&#x200B;欄位：
>
>     **範例：**
>
>     ```
>     {
>     
>     "books": [
>     
>     {
>     
>     "id": "ID",
>     
>     "title": "Title",
>     
>     "author": "Author"
>     
>     }
>     
>     ]
>     
>     }
>     
>     ```
>
1. 按一下「**[!UICONTROL 儲存]**」。資料結構中的[!UICONTROL 規格]欄位現在包含產生的結構。
1. 將您的資料結構名稱變更為更具體的名稱，然後按一下[儲存]。**** 對應至根陣列屬性的欄位會顯示為JSON模組設定中的可對應欄位。
>
1. 按一下欄位旁的&#x200B;**[!UICONTROL 對應]**&#x200B;按鈕，並將Array彙總器輸出中的`Array[]`專案對應至該欄位。
>
1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以關閉[!UICONTROL JSON]模組的設定。
>
1. 開啟[!UICONTROL 陣列彙總]模組的設定。 將&#x200B;**[!UICONTROL 目標結構]**&#x200B;從[!UICONTROL 自訂]變更為與根陣列屬性相對應的[!UICONTROL JSON]模組欄位。 將來自[!DNL Google Sheets]模組的專案對應到適當的欄位。
>
1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;關閉[!UICONTROL 陣列彙總]模組的設定。
>
1. 執行情境。
>
[!UICONTROL JSON]模組輸出正確的JSON格式。
>
1. 開啟[!DNL Google Sheets]模組的設定，並增加[!UICONTROL 傳回資料列數目上限]數字，使其大於試算表中的資料列數目，以處理所有資料。

## 疑難排解

### 無法對應來自[!UICONTROL 剖析JSON]模組的資料

請確定JSON內容已正確對應到[!UICONTROL 剖析JSON]模組，而且資料結構的定義正確。 如需詳細資訊，請參閱本文中的[將資料記錄轉換為JSON](#transforming-data-records-to-json)。

### 在JSON中使用條件陳述式時，模組失敗

在JSON中使用條件陳述式（例如`if`）時，請將引號放在條件陳述式之外。

>[!INFO]
>
**範例：**
>
![](assets/quotes-in-json-350x120.png)
