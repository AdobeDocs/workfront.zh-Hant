---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 從Web服務接收Webhook
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 從Web服務接收Webhook

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [為沒有聯結器的Web服務設定webhook](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

如果Web服務目前未在[!DNL Adobe Workfront Fusion]中實作為應用程式，但它支援傳送Webhook，則您可以使用自訂Webhook模組作為立即觸發程式，將服務新增至案例。

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

## 接收webhook

1. 將&#x200B;**[!UICONTROL Webhook] >[!UICONTROL 自訂webhook]**&#x200B;模組新增至您的情境。
1. 按一下「新增&#x200B;**[!UICONTROL 」]**，在顯示的方塊中輸入&#x200B;**[!UICONTROL Webhook名稱]**，然後按一下「儲存&#x200B;**[!UICONTROL 」]**。

1. 按一下&#x200B;**[!UICONTROL 將地址複製到剪貼簿]**，然後按一下&#x200B;**[!UICONTROL 確定]**。

1. 登入Web服務並在那裡執行下列動作：

   1. 在Web服務的[!UICONTROL 設定]區域中，建立webhook。
   1. 在步驟3貼上您複製到剪貼簿的地址。
   1. 選取將觸發webhook的事件。

1. 在[!DNL Workfront Fusion]案例中，指定您要觸發一或多個[!UICONTROL 自訂webhook]模組的事件。
1. 執行情境。

   當事件發生時，會觸發[!UICONTROL 自訂webhook]模組並且案例會執行。
