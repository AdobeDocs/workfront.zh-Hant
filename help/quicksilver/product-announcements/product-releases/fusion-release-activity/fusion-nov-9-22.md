---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 「Workfront Fusion發行活動： 2022年11月7日當週」
description: 本頁說明2022年11月7日當週在Adobe Workfront Fusion中所做的所有增強功能。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Workfront Fusion發行活動： 2022年11月7日當週

**Webhook佇列最佳化**

此發行版本已最佳化Fusion的webhook佇列。 接受webhook的服務現在與佇列和其他處理序分開。 此變更讓Fusion能夠以更快、更一致的速率處理webhook佇列。

在此變更實作期間，我們能夠更清楚瞭解已排入佇列的webhook事件的預期記錄處理時間。 Fusion的webhook檢視器頁面預計不會超過1分鐘。

若要檢視目前排入佇列的Webhook事件，請在左側導覽中導覽至Webhook。 分子中帶有數字的卡車圖示表示該webhook的佇列事件。 按一下卡車圖示以檢視已排入佇列的事件。

![](assets/fusion-webhook-queue-1866x567.png)


**未使用的Webhook現在將會停用或刪除**

我們已對Workfront Fusion處理未使用Webhook的方式進行一些變更。 現在，如果符合下列任一條件，Webhook就會自動停用：

* webhook已超過5天未連線至任何案例。
* webhook僅用於非使用中情況，這些情況已非使用中超過30天。

如果停用的Webhook未連線至任何情境且處於停用狀態超過30天，則會自動刪除和取消註冊。
