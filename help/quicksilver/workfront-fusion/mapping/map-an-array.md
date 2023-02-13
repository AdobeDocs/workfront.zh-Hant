---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在中映射陣列 [!DNL Adobe] Workfront融合
description: 您可以將陣列對應至Adobe Workfront Fusion中的模組欄位。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 在中映射陣列 [!DNL Adobe Workfront Fusion]

陣列是可包含下列項目的特殊類型：

* 一個或多個文本值（簡單陣列）
* 同一類型的一個或多個集合（複雜陣列）

>[!INFO]
>
>**範例：** 此 [!UICONTROL 觀看電子郵件] 模組會針對每封電子郵件傳回一系列附件。 每個附件都代表一個集合，其中可能包含名稱、內容、大小等。

如需詳細資訊，請參閱 [中的項目資料類型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 映射陣列

1. 按一下目標欄位中的按鈕。

   >[!INFO]
   >
   >  **範例：** 在上述範例中，您可按一下 [!UICONTROL 新增附件] 按鈕。
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 在顯示的方塊中，輸入項目。

   面板可讓您以與任何其他類型的項目相同的方式對應欄位。 如果您不想個別填入每個項目，但想將另一個陣列對應至目標欄位，請使用 [!UICONTROL 地圖] 按鈕。 在此情況下，請確定兩個陣列（源陣列和目標陣列）具有相同的結構。

   您可以將任何數量的項目新增至陣列。

您可以使用迭代器將陣列分割為個別套件組合。 如需詳細資訊，請參閱 [[!UICONTROL 迭代器] 模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
