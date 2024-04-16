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
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# 中的數學函式 [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

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
   <p>目前：否 [!DNL Workfront Fusion] 授權需求。</p> 
   <p>或</p> 
   <p>舊版：任何 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">產品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 計畫：您的組織必須購買 [!DNL Adobe Workfront Fusion].</li><li>[！UICONTROL Ultimate] [!DNL Workfront] 計畫： [!DNL Workfront Fusion] 已包括在內。</li></ul> 
   <p>或</p> 
   <p>目前：您的組織必須購買 [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 平均([值陣列])平均值(value1； [value2]， ...)]

傳回特定陣列中數值的平均值，或個別輸入之數值的平均值。

## [!UICONTROL ceil （數字）]

傳回大於或等於指定數字的最小整數。

>[!INFO]
>
>**範例：**
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
>**範例：**
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

## [!UICONTROL 最大([值陣列])， max(value1；value2； ...)]

傳回指定陣列中的最大數字或個別輸入數字中的最大數字。

## [!UICONTROL 分鐘([值陣列])， min(value1； value2； ...)]

傳回指定陣列中的最小數字，或個別輸入數字中的最小數字。

## [!UICONTROL round (number)]

將數值四捨五入至最接近的整數。

>[!INFO]
>
>**範例：**
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

## [!UICONTROL sum ([值陣列])， sum(value1； value2； ...)]

傳回指定陣列中值的總和，或個別輸入的數字總和。

## [!UICONTROL parseNumber （數字；小數分隔符號）]

剖析包含數字的字串並傳回數字。 例如， parseNumber(1 756,456；，)

## [!UICONTROL formatNumber (數字；decimalPOINTS； [decimalSeparator]； [千位分隔符號])]

傳回要求格式的數字。 依預設，小數點為逗號(，)，千分位分隔符號為句點(.)。

>[!INFO]
>
>**範例：**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>傳回123.456.789,000
