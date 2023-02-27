---
content-type: api
navigation-topic: general-api
title: 事件訂閱傳送需求
description: 事件訂閱傳送需求
author: Becky
feature: Workfront API
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# 事件訂閱傳送需求

事件訂閱訊息是可設定的通知，以在發生某些事件時通知使用者。 若要進一步了解事件訂閱，請參閱 [常見問題集 — 事件訂閱](../../wf-api/general/event-subs-faq.md).

## 事件訂閱訊息傳送標準

使用Adobe Workfront事件訂閱訊息的服務端點必須符合下列基本需求，才能確保訊息可正確傳送和接收：

* 服務端點必須接受HTTPPOST請求。 HTTPPOST是用於事件訂閱訊息（包括驗證訊息）所有傳送的要求方法。

* 為了讓事件訂閱傳送系統確認已成功接收訊息，端點必須為所有傳入訊息傳回200層級HTTP狀態（例如200 OK或202）。

* 如果未返回200級狀態，則事件訂閱系統會假設消息未成功傳送，並開始應用相應的重試策略。 要了解有關Workfront重試策略的詳細資訊，請參閱 [事件訂閱重試次數](../../wf-api/api/event-sub-retries.md).

* 與返回200級狀態作為響應狀態一起，必須在嘗試傳送後的5秒內接收HTTP響應。此約束確保消費者業務流程或基礎架構限制不會延遲傳送其他待傳送郵件。

* 如果長期執行的業務流程從事件訂閱訊息觸發，Workfront建議

   1. 終結點在收到消息時保存消息資訊，並立即以200級狀態進行響應。
   1. 端點回應事件訂閱傳送請求後，即可處理儲存的訊息。
