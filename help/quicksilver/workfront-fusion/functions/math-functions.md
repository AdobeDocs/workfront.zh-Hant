---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的數學函式
description: Adobe Workfront Fusion對應面板中有以下數學函式。
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---

# 中的數學函式 [!DNL Adobe Workfront Fusion]

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 平均([值陣列])平均值(value1； [value2]， ...)]

傳回特定陣列中數值的平均值，或個別輸入數值的平均值。

## [!UICONTROL ceil （數字）]

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

## [!UICONTROL floor (number)]

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

## [!UICONTROL formatNumber (數字；decimalPOINTS； [小數分隔符號]； [千分位分隔符號])]

傳回請求格式的數字。 預設情況下，小數點為逗號(，)，千分位分隔符號為句點(.)。

>[!INFO]
>
>**範例:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>傳回123.456.789,000

## [!UICONTROL 最大值([值陣列])， max(value1；value2； ...)]

傳回指定陣列中的最大數字或個別輸入數字中的最大數字。

## [!UICONTROL 分鐘([值陣列])， min(value1； value2； ...)]

傳回指定陣列中的最小數字或個別輸入數字中的最小數字。

## [!UICONTROL parseNumber （數字；小數分隔符號）]

剖析包含數字的字串並傳回數字。 例如， parseNumber(1 756,456；，)

## [!UICONTROL round (number)]

將數值四捨五入至最接近的整數。

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

## [!UICONTROL sum ([值陣列])、sum(value1； value2； ...)]

傳回指定陣列中值的總和或個別輸入的數字的總和。
