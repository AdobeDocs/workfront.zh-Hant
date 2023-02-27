---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱重試次數
description: 事件訂閱重試次數
author: Becky
feature: Workfront API
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 事件訂閱重試次數

實作訊息傳遞系統時，必須處理一些警告，以確保穩定性、一致性和良好的使用者體驗。 消息傳遞系統的一個缺點是確保消息成功到達其目的地，並知道在消息未到達時該做什麼。

有些整合功能會接受傳送失敗，然後放置訊息並移至下一則訊息。  在其他整合中，無法傳送訊息的情況無法忽略。 例如，金融整合可能會嘗試傳送訊息，但會收到HTTP狀態代碼404，這表示伺服器找不到要傳送訊息的端點。 在這種情況下，遺漏的資訊可能意味著某人沒有按時獲得報酬，或某個組織正在審查合同資源的預算。

## Adobe Workfront事件訂閱重試策略

由於客戶將Workfront平台當成日常知識工作的核心，Workfront事件訂閱架構提供一種機制，可確保盡可能最充分地嘗試傳送每則訊息。

無法傳送至客戶端點的事件觸發傳出訊息會重新傳送，直到傳送成功為止，最長48小時。 在此期間，重試會以逐漸減少的頻率發生，直到傳送成功或48小時過去為止。

客戶需要確保使用Workfront事件訂閱之傳出訊息的任何端點都已設定，以便在傳送成功時，將200層級的回應訊息傳回Workfront。

## 處理失敗的事件觸發的傳出訊息

以下流程圖顯示了使用「Workfront事件訂閱」重新嘗試傳送訊息的策略：

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

以下說明與流程圖中描述的步驟相對應：

1. 無法傳遞訊息。
1. 已記錄訊息傳送失敗資訊。

   記錄所有傳送訊息的失敗嘗試，以便執行偵錯，以判斷指定失敗或一連串失敗的根本原因。

1. URL失敗增加。
1. 消息嘗試計數增加。
1. 計算延遲，直到將再次嘗試此郵件的傳送。
1. 消息被放置到消息重試隊列中。

   如前面的流程圖所示，用於處理消息傳送重試的消息隊列是與處理每個消息的初始傳送嘗試的隊列不同的隊列。 這允許接近即時的消息流繼續不受任何消息子集的故障的影響。

1. 評估URL電路狀態。 發生下列任一情況：

   * 如果電路已開啟，且目前不允許傳送，請在步驟5重新啟動程式。
   * 如果電路為半開，表示我們的電路目前已開啟，但已經過足夠的時間來測試URL，以查看傳送至它的問題是否已解決。
   * 如果已達到郵件傳送嘗試限制（重試48小時），則會捨棄郵件

1. 如果URL電路已關閉並允許傳送，請嘗試傳送訊息。 如果此傳送失敗，訊息會在步驟1重新啟動

1. 如果URL電路已關閉並允許傳送，請嘗試傳送訊息。 如果此傳送失敗，訊息會在步驟1重新啟動。

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
