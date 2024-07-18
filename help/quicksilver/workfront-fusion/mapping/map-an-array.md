---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在 [!DNL Adobe] Workfront Fusion中對應陣列
description: 您可以將陣列對應至Adobe Workfront Fusion中的模組欄位。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中對應陣列

陣列是一種特殊型別的專案，可包含下列專案：

* 一或多個文字值（簡單陣列）
* 相同型別（複雜陣列）的一或多個集合

>[!INFO]
>
>**範例：** [!UICONTROL 觀看電子郵件]模組傳回每個電子郵件的附件陣列。 每個附件代表一個集合，其中可能包含名稱、內容、大小等。

如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)中的[專案資料型別。

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

## 對應陣列

1. 按一下位於目標欄位中的按鈕。

   >[!INFO]
   >
   >  **範例：**&#x200B;在上述範例中，您可以按一下電子郵件的[!UICONTROL 新增附件]按鈕。
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 在顯示的方塊中，輸入專案。

   面板可讓您以與其他任何型別專案相同的方式對應欄位。 如果您不想分別填入每個專案，但想將另一個陣列對應到目標欄位，請使用[!UICONTROL 對應]按鈕。 在此情況下，請確定兩個陣列（來源陣列和目標陣列）具有相同的結構。

   您可以新增任意數量的專案至陣列。

您可以使用疊代器將陣列分割成個別的組合。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[[!UICONTROL 迭代器]模組。
