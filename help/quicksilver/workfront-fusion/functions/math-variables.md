---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 中的數學變數 [!DNL Adobe Workfront Fusion]
description: 下列數學變數可用於 [!DNL Adobe Workfront Fusion mapping] 面板。
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 3%

---

# 中的數學變數 [!DNL Adobe Workfront Fusion]

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

## pi

代表數學符號$\pi$。

## [!UICONTROL random]

傳回範圍中的浮點偽隨機數 [`0`，`1`] (包含 `0`，但不提供 `1`)。

使用以下公式來產生範圍中的整數偽隨機數 [`min`，`max`] （包含兩者） `min` 和 `max`)：

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
