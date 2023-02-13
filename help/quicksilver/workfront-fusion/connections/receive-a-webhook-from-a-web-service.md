---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 從Web服務接收Webhook
description: 如果網站服務目前並未以 [!DNL Adobe Workfront Fusion]，但支援傳送webhook，您可以使用自訂webhook模組作為即時觸發，將服務新增至案例。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 從Web服務接收Webhook

如果網站服務目前並未以 [!DNL Adobe Workfront Fusion]，但支援傳送webhook，您可以使用自訂webhook模組作為即時觸發，將服務新增至案例。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 接收網頁鈎

1. 新增 **[!UICONTROL Webhook] >[!UICONTROL 自訂網頁連結]** 模組至您的案例。
1. 按一下 **[!UICONTROL 新增]**，鍵入 **[!UICONTROL Webhook名稱]** 在顯示的方塊中，然後按一下 **[!UICONTROL 儲存]**.

1. 按一下 **[!UICONTROL 將地址複製到剪貼簿]**，然後按一下 **[!UICONTROL 確定]**.

1. 登入網站服務，並在此處執行下列動作：

   1. 在 [!UICONTROL 設定] 區域，建立webhook。
   1. 在步驟3中，貼上您複製到剪貼簿的位址。
   1. 選取將觸發Webhook的事件。

1. 在 [!DNL Workfront Fusion] 案例，指定您要觸發的事件或事件 [!UICONTROL 自訂網頁連結] 模組。
1. 執行案例。

   當事件或事件發生時， [!UICONTROL 自訂網頁連結] 模組觸發，而情境執行。
