---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON模組
description: Adobe Workfront Fusion JSON應用程式提供模組，可處理JSON格式的資料，讓Adobe Workfront Fusion可進一步處理資料內容，或建立新的JSON內容。
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# [!UICONTROL JSON] 模組

此 [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] 應用程式提供模組，可以處理JSON格式的資料， [!DNL Adobe Workfront Fusion] 可進一步使用資料內容，或建立新的JSON內容。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 剖析JSON

* [資料結構](#data-structure)
* [集合與陣列](#collection-vs-array)

### 資料結構

資料結構說明JSON資料的組織方式，並啟用將個別JSON項目對應至您案例中的其他模組。 如果您未提供資料結構，則可手動執行模組和 [!DNL Workfront Fusion] 將從提供的JSON建置結構：

1. 新增 [!UICONTROL 剖析JSON] 模組至案例。
1. 在 **[!UICONTROL JSON字串]** 欄位中，輸入要從中建立資料結構的JSON。
1. 不將其他模組連接到 [!UICONTROL 剖析JSON] 模組尚未完成。 因為 [!DNL Workfront Fusion] 尚不知道JSON資料的結構，因此無法從 [!UICONTROL 剖析JSON] 模組轉換至您案例中的其他模組。
1. 手動執行案例。 這可讓 [!UICONTROL 剖析JSON] 模組，從您提供的JSON識別JSON結構。
1. 您現在可以連接下列模組。 剖析JSON模組中的項目現在可用於對應。

如需詳細資訊，請參閱 [中的資料結構 [!UICONTROL Adobe Workfront融合]](../../workfront-fusion/modules/data-structures.md).

### 集合與陣列

如果JSON字串欄位包含集合 `{ ... }`，輸出是包含集合項目的單一套件組合。

>[!INFO]
>
>**範例:**
>
>
```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

如果JSON字串欄位包含陣列 `[ ... ]`，則輸出是一系列套件組合。 每個套件都包含一個陣列元素。

>[!INFO]
>
>**範例:**
>
>
```
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

設定時 [!DNL JSON] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些欄位，還可能會顯示其他JSON欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [匯總至JSON](#aggregate-to-json)
* [將JSON轉換為XML](#convert-json-to-xml)
* [剖析JSON](#parse-json)
* [建立JSON](#create-json)
* [轉換JSON](#transform-json)

### [!UICONTROL 匯總至JSON]

此匯總模組會將上一個模組的輸出匯總至JSON。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組] </td> 
   <td> <p>選取要輸出匯總至JSON之資料的模組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料結構]</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 資料結構決定了此模組中可用的其他欄位。 如需詳細資訊，請參閱 <a href="#data-structure" class="MCXref xref">資料結構</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL縮進]</td> 
   <td> <p> 選擇要使用制表符、兩個空格或四個空格縮進JSON。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL組依據]</td> 
   <td>定義要將匯總輸出分組的表達式。 此運算式可包含一或多個已對應項目。 然後，使用此運算式的值將匯總的資料分成群組。 每個群組會以獨立套件的形式輸出，其中包含鍵值（評估的運算式）和值（匯總文字）。 您可以在後續模組中將索引鍵當作篩選器。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL在空聚合後停止處理]</td> 
   <td>啟用此選項可在沒有結果時停止方案。</td> 
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
   <td role="rowheader">[!UICONTROL JSON字串] </td> 
   <td> <p>輸入或對應您要轉換為XML的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 剖析JSON]

此動作模組會將JSON字串剖析為資料結構，以便您存取JSON字串內的資料。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料結構]</td> 
   <td> <p>選取您要用來建立JSON的資料結構。 如需詳細資訊，請參閱 <a href="#data-structure" class="MCXref xref">資料結構</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON字串] </td> 
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
   <td> <p>選取您要用來建立JSON的資料結構。 如需詳細資訊，請參閱 <a href="#data-structure" class="MCXref xref">資料結構</a> 這篇文章。</p> </td> 
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
   <td role="rowheader">[!UICONTROL對象]</td> 
   <td> <p>輸入或對應您要轉換為JSON的物件。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 將資料記錄轉換為JSON

>[!INFO]
>
>**範例：** 以下範例說明如何從 [!DNL Google Sheets] 轉換為JSON格式：
>
>1. 放置 [!DNL Google Sheets] > [!UICONTROL 選取列] 模組來擷取資料。 設定模組以從 [!DNL Google] 試算表。 設&#x200B;定&#x200B;**[!UICONTROL 返回行數上限]** 小數字，但大於1以用於測試（例如，3）。 執行 [!DNL Google Sheets] 模組，請按一下滑鼠右鍵並選取「**[!UICONTROL 僅運行此模組]**.&quot; 驗證模組的輸出。
1. 連接 [!UICONTROL 陣列聚合器] 模組之後 [!DNL Google Sheets] 模組。 在模組的設定中，選取 [!DNL Google Sheets] 模組 **[!UICONTROL 源節點]** 欄位。 暫時保留其他欄位。
1. Connect [!UICONTROL JSON] > [!UICONTROL 建立JSON] 模組之後 [!UICONTROL 陣列聚合器] 模組。 模組的設定需要說明JSON格式的資料結構。 按一下 **[!UICONTROL 新增]** 開啟「資料結構」設定。 要建立此資料結構，最簡單的方式是從JSON範例自動產生。 按一下 **[!UICONTROL 產生器]** 並將您的JSON範例貼到 **[!UICONTROL 範例資料]** 欄位：

   **範例:**
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
1. 按一下&#x200B;**[!UICONTROL 儲存]**。此 [!UICONTROL 規格] 資料結構中的欄位現在包含產生的結構。
1. 將資料結構的名稱變更為更具體的名稱，然後按一下 **[!UICONTROL 儲存]**. 與根陣列屬性對應的欄位會在JSON模組的設定中顯示為可對應欄位。
1. 按一下 **[!UICONTROL 地圖]** 按鈕，並對應 `Array[]` 從陣列聚合器輸出到它的項目。
1. 按一下 **[!UICONTROL 確定]** 關閉 [!UICONTROL JSON] 模組設定。
1. 開啟 [!UICONTROL 陣列聚合器] 模組。 變更 **[!UICONTROL 目標結構]** 從 [!UICONTROL 自訂] 到 [!UICONTROL JSON] 模組的欄位，對應於根陣列屬性。 對應來自 [!DNL Google Sheets] 模組至適當欄位。
1. 按一下 **[!UICONTROL 確定]** 關閉 [!UICONTROL 陣列聚合器] 模組設定。
1. 執行案例。
   此 [!UICONTROL JSON] 模組會輸出正確的JSON格式。
1. 開啟 [!DNL Google Sheets] 模組和增加 [!UICONTROL 返回行數上限] 大於試算表中處理所有資料的列數。


## 疑難排解

### 無法映射來自 [!UICONTROL 剖析JSON] 模組

請確定JSON內容已正確對應至 [!UICONTROL 剖析JSON] 模組和資料結構已正確定義。 如需詳細資訊，請參閱 [將資料記錄轉換為JSON](#transforming-data-records-to-json) 這篇文章。

### 在JSON中使用條件陳述式時模組失敗

使用條件陳述式時，例如 `if` 在JSON中，將引號放在條件陳述式之外。

>[!INFO]
**範例:**
![](assets/quotes-in-json-350x120.png)
