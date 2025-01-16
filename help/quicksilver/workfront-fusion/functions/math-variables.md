---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: ' [!DNL Adobe Workfront Fusion]中的數學變數'
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 2%

---

# [!DNL Adobe Workfront Fusion]中的數學變數

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [數學變數](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/math-variables.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

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

## pi

代表數學符號$\pi$。

## [!UICONTROL random]

傳回範圍[`0`，`1`]中的浮點偽隨機數（包含`0`，但不包含`1`）。

使用以下公式來產生範圍[`min`，`max`]中的整數偽隨機數（包含`min`和`max`）：

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
