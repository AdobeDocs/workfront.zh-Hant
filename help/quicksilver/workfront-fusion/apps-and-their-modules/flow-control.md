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
source-wordcount: '637'
ht-degree: 1%

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
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 若為工作自動化與整合]，[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
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

## 中繼器

您可以使用 [!UICONTROL 中繼器] 重複指定次數之工作的模組。 A [!UICONTROL 中繼器] 模組逐一產生組合。

例如，您可以使用 [!UICONTROL 中繼器] 模組，透過連線 **[!UICONTROL 電子郵件] >[!UICONTROL 傳送電子郵件給我]** 模組至 [!UICONTROL 中繼器] 模組。

若要使用 [!UICONTROL 中繼器] 模組：

1. 按一下 [!UICONTROL 流量控制] 圖示 ![](assets/flow-control-icon.gif) 在畫面底部，然後按一下 **[!UICONTROL 中繼器]** 在顯示的功能表中。
1. 按一下 [!UICONTROL 中繼器] 組合，然後按一下 **[!UICONTROL 自動連線]** 在顯示的方塊中。
1. 在 [!UICONTROL 流量控制] 在出現的方塊中，輸入您想在 **[!UICONTROL 重複]** 方塊。

   在我們的電子郵件範例中，您會輸入5。

   ![](assets/repeater-2-350x207.png)

   專案的值會隨著每次重複而增加，增加值是在 **[!UICONTROL 步驟]** 欄位，您可以選取 **[!UICONTROL 顯示進階設定]**. 此數字預設為1。

1. 按一下 **[!UICONTROL 確定]** 以關閉 **[!UICONTROL 流量控制]** 方塊。

1. 按一下連線至的應用程式或服務模組 [!UICONTROL 中繼器] 模組。
1. 在出現的方塊中，鍵入要重複的資訊。

   在我們的電子郵件範例中，您會在 [!UICONTROL 主旨] 方塊，然後地圖 `i` 中繼器模組。

   ![](assets/repeater-3-350x207.png)

| 項目 | 說明 |
|---|---|
| [!UICONTROL 初始值] | 輸入或對應您希望模組設定的數字 `i` 在第一個反複專案內。 預設值為1。 |
| [!UICONTROL 重覆] | 輸入或對應您希望模組重複的次數。 此數字必須大於或等於0，且小於或等於10,000。 |
| [!UICONTROL 步驟] | 這是模組增加數值的數字 `i`. 預設值為1。 |

{style="table-layout:auto"}

>[!NOTE]
>
>重複次數並非由 `i`，因為它會在程式設計中處於回圈中。 模組將重複 [!UICONTROL 重複] 欄位。 值 `i` 隨著的每次反複專案變更 [!DNL repeater] 模組，並可對應至後續的模組。 上述範例對映下列專案的值： `i` 進入Hello訊息中，導致訊息顯示「Hello 1」、「Hello 2」等。

## [!UICONTROL 迭代器]

一個 [!UICONTROL 迭代器] 是一種特殊型別的模組，可將陣列轉換為一系列組合。 每個陣列專案都將是中的獨立套件 [!UICONTROL 迭代器] 模組輸出。 如需詳細資訊，請參閱 [[!UICONTROL 迭代器] 中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## 陣列彙總

陣列彙總器是一種特殊型別的模組，允許將多個套件組合合併為一個單一套件。 如需詳細資訊，請參閱 [[!UICONTROL 彙總] Adobe Workfront Fusion中的模組](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL 路由器]

此 [!UICONTROL 路由器] 模組可讓您將流量分支至數個路由，並以不同方式處理每個路由內的資料。 一次a [!UICONTROL 路由器] 模組會接收一個束，然後依照路由附加至的順序將其轉送到每個連線的路由。 [!UICONTROL 路由器] 模組。 如需詳細資訊，請參閱 [中的路由器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
