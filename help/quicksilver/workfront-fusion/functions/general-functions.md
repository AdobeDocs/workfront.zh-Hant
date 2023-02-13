---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion的一般功能
description: Adobe Workfront Fusion對應面板提供下列一般功能。
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

---

# 中的一般函式 [!DNL Adobe Workfront Fusion]

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL get（物件或陣列）路徑)]

返回對象或陣列的值路徑。 若要存取巢狀物件，請使用點記號。 陣列中的第一個項是索引1。

>[!INFO]
>
>**範例:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if（表達式）;value1;value2)]

傳回 `value1` 如果運算式被評估為true;否則會傳回 `value2`.

>[!INFO]
>
>**範例:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    傳回A
>
>* `if( = 2 ; A ; B )`
   >
   >   傳回B


## [!UICONTROL ifempty(value1);value2)]

傳回 `value1` 如果此值不為空；否則會傳回 `value2`.

>[!INFO]
>
>**範例:**
>
>* `ifempty(` `A` `;` `B` )
   >
   >   傳回A
>
>* `ifempty(` `unknown` `;` `B` )
   >
   >   傳回B
>
>* `ifempty(` `""` `;` `B` )
   >
   >   傳回B


## [!UICONTROL 開關（表達式）value1;結果1; [value2;結果2;...]; [else])]

根據值清單評估一個值（稱為運算式）;返回與第一個匹配值對應的結果。

>[!INFO]
>
>**範例:**
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
>  傳回4

## [!UICONTROL 忽略(object)key1; [key2;...])]

省略物件的指定金鑰，並傳回其餘金鑰。

>[!INFO]
>
>**範例:**
>
>`omit(` 使用者 `;` 密碼 `)`
>
>傳回使用者資訊的集合，排除密碼。

## [!UICONTROL pick(object);key1; [key2;...])]

僅從物件中挑選指定的金鑰。

>[!INFO]
>
>**範例:**
>
>`pick(` 使用者 `;` 密碼 `;` 電子郵件 `)`
>
>僅傳回使用者密碼和電子郵件地址的集合。
