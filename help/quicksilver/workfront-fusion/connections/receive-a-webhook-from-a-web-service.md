---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 從Web服務接收Webhook
description: 如果Web服務目前未實作為中的應用程式 [!DNL Adobe Workfront Fusion]，但它支援傳送webhook，您可以使用自訂webhook模組作為即時觸發程式來將服務新增到情境中。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# 從Web服務接收Webhook

如果Web服務目前未實作為中的應用程式 [!DNL Adobe Workfront Fusion]，但它支援傳送webhook，您可以使用自訂webhook模組作為即時觸發程式來將服務新增到情境中。

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

## 接收webhook

1. 新增 **[!UICONTROL Webhook] >[!UICONTROL 自訂webhook]** 模組至您的情境。
1. 按一下 **[!UICONTROL 新增]**，輸入a **[!UICONTROL Webhook名稱]** 在顯示的方塊中，按一下 **[!UICONTROL 儲存]**.

1. 按一下 **[!UICONTROL 將地址複製到剪貼簿]**，然後按一下 **[!UICONTROL 確定]**.

1. 登入Web服務並在那裡執行下列動作：

   1. 在 [!UICONTROL 設定] Web服務的區域，建立webhook。
   1. 在步驟3中貼上您複製到剪貼簿的地址。
   1. 選取將觸發webhook的事件。

1. 在 [!DNL Workfront Fusion] 情境，指定您要觸發的事件 [!UICONTROL 自訂webhook] 模組。
1. 執行情境。

   當一或多個事件發生時， [!UICONTROL 自訂webhook] 模組觸發且案例執行。
