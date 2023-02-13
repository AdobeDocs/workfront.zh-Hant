---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront融合中的數學函式
description: 下列數學函式可在「Adobe Workfront融合」對應面板中使用。
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# 中的數學函式 [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL 平均值[值陣列])平均值(value1); [value2], ...)]

傳回特定陣列中數值的平均值，或個別輸入數值的平均值。

## [!UICONTROL ceil（數字）]

傳回大於或等於指定數字的最小整數。

>[!INFO]
>
>**範例:**
>
>* `ceil(` `1.2` `)`
   >
   >   傳回2
>
>* `ceil(` `4` `)`
   >
   >   傳回4


## [!UICONTROL 下限（數字）]

傳回小於或等於指定數字的最大整數。

>[!INFO]
>
>**範例:**
>
>* `floor(` `1.2` `)`
   >
   >   傳回1
>
>* `floor(` `1.9` `)`
   >
   >   傳回1
>
>* `floor(` `4` `)`
   >
   >   傳回4


## [!UICONTROL formatNumber(number;decimalPOINTS; [decimalSeparator]; [千分位分隔符號])]

以請求的格式返回數字。 預設情況下，小數點是逗號(,)，千分位分隔符號是句點(.)。

>[!INFO]
>
>**範例:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>返回123.456.789,000

## [!UICONTROL 最大值([值陣列]), max(value1;value2;...)]

返回指定陣列中的最大數字，或返回單獨輸入的數字中的最大數字。

## [!UICONTROL min([值陣列])、min(value1);value2;...)]

返回指定陣列中的最小數字，或返回在單獨輸入的數字中的最小數字。

## [!UICONTROL parseNumber(number;小數分隔符號]

使用數字剖析字串並傳回數字。 例如， parseNumber(1 756,456;,)

## [!UICONTROL 四捨五入（數字）]

將數值四捨五入為最接近的整數。

>[!INFO]
>
>**範例:**
>
>* `round(` `1.2` `)`
   >
   >   傳回1
>
>* `round(` `1.5` `)`
   >
   >   傳回2
>
>* `round(` `1.7` `)`
   >
   >   傳回2
> 
>* `round(` `2` `)`
   >
   >   傳回2


## [!UICONTROL 加總([值陣列])、sum(value1);value2;...)]

傳回指定陣列中值的總和，或個別輸入的數字總和。
