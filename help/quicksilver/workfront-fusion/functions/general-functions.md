---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的一般函式
description: Adobe Workfront Fusion對應面板中有以下一般函式。
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 5cd1cbd1976d5574668098be53daee780a9cc1fb
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的一般函式

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
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## [!UICONTROL get （物件或陣列；路徑）]

傳回物件或陣列的值路徑。 若要存取巢狀物件，請使用點標籤法。 陣列中的第一個專案是索引1。

>[!INFO]
>
>**範例：**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if （運算式；值1；值2）]

如果運算式評估為true，則傳回`value1`；否則會傳回`value2`。

若要建立if陳述式（只有在兩個或多個運算式被評估為true時才傳回值），請使用`and`關鍵字。

若要合併`if`陳述式，請使用`and`和`or`運運算元。

![和運運算元](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**範例：**
>
>* `if( 1 = 1 ; A ; B )`
>
>    傳回
>
>* `if( 1 = 2 ; A ; B )`
>
>   傳回B
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    傳回B
>   

## [!UICONTROL imfempty (value1； value2)]

如果此值不是空的，則傳回`value1`；否則會傳回`value2`。

>[!INFO]
>
>**範例：**
>
>* `ifempty(` `A` `;` `B`
>
>   傳回
>
>* `ifempty(` `unknown` `;` `B`
>
>   傳回B
>
>* `ifempty(` `""` `;` `B`
>
>   傳回B

## [!UICONTROL switch （運算式； value1； result1； [value2； result2； ...]； [else]）]

根據值清單評估一個值（稱為運算式）；傳回對應至第一個相符值的結果。 若要包含`else`值，請將其新增到最終運算式或值之後。

>[!INFO]
>
>**範例：**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   傳回2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   傳回3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>   傳回4
>   
>   在此函式中，4是在未套用運算式時傳回的值（`else`值）。

## [!UICONTROL 省略（物件；key1； [key2； ...]）]

省略物件的指定索引鍵並傳回其餘索引鍵。

>[!INFO]
>
>**範例：**
>
>`omit(`使用者`;`密碼`)`
>
>傳回使用者資訊（不包括密碼）的集合。

## [!UICONTROL pick（物件；key1； [key2； ...]）]

僅從物件中挑選指定的索引鍵。

>[!INFO]
>
>**範例：**
>
>`pick(`使用者`;`密碼`;`電子郵件`)`
>
>只傳回使用者密碼和電子郵件地址的集合。

## mergeCollections(collection1 ； collection2)

結合兩個集合的機碼值組以將其合併。 如果兩個集合包含相同的索引鍵，則第二個集合的值會覆寫第一個集合的值。

