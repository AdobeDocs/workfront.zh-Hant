---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的陣列函式
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 1%

---

# Adobe Workfront Fusion中的陣列函式

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [陣列函式](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/array-functions.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td>  
   <td> <p>任何</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td>  
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td>  
   <td> 
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p> 
   <p>或</p> 
   <p>舊版：任何 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">產品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul> 
   <p>或</p> 
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 函數

* [加入](#join-array-separator)
* [length](#length-array)
* [金鑰](#keys-object)
* [切片](#slice-array-start-end)
* [合併](#merge-array1-array2)
* [包含](#contains-array-value)
* [移除](#remove-array-value1-value2)
* [新增](#add-array-value1-value2)
* [地圖](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [隨機播放]
* [sort](#sort-array-order-key)
* [反向](#reverse-array)
* [flatten](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arraydifference](#arraydifference-array1-array2-mode)
* [重複資料刪除]

### [!UICONTROL 聯結（陣列；分隔符號）]

在每個專案之間使用指定的分隔符號，將陣列中的所有專案串連到字串中。

### [!UICONTROL 長度（陣列）]

傳回陣列中的專案數。

### [!UICONTROL 鍵（物件）]

傳回給定物件或陣列屬性的陣列。

### [!UICONTROL 磁碟片段（陣列；開始；[結束]）]

傳回僅包含所選專案的新陣列。

### [!UICONTROL 合併(array1； array2； ...)]

將一個或多個陣列合併到一個陣列中。

### [!UICONTROL 包含（陣列；值）]

驗證陣列是否包含值。

### [!UICONTROL 移除（陣列；值1；值2； ...）]

移除陣列引數中指定的值。 此函式僅對文字或數字的原始陣列有效。

### [!UICONTROL 新增（陣列；值1；值2； ...）]

將引數中指定的值加入陣列並傳回該陣列。

### [!UICONTROL 對應（複雜陣列；機碼；[用於篩選的機碼]；[用於篩選的可能值]）]

傳回包含複雜陣列值的原始陣列。 此函式允許篩選值。 將原始變數名稱用於金鑰。

>[!INFO]
>
>**範例：**
>
>* `map(Emails[];email)`
>
>  傳回包含電子郵件的基本陣列
>
>* `map(Emails[];email;label;work;home)`
>
>  傳回原始陣列，其中包含標籤等於工作或住家位置的電子郵件

如需詳細資訊，請參閱[在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組

### 隨機播放

### [!UICONTROL 排序（陣列；[順序]；[索引鍵]）]

排序陣列的值。 `order`引數的有效值為：

* `asc`

  （預設） — 遞增順序： 1、2、3、...代表型別「數字」。 A， B， C， a， b， c， ...適用於文字

* `desc`

  遞減順序： ...， 3， 2， 1代表型別Number。...， c， b， a， C， B， A代表文字。

* `asc ci`

  不區分大小寫的遞增順序：A、a、B、b、C、c...代表文字型別。

* `desc ci`

  不區分大小寫的遞減順序： ...， C， c， B， b， A，代表文字型別。

使用`key`引數來存取複雜物件內的屬性。

將原始變數名稱用於金鑰。

若要存取巢狀屬性，請使用點標籤法。

陣列中的第一個專案是索引1。

>[!INFO]
>
>**範例：**
>
>* `sort(Contacts[];name)`
>
>    以預設遞增順序依「name」屬性來排列連絡人陣列
>
>* `sort(Contacts[];desc;name)`
>
>   依「name」屬性以遞減順序來排列連絡人陣列
>
>* `sort(Contacts[];asc ci;name)`
>
>    以不區分大小寫的遞增順序依「name」屬性來排列連絡人陣列
>
>* `sort(Emails[];sender.name)`
>
>    依「sender.name」屬性排序電子郵件陣列

### [!UICONTROL 反向（陣列）]

陣列中的第一個元素會成為最後一個元素，第二個元素會成為倒數第二個元素，依此類推。

### [!UICONTROL 平面化（陣列）]

建立一個新陣列，將所有子陣列元素以遞回方式串連到其中，直到指定的深度。

### [!UICONTROL distinct （陣列；[索引鍵]）]

移除陣列內的重複專案。 使用&quot;[!UICONTROL key]&quot;引數來存取複雜物件內的屬性。 若要存取巢狀屬性，請使用點標籤法。 陣列中的第一個專案是索引1。

>[!INFO]
>
>**範例：** `distinct(Contacts[];name)`
>
>透過比較「name」屬性來移除連絡人陣列內的重複專案

### toCollection

### toArray

此函式將集合轉換為機碼值組的陣列。

>[!INFO]
>
>**範例：**
>
>已提供集合
>
>`{ key1: "value1", key2: "value2:}`
>
>函式
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>傳回機碼值組的陣列
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1，array2，模式]]

傳回兩個陣列之間的差異。

為`mode`引數輸入下列其中一個值。

* `classic`：傳回新陣列，其中包含`array2`中不存在的`array1`的所有元素。

* `symmetric`：傳回兩個陣列不共用的元素陣列。

  換言之，此函式傳回的陣列包含`array2`中不存在的`array1`的所有元素，以及`array1`中不存在的`array2`的所有元素。

  >[!INFO]
  >
  >**範例：**
  >
  >假設使用下列陣列：
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    傳回`[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    傳回`[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    傳回`[1,2,6,7]`

### 去重複化

## 關鍵字

### emptyarray
