---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront聚變中的流量控制
description: 當您建立或編輯案例時，可以配置設定以控制資料流過該案例的方式。
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 1%

---

# Adobe Workfront聚變中的流量控制

當您建立或編輯案例時，可以配置設定以控制資料流過該案例的方式。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>   <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 中繼器

您可以使用 [!UICONTROL 中繼器] 模組，重複指定次數的任務。 A [!UICONTROL 中繼器] 模組生成一個又一個的套件。

例如，您可以使用 [!UICONTROL 中繼器] 模組，透過連接 **[!UICONTROL 電子郵件] >[!UICONTROL 給我發電子郵件]** 模組 [!UICONTROL 中繼器] 模組。

若要使用 [!UICONTROL 中繼器] 模組：

1. 按一下 [!UICONTROL 流量控制] 圖示 ![](assets/flow-control-icon.gif) 在畫面底部，按一下 **[!UICONTROL 中繼器]** 在顯示的功能表中。
1. 按一下 [!UICONTROL 中繼器] 組合，然後按一下 **[!UICONTROL 自動連接]** 框中。
1. 在 [!UICONTROL 流量控制] 框中，在 **[!UICONTROL 重複]** 框。

   在我們的電子郵件範例中，您會輸入5。

   ![](assets/repeater-2-350x207.png)

   項目的值會隨著 **[!UICONTROL 步驟]** 欄位，您可以透過選取 **[!UICONTROL 顯示高級設定]**. 此數字預設為1。

1. 按一下 **[!UICONTROL 確定]** 關閉 **[!UICONTROL 流量控制]** 框。

1. 按一下連線至的應用程式或服務模組 [!UICONTROL 中繼器] 模組。
1. 在顯示的方塊中，輸入您要重複的資訊。

   在我們的電子郵件範例中，您可在 [!UICONTROL 主旨] 框，然後映射 `i` 來自中繼器模組。

   ![](assets/repeater-3-350x207.png)

| 項目 | 說明 |
|---|---|
| [!UICONTROL 初始值] | 輸入或映射您要模組設定為的編號 `i` 在第一個小版本中。 預設值為1。 |
| [!UICONTROL 重覆] | 輸入或對應您要模組重複的次數。 此數字必須大於或等於0，且小於或等於10,000。 |
| [!UICONTROL 步驟] | 這是模組用來增加 `i`. 預設值為1。 |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>重複次數不由 `i`，因為寫程式會循環。 模組會重複 [!UICONTROL 重複] 欄位。 值 `i` 會隨著 [!DNL repeater] 模組，且可對應至稍後的模組。 上述範例將 `i` 進入Hello訊息，導致顯示「Hello 1」、「Hello 2」等訊息。

## [!UICONTROL 迭代器]

安 [!UICONTROL 迭代器] 是一種特殊類型的模組，可將陣列轉換為一系列捆綁包。 每個陣列項目都是 [!UICONTROL 迭代器] 模組輸出。 如需詳細資訊，請參閱 [[!UICONTROL 迭代器] 模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## 陣列聚合器

陣列聚合器是一種特殊類型的模組，它允許將多個捆綁組合合併為一個捆綁組合。 如需詳細資訊，請參閱 [[!UICONTROL 匯總器] 模組於Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL 路由器]

此 [!UICONTROL 路由器] 模組可讓您將流分支到多條路由，並以不同方式處理每條路由內的資料。 一次a [!UICONTROL 路由器] 模組接收一個包，它按照路由附加到的順序將它轉發到每個連接的路由 [!UICONTROL 路由器] 模組。 如需詳細資訊，請參閱 [路由器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
