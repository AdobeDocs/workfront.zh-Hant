---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的陣列函式
description: 下列陣列函式可在Adobe Workfront Fusion對應面板中使用。
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 5860e75d0a6521abbe082668749f78058fe7a114
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Adobe Workfront Fusion中的陣列函式

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
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

## [!UICONTROL 新增（陣列；value1；value2； ...）]

將引數中指定的值加入陣列並傳回該陣列。

## [!UICONTROL 包含（陣列；值）]

驗證陣列是否包含值。

## [!UICONTROL 相異(陣列； [key])]

移除陣列內的重複專案。 使用&quot;[!UICONTROL key]用於存取複雜物件內部屬性的「 」引數。 若要存取巢狀屬性，請使用點標籤法。 陣列中的第一個專案是索引1。

>[!INFO]
>
>**範例：** `distinct(Contacts[];name)`
>
>透過比較「name」屬性來移除連絡人陣列內的重複專案

## [!UICONTROL 平面化（陣列）]

建立一個新陣列，將所有子陣列元素以遞回方式串連到其中，直到指定的深度。


## [!UICONTROL 聯結（陣列；分隔符號）]

在每個專案之間使用指定的分隔符號，將陣列中的所有專案串連到字串中。

## [!UICONTROL 索引鍵（物件）]

傳回給定物件或陣列屬性的陣列。

## [!UICONTROL 長度（陣列）]

傳回陣列中的專案數。

## [!UICONTROL 對應(複雜陣列；索引鍵；[篩選索引鍵]；[篩選的可能值])]

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

如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL 合併(array1； array2； ...)]

將一個或多個陣列合併到一個陣列中。

## [!UICONTROL 移除（陣列；值1；值2； ...）]

移除陣列引數中指定的值。 此函式僅對文字或數字的原始陣列有效。

## [!UICONTROL 反向（陣列）]

陣列中的第一個元素會成為最後一個元素，第二個元素會成為倒數第二個元素，依此類推。

## [!UICONTROL 磁碟片段(陣列；開始； [結束])]

傳回僅包含所選專案的新陣列。

## [!UICONTROL 排序(陣列； [訂購]； [key])]

排序陣列的值。 的有效值 `order` 引數為：

* `asc`

  （預設） — 遞增順序： 1、2、3、...代表型別「數字」。 A， B， C， a， b， c， ...適用於文字

* `desc`

  遞減順序： ...， 3， 2， 1代表型別Number。...， c， b， a， C， B， A代表文字。

* `asc ci`

  不區分大小寫的遞增順序：A、a、B、b、C、c...代表文字型別。

* `desc ci`

  不區分大小寫的遞減順序： ...， C， c， B， b， A，代表文字型別。

使用 `key` 引數以存取複雜物件內的屬性。

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

## [!UICONTROL arraydifference [陣列1，陣列2，模式]]

傳回兩個陣列之間的差異。

輸入下列其中一個值 `mode` 引數。

* `classic`：傳回包含所有元素的新陣列 `array1` 中不存在的 `array2`.

* `symmetric`：傳回兩個陣列不共用的元素陣列。

  換言之，此函式傳回的陣列包含了 `array1` 中不存在的 `array2`，以及的所有元素 `array2` 中不存在的 `array1`.

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
  >    傳回 `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    傳回 `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    傳回 `[1,2,6,7]`

## toArray

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
