---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱重試次數
description: 事件訂閱重試次數
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 0325d305c892c23046739feff17d4b1fc11100cc
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 事件訂閱重試次數

實作訊息傳送系統時，為了確保穩定性、一致性和良好的使用者體驗，有一些需要注意的事項。 訊息傳送系統的缺點之一，是確保訊息成功到達目的地，以及知道訊息無法到達時該怎麼做。

有些整合功能可能會接受傳送失敗，然後捨棄訊息並移至下一個訊息。  在其他整合中，無法忽略傳送訊息的失敗。 例如，財務整合可能會嘗試傳遞訊息，但收到HTTP狀態代碼404，表示伺服器找不到要傳遞訊息的端點。 在這種情況下，遺漏訊息可能意味著某人未收到時間報酬，或組織超過合約資源的預算。

## 事件訂閱重試的Adobe Workfront策略

由於客戶將Workfront平台當做其日常知識工作的核心部分，因此Workfront事件訂閱架構提供的機制可確保儘可能全力傳送每則訊息。

無法傳送至客戶端點的事件觸發傳出訊息會重新傳送，直到傳送成功為止，最長可達48小時。 在此期間，重試的頻率會遞增到傳送成功或進行11次嘗試為止。

這些重試嘗試的公式為：

`((2^attempt) - 1) * 84800ms`

第一次重試在1.5分鐘後發生，第二次在約5分鐘後發生，而第11次在約48小時後發生。

客戶需要確保當傳送成功時，任何使用Workfront事件訂閱傳出訊息的端點都會設定為傳回200層級的回應訊息至Workfront。

## 已停用和凍結的訂閱規則

* 如果訂閱URL的失敗率超過70%，超過100次嘗試，或有2,000次連續失敗，則&#x200B;**已停用**
* 如果訂閱URL連續失敗超過2,000次，而且上次成功是在超過72小時之前，或是在任何時間範圍內連續失敗超過50,000次，則訂閱URL為&#x200B;**凍結**。
* **已停用**&#x200B;訂閱URL將繼續每10分鐘嘗試傳送一次，並在成功傳送後重新啟用。
* **凍結**&#x200B;訂閱URL絕對不會嘗試傳送，除非透過發出API要求來手動啟用。



<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
