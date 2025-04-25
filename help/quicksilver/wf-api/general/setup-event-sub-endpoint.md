---
content-type: api
navigation-topic: general-api
title: 事件訂閱傳送需求
description: 事件訂閱傳送需求
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# 事件訂閱傳送需求

事件訂閱訊息是通知，可設定為在某些事件發生時通知使用者。 若要深入瞭解哪些是事件訂閱，請參閱[常見問題集 — 事件訂閱](../../wf-api/general/event-subs-faq.md)。

## 事件訂閱訊息傳遞的標準

使用Adobe Workfront事件訂閱訊息的服務端點必須符合下列基本要求，才能確保訊息可正確傳送及接收：

* 服務端點必須接受HTTP POST要求。 HTTP POST是在所有傳送事件訂閱訊息（包括驗證訊息）中使用的要求方法。

* 為了讓事件訂閱傳遞系統確認訊息已成功接收，端點必須為所有傳入訊息傳回200層級HTTP狀態（例如，200 OK或202）。

* 如果未傳回200層級的狀態，事件訂閱系統會假設訊息未成功傳遞，並開始套用適當的重試原則。 若要深入瞭解Workfront重試原則，請參閱[事件訂閱重試](../../wf-api/api/event-sub-retries.md)。

* 在將200層級狀態傳回為回應狀態的同時，您必須在傳送嘗試開始後的五秒內收到HTTP回應。此限制可確保消費者業務程式或基礎架構限制不會延遲傳送其他擱置傳送的訊息。

* 如果由事件訂閱訊息觸發的長期執行業務流程，Workfront建議  該

   1. 端點會在收到訊息時儲存訊息資訊，並立即以200層級狀態回應。
   1. 端點回應事件訂閱傳遞請求後，即可處理儲存的訊息。

* 事件訂閱訊息或物件不能大於1 MB。
