---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]
description: 許多服務都提供WebHook，以便在服務中發生特定更改時提供即時通知。 若要處理這些通知，建議您使用即時觸發程式。 本文說明在Adobe Workfront Fusion中使用即時觸發程式的功能。
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 04191419ab6079cc34576b5a7532cd1596e4b91d
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# 中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]

許多服務都提供WebHook，以便在服務中發生特定更改時提供即時通知。 若要處理這些通知，建議您使用即時觸發程式。 您可輕鬆識別 [!DNL Adobe Workfront Fusion] 因為他們的標籤：

![](assets/instant-350x256.png)

如果服務未提供Webhook，則您需要使用輪詢觸發器定期輪詢服務。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 檢視Webhook的佇列

來自傳入WebHook的所有消息都儲存在WebHook的隊列中。

1. 按一下 **[!UICONTROL Webhook]** 的上界。
1. 找到要查看隊列的Webhook。
1. 按一下帶有卡車圖示的按鈕，以及收到的Webhook數量。

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >無論您如何設定選項，傳入的Webhook資料都始終儲存在隊列中 [!UICONTROL 資料] 是機密(如 [中的藍本設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md))。 在案例中處理資料後，資料就會從系統中永久刪除。

## 排程即時觸發

如果您的案例包含即時觸發器，您可以排程該案例以立即執行：

![](assets/schedule-setting-350x185.png)

在此情況下，您的案例會在 [!DNL Workfront Fusion] 從服務接收新資料。 執行情境後，會計算佇列中等待的待處理WebHook的總數，且情境的執行週期與有待處理WebHook的相同，每個週期處理一個WebHook。 如需詳細資訊，請參閱 [中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* 循環與方案運行不同。 1個方案執行內可以有多個週期。
>* 當您執行計畫為即時的即時觸發的案例時，會套用下列例外：
   >
   >     * 兩個執行之間的間隔不受定價計畫中的最小間隔的限制。

      >
      >       例如，一旦情境完成執行，就會再次檢查Webhook的佇列。 如果有任何掛起的WebHook，則情境會立即再次執行，並再次處理所有掛起的WebHook。
   >   
   >     * 「最大週期數」情境設定會忽略，並設為100，這表示在單一情境執行期間（每個週期1個事件的速率）不會處理超過100個擱置的WebHook。
>



如果您使用以下任何其他排程設定： [!UICONTROL 立即]，則會依您指定的間隔執行情境。 由於在間隔期間可在佇列中收集數個WebHook，因此建議設定 [[!UICONTROL 最大循環數]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) 值高於預設值1，以在一個案例中執行處理多個Webhook:

1. 按一下 [!UICONTROL 藍本設定] 圖示 ![](assets/gear-icon-settings.png) 在案例底部。
1. 在 **[!UICONTROL 藍本設定]** 框中，鍵入數字 **[!UICONTROL 最大循環數]** 框，指定每次執行該方案時要運行的隊列中的webhook數。

## 比率限制

目前的速率限制為每秒5個Webhook。 如果超過限制，則會傳回429狀態代碼。

## 非作用中WebHook的過期

系統會移除已超過120小時未指派給任何案例的WebHook。

## Webhook負載

[!DNL Workfront Fusion] 儲存webhook負載30天。 在建立Webhook裝載後30天以上存取該裝載會導致錯誤「[!UICONTROL 無法從儲存讀取檔案。]&quot;

## 錯誤處理

當您的案例中發生即時觸發的錯誤時，該案例會：

* 立即停止 — 當設定為運行情況時 [!UICONTROL 立即].
* 在3次失敗嘗試後停止（3個錯誤） — 當情境設為如排程執行時。

如果在方案執行期間發生錯誤，則在即時觸發器的回滾階段期間，Webhook會重新放入佇列中。 在此情況下，您可以修正案例並重新執行。 如需詳細資訊，請參閱 [回復](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 在文章中 [中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

如果您的案例中有Webhook回應模組，則會將錯誤傳送至Webhook回應。 Webhook回應模組一律會執行於最後(若 [!UICONTROL 自動提交] 選項)。 如需詳細資訊，請參閱 [回應Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) 在文章中 [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## 自訂Webhook

您可以建立自己的Webhook。 如需詳細資訊，請參閱 [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook停用

如果下列任一情況適用，Webhook就會自動停用：

* Webhook已超過5天未連接到任何情況
* Webhook僅用於已停用超過30天的非作用中案例。

如果停用的WebHook未連線至任何案例，且已停用30天以上，系統就會自動刪除並取消註冊。


