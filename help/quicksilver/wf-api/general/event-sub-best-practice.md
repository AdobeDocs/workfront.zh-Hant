---
content-type: api
navigation-topic: general-api
title: 活動訂閱最佳實務
description: 活動訂閱最佳實務
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
TQID: https://experienceleague.adobe.com/uT7erlnJR5-h-KKGQiuztzZKBtwtEvWQ8U-EUgN4TG4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 15%

---

# 活動訂閱最佳實務

在您正確設定服務並建立事件訂閱以觸發這些訊息傳送後，Adobe Workfront事件訂閱訊息就會自動從Workfront傳送。 若要深入瞭解如何正確設定事件訂閱，請參閱[事件訂閱傳遞需求](../../wf-api/general/setup-event-sub-endpoint.md)。


以下列出一些最佳實務，協助您有效建立事件訂閱。

## 提供所有必要的請求內文欄位

請確定所有必要的請求內文欄位均已提供給API。 如需所有必要要求屬性的相關資訊，請參閱[事件訂閱API](../../wf-api/general/event-subs-api.md)。

## 避免包含額外的內文欄位

請勿在請求中包含額外的內文欄位，因為這會導致API無法建立訂閱。

## 避免讓事件訂閱超載

事件訂閱服務旨在為所有使用者提供可靠的事件傳送。 為了確保這一點，已經實施了防護措施，以防止單一使用者產生過多的事件，從而可能對所有使用者造成服務品質問題。 因此，在短時間內以高頻率產生過多事件的使用者，可能會經歷沙箱化和事件傳遞延遲的情況。

## 在寬限期內完成測試

嘗試在100則訊息的寬限期內完成所有訂閱測試。 若要深入瞭解此寬限期，請參閱[常見問題集 — 活動訂閱](../../wf-api/general/event-subs-faq.md)。

## 符合標準事件訂閱訊息傳送需求

確認您的訂閱端點符合標準事件訂閱訊息傳送要求。 若要瞭解這些需求，請參閱[事件訂閱傳遞需求](../../wf-api/general/setup-event-sub-endpoint.md)。

## 依全域區域的允許清單IP位址

若要透過防火牆接收事件訂閱裝載，您必須依全域區域將IP位址新增至允許清單。 若要深入瞭解，請參閱[事件訂閱API](../../wf-api/general/event-subs-api.md)。

## 擁有正確的存取層級和驗證

若要建立、查詢或刪除事件訂閱，您的Workfront使用者需要：

* **系統管理員的存取層級**
若要瞭解更多資訊，請參閱[授予使用者完整管理存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)或[授予使用者對特定區域的管理存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* 如果您的組織使用Adobe IMS （Identity Management系統），請包含在`X-User-Token`標頭中傳遞的IMS使用者權杖。
