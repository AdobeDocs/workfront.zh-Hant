---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: mime模組
description: 您可以在Adobe Workfront Fusion中使用MIME型別。 多用途網際網路郵件延伸模組(MIME)型別是標籤，可讓軟體識別網際網路上共用的不同資料型別。 Web伺服器和瀏覽器會使用MIME型別來決定應該對檔案執行的操作。 例如，具有MIME型別text/html的檔案在瀏覽器中的處理方式與MIME型別image/jpeg的檔案不同。 MIME型別獨立於作業系統和硬體。
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# [!UICONTROL MIME]模組

您可以在Adobe Workfront Fusion中使用MIME型別。 多用途網際網路郵件延伸模組(MIME)型別是標籤，可讓軟體識別網際網路上共用的不同資料型別。 Web伺服器和瀏覽器會使用MIME型別來決定應該對檔案執行的操作。 例如，MIME型別為`text/html`的檔案在瀏覽器中的處理方式與MIME型別為`image/jpeg`的檔案不同。 MIME型別獨立於作業系統和硬體。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## [!UICONTROL MIME]模組及其欄位

### [!UICONTROL 取得MIME型別]

此轉換器模組會傳回與指定名稱、路徑或副檔名相關聯的MIME型別。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案]</td> 
   <td> <p>輸入或對應您要決定其MIME型別的檔案。 </p> <p>您可以使用以下方式輸入檔案：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL檔案路徑]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[！UICONTROL檔案名稱]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>image.jpeg</p> </li> 
     <li><strong>[！UICONTROL副檔名]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 取得副檔名]

此轉換器模組會傳回指定MIME型別的原始副檔名。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL MIME型別]</td> 
   <td> <p>輸入或對應您要決定副檔名的MIME型別。 </p> </td> 
  </tr> 
 </tbody> 
</table>
