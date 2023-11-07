---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱重試次數
description: 事件訂閱重試次數
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 事件訂閱重試次數

實作訊息傳送系統時，為了確保穩定性、一致性和良好的使用者體驗，有一些需要注意的事項。 訊息傳送系統的缺點之一，是確保訊息成功到達目的地，以及知道訊息無法到達時該怎麼做。

有些整合功能可能會接受傳送失敗，然後捨棄訊息並移至下一個訊息。  在其他整合中，無法忽略傳送訊息的失敗。 例如，財務整合可能會嘗試傳遞訊息，但收到HTTP狀態代碼404，表示伺服器找不到要傳遞訊息的端點。 在這種情況下，遺漏訊息可能意味著某人未收到時間報酬，或組織超過合約資源的預算。

## 事件訂閱重試的Adobe Workfront策略

由於客戶將Workfront平台當做其日常知識工作的核心部分，因此Workfront事件訂閱架構提供的機制可確保儘可能全力傳送每則訊息。

無法傳送至客戶端點的事件觸發傳出訊息會重新傳送，直到傳送成功為止，最長可達48小時。 在此期間，會以遞減的頻率重試，直到傳送成功或直到48小時為止。

客戶需要確保當傳送成功時，任何使用Workfront事件訂閱傳出訊息的端點都會設定為傳回200層級的回應訊息至Workfront。

## 處理失敗的事件觸發傳出訊息

以下流程圖顯示使用Workfront事件訂閱重新嘗試訊息傳送的策略：

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

下列說明與流程圖中描述的步驟相對應：

1. 訊息無法傳遞。
1. 訊息傳送失敗資訊會記錄下來。

   所有傳送訊息的失敗嘗試都會記錄下來，以便執行偵錯以判斷指定失敗或一系列失敗的根本原因。

1. URL失敗次數會增加。
1. 訊息嘗試計數會增加。
1. 計算延遲，直到再次嘗試此訊息的傳遞。
1. 訊息已放置到訊息重試佇列中。

   如前面的流程圖所示，用於處理訊息傳送重試的訊息佇列與處理每則訊息之初始傳送嘗試的佇列是不同的佇列。 這可讓近乎即時的訊息流程不受任何訊息子集失敗所阻礙。

1. 已評估URL電路狀態。 會發生下列其中一種情況：

   * 如果電路已開啟且目前不允許傳遞，請在步驟5重新啟動此程式。
   * 如果電路是半開啟的，這表示我們的電路目前是開啟的，但已經過了足夠的時間來測試URL，以檢視傳送給它的問題是否已解決。
   * 如果已達到訊息傳送嘗試限制（重試達48小時），則會捨棄訊息

1. 如果URL電路已關閉並允許傳送，請嘗試傳送訊息。 如果此傳送失敗，訊息將在步驟1重新啟動

1. 如果URL電路已關閉並允許傳送，請嘗試傳送訊息。 如果此傳送失敗，訊息將在步驟1重新啟動。

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
