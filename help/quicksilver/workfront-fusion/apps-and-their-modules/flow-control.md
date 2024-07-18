---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion中的流量控制
description: 當您建立或編輯案例時，可以設定設定來控制資料流經案例的方式。
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Adobe Workfront Fusion中的流量控制

當您建立或編輯案例時，可以設定設定來控制資料流經案例的方式。

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 中繼器

您可以使用[!UICONTROL 中繼器]模組來重複指定次數的工作。 [!UICONTROL 中繼器]模組會產生一個接一個的組合。

例如，您可以使用[!UICONTROL 中繼器]模組，傳送主題為「Hello 1」、「Hello 2」等的5封電子郵件，方法是將&#x200B;**[!UICONTROL 電子郵件] >[!UICONTROL 傳送電子郵件]**&#x200B;模組至[!UICONTROL 中繼器]模組。

若要使用[!UICONTROL 中繼器]模組：

1. 按一下畫面底部的[!UICONTROL 流量控制]圖示![](assets/flow-control-icon.gif)，然後在顯示的功能表中按一下&#x200B;**[!UICONTROL 中繼器]**。
1. 按一下[!UICONTROL 中繼器]組合，然後在顯示的方塊中按一下&#x200B;**[!UICONTROL 自動連線]**。
1. 在出現的[!UICONTROL 流量控制]方塊中，在&#x200B;**[!UICONTROL 重複]**&#x200B;方塊中輸入您想要的重複（輸出組合）數目。

   在我們的電子郵件範例中，您會輸入5。

   ![](assets/repeater-2-350x207.png)

   每次重複時，專案的值會以&#x200B;**[!UICONTROL 步驟]**&#x200B;欄位中指定的值增加，您可以選取&#x200B;**[!UICONTROL 顯示進階設定]**&#x200B;來檢視該欄位。 此數字預設為1。

1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以關閉&#x200B;**[!UICONTROL 流量控制]**&#x200B;方塊。

1. 按一下連線至[!UICONTROL 中繼器]模組的應用程式或服務模組。
1. 在出現的方塊中，鍵入要重複的資訊。

   在我們的電子郵件範例中，您會在[!UICONTROL 主旨]方塊中輸入Hello，然後從中繼器模組對應`i`。

   ![](assets/repeater-3-350x207.png)

| 項目 | 說明 |
|---|---|
| [!UICONTROL 初始值] | 輸入或對映您要在第一個反複專案中設定為`i`的模組。 預設值為1。 |
| [!UICONTROL 重複] | 輸入或對應您希望模組重複的次數。 此數字必須大於或等於0，且小於或等於10,000。 |
| [!UICONTROL 步驟] | 這是模組增加`i`值的數目。 預設值為1。 |

{style="table-layout:auto"}

>[!NOTE]
>
>重複次數不是由`i`的值決定，因為它在程式設計中會處於回圈中。 模組將重複[!UICONTROL 重複]欄位中指定的次數。 值`i`會隨著[!DNL repeater]模組的每個反複專案而變更，並可對應至之後的模組。 上述範例將`i`的值對應到Hello訊息中，導致訊息顯示「Hello 1」、「Hello 2」等。

## [!UICONTROL 迭代器]

[!UICONTROL 疊代器]是一種特殊的模組，可將陣列轉換為一系列組合。 在[!UICONTROL 疊代器]模組輸出中，每個陣列專案都是個別的組合。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[[!UICONTROL 迭代器]模組。

## 陣列彙總

陣列彙總器是一種特殊型別的模組，可將數個套件合併為單一套件。 如需詳細資訊，請參閱Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md)中的[[!UICONTROL 彙總]模組。

## [!UICONTROL 路由器]

[!UICONTROL 路由器]模組可讓您將流量分支為數個路由，並以不同方式處理每個路由中的資料。 一旦[!UICONTROL 路由器]模組收到套件組合，它會依照路由附加至[!UICONTROL 路由器]模組的順序將其轉送至每個連線的路由。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md)中的[路由器模組。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
