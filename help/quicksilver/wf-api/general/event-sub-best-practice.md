---
content-type: api
navigation-topic: general-api
title: 事件訂閱最佳實務
description: 事件訂閱最佳實務
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 事件訂閱最佳實務

Adobe Workfront事件訂閱訊息會在您正確設定服務並建立事件訂閱以觸發這些訊息傳送後，從Workfront自動傳送。 若要進一步了解如何正確設定事件訂閱，請參閱 [事件訂閱傳送需求](../../wf-api/general/setup-event-sub-endpoint.md).


以下列出幾個最佳實務，可協助您有效建立事件訂閱。

## 提供所有必要的請求正文欄位

請確定所有必要的要求內文欄位皆已提供給API。 如需所有必要請求屬性的相關資訊，請參閱 [事件訂閱API](../../wf-api/general/event-subs-api.md).

## 避免包含額外的內文欄位

請求中請勿包含額外的內文欄位，因為這會導致API無法建立訂閱。

## 在寬限期內完成測試

嘗試在100個訊息的寬限期內完成所有訂閱測試。 若要深入了解此寬限期，請參閱 [常見問題集 — 事件訂閱](../../wf-api/general/event-subs-faq.md).

## 符合標準事件訂閱訊息傳送需求

確認訂閱端點符合標準事件訂閱訊息傳送要求。 若要了解這些需求，請參閱 [事件訂閱傳送需求](../../wf-api/general/setup-event-sub-endpoint.md).

## 允許按全域區域列出IP地址

若要透過防火牆接收事件訂閱裝載，您必須依全域地區將IP位址新增至允許清單。 若要進一步了解，請參閱 [事件訂閱API](../../wf-api/general/event-subs-api.md).

## 擁有正確的存取層級和API金鑰

若要建立、查詢或刪除事件訂閱，您的Workfront使用者需：

* 的存取層級 **系統管理員**
若要進一步了解，請參閱 [授予使用者完整的管理存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) 或 [授予用戶對特定區域的管理訪問權限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* API金鑰

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
