---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: ' [!DNL Adobe Workfront Fusion]中的即時觸發程式(webhook)'
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的即時觸發器(webhook)

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [即時觸發程式(webhook)](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/webhooks-reference.html)
>* [檢視webhook的佇列](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-webhook-queue.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

許多服務都會提供Webhook，以便在服務發生特定變更時傳送即時通知。 若要處理這些通知，建議您使用立即觸發程式。 您可以在[!DNL Adobe Workfront Fusion]中輕鬆辨識這些專案，因為其標籤：

![](assets/instant-350x256.png)

如果服務不提供Webhook，您需要使用輪詢觸發程式來定期輪詢服務。

如需Workfront Fusion中Webhook的影片簡介，請參閱：

* [Webhook簡介](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [中繼Webhook](https://video.tv.adobe.com/v/3427030/){target=_blank}

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

## 檢視webhook的佇列

所有來自傳入webhook的訊息都會儲存在webhook的佇列中。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Webhooks]**。
1. 尋找您要檢視其佇列的Webhook。
1. 按一下帶有卡車圖示和已接收Webhook數量的按鈕。

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >無論您如何設定選項[!UICONTROL 資料]是機密的（在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)的[案例設定面板中說明），傳入的webhook資料一律會儲存在佇列中。 在案例中處理資料後，資料就會從系統中永久刪除。

## 排程即時觸發程式

如果您的案例包含立即觸發器，您可以排程案例立即執行：

![](assets/schedule-setting-350x185.png)

在此情況下，當[!DNL Workfront Fusion]從服務收到新資料時，您的情境會立即執行。 執行案例後，系統會計算佇列中等待的擱置Webhook總數，而案例執行的週期與擱置Webhook相同，每個週期處理一個Webhook。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的[案例執行、週期和階段。

>[!NOTE]
>
>* 週期與案例執行不同。 1個案例執行中可以有多個週期。
>* 當您使用排定為立即的立即觸發程式執行案例時，將會套用下列例外：
>
>     * 根據定價計畫，兩個執行之間的間隔不受最小間隔的限制。
>
>       例如，一旦案例完成執行，就會再次檢查webhook的佇列。 如果有任何擱置中的Webhook，情境會立即再次執行，並再次處理所有擱置中的Webhook。
>   
>     * 「最大週期數」情境設定會忽略並設為100，這表示在單一情境執行期間不會處理超過100個擱置中的Webhook （每個週期為1個事件）。
>


如果您使用[!UICONTROL 立即]以外的任何其他排程設定，情境會依您指定的間隔執行。 由於間隔期間可在佇列中收集數個webhook，因此建議將[[!UICONTROL 最大週期數]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum)設定為比預設1更高的值，以便在一次案例執行中處理更多webhook：

1. 按一下案例底部的[!UICONTROL 案例設定]圖示![](assets/gear-icon-settings.png)。
1. 在出現的&#x200B;**[!UICONTROL 情境設定]**&#x200B;方塊中，在&#x200B;**[!UICONTROL 最大循環數]**&#x200B;方塊中輸入數字，以表示每次執行情境時，您要從佇列中執行的Webhook數目。

## 速率限制

目前的速率限製為每秒5個Webhook。 如果超過限制，則會傳回429狀態代碼。

## 非作用中Webhook的到期

已超過120小時未指派給任何情境的webhook會被移除。

## Webhook裝載

[!DNL Workfront Fusion]儲存webhook裝載30天。 存取webhook裝載時，若在裝載建立超過30天後進行，會導致&#39;&#39;[!UICONTROL 無法從儲存空間讀取檔案。]&#39;&#39;

## 錯誤處理

當您的案例中出現具有立即觸發器的錯誤時，案例：

* 立即停止 — 設定為立即執行[!UICONTROL 時]。
* 嘗試3次不成功後停止（3個錯誤） — 案例設定為依排程執行時。

如果案例執行期間發生錯誤，webhook會在即時觸發器的復原階段重新放入佇列中。 在此情況下，您可能會修正該案例並重新執行。 如需詳細資訊，請參閱文章[案例執行、週期和 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的階段[復原](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback)。

如果您的案例中存在Webhook回應模組，則會將錯誤傳送至Webhook回應。 Webhook回應模組一律在最後執行（在Scenario設定中的[!UICONTROL 自動認可]選項未啟用的情況下）。 如需詳細資訊，請參閱文章[Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)中的[回應Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi)。

## 自訂Webhook

您可以建立自己的Webhook。 如需詳細資訊，請參閱[Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)。

## Webhook停用

如果符合下列任一條件，Webhook就會自動停用：

* webhook已超過5天未連線至任何案例
* webhook僅用於非使用中情況，這些情況已非使用中超過30天。

如果停用的Webhook未連線至任何情境且處於停用狀態超過30天，則會自動刪除和取消註冊。


