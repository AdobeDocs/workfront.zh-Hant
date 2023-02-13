---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: MIME模組
description: 您可以在Adobe Workfront Fusion中使用MIME類型。 多用途Internet郵件擴展(MIME)類型是標籤，允許軟體標識在Internet上共用的不同類型的資料。 Web伺服器和瀏覽器使用MIME類型來判斷應對檔案執行什麼操作。 例如，具有MIME類型的文本/html的檔案在瀏覽器中的處理方式與具有MIME類型的影像/jpeg的檔案不同。 MIME類型的功能與作業系統和硬體無關。
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# [!UICONTROL MIME] 模組

您可以在Adobe Workfront Fusion中使用MIME類型。 多用途Internet郵件擴展(MIME)類型是標籤，允許軟體標識在Internet上共用的不同類型的資料。 Web伺服器和瀏覽器使用MIME類型來判斷應對檔案執行什麼操作。 例如，MIME類型的檔案 `text/html` 在瀏覽器中的處理方式與MIME類型的檔案不同 `image/jpeg`. MIME類型的功能與作業系統和硬體無關。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL MIME] 模組及其欄位

### [!UICONTROL 取得MIME類型]

此變壓器模組會傳回與指定名稱、路徑或副檔名相關聯的MIME類型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案]</td> 
   <td> <p>輸入或映射要確定MIME類型的檔案。 </p> <p>您可以使用：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL檔案路徑]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL檔案名]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL副檔名]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 取得副檔名]

此變壓器模組會傳回指定MIME類型的原始副檔名。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME類型]</td> 
   <td> <p>輸入或映射要確定副檔名的MIME類型。 </p> </td> 
  </tr> 
 </tbody> 
</table>
