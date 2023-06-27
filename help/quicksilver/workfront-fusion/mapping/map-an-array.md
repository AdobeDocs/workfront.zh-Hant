---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 將陣列對應 [!DNL Adobe] Workfront Fusion
description: 您可以將陣列對應至Adobe Workfront Fusion中的模組欄位。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 將陣列對應 [!DNL Adobe Workfront Fusion]

陣列是一種特殊型別的專案，可包含下列專案：

* 一或多個文字值（簡單陣列）
* 相同型別（複雜陣列）的一或多個集合

>[!INFO]
>
>**範例：** 此 [!UICONTROL 觀看電子郵件] 模組會傳回每封電子郵件的附件陣列。 每個附件都代表一個集合，其中可能包含名稱、內容、大小等。

如需詳細資訊，請參閱 [中的專案資料型別 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## 對應陣列

1. 按一下位於目標欄位中的按鈕。

   >[!INFO]
   >
   >  **範例：** 對於上述範例，您可以按一下 [!UICONTROL 新增附件] 電子郵件按鈕。
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 在顯示的方塊中，輸入專案。

   面板可讓您以與其他任何型別的專案相同的方式對應欄位。 如果您不想分別填寫每個專案，但想將另一個陣列對應到目標欄位，請使用 [!UICONTROL 地圖] 按鈕。 在此情況下，請確定兩個陣列（來源陣列和目標陣列）具有相同的結構。

   您可以新增任意數量的專案至陣列。

您可以使用疊代器將陣列分割成個別的組合。 如需詳細資訊，請參閱 [[!UICONTROL 迭代器] 中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
