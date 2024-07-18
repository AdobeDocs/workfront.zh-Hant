---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]中的資料結構'
description: 資料結構是一份檔案，詳細說明要傳輸至Adobe Workfront Fusion的資料格式。 根據此檔案，案例編輯器能夠確定哪個模組傳回或接收哪種資料。 資料結構檔案最常用於序列化/剖析資料格式，例如JSON、XML、CSV等。
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的資料結構

資料結構是一份檔案，詳細說明要傳輸至[!DNL Adobe Workfront Fusion]的資料格式。 根據此檔案，案例編輯器能夠確定哪個模組傳回或接收哪種資料。 資料結構檔案最常用於序列化/剖析資料格式，例如JSON、XML、CSV等。

您可以在[!UICONTROL 資料結構概觀]區段或需要資料結構規格的模組設定中按一下[!UICONTROL 建立新資料結構]按鈕，以建立資料結構。

支援的資料型別在[[!UICONTROL 模組的型別]](../../workfront-fusion/modules/module-types.md)文章中有說明。

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

## 資料結構產生器

資料結構並不一定都必須建立。 使用我們的內建產生器中的範本，可以更輕鬆進行。 藉由提供資料範例，產生器會自動根據您輸入的資料範例建立資料結構。 之後可以手動修改建立的資料結構。

![](assets/data-structure-generator-350x341.jpg)
