---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion發行活動：《2022年11月7日周》'
description: 本頁說明2022年11月7日當周在Adobe Workfront Fusion中所做的所有增強功能。
author: Luke
feature: Product Announcements, Workfront Fusion
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 9aaba3062bc5d1166c37821a6a3216f7f1d965b1
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Workfront Fusion發行活動：2022年11月7日當周

**Webhook隊列優化**

此版本已最佳化Fusion的Webhook佇列。 接受Webhook的服務現在與佇列和其他程式分開。 這項更改使Fusion能夠以更快且更一致的速率處理Webhook隊列成為可能。

在實施此變更期間，我們更了解佇列Webhook事件的預期記錄處理時間。 Fusion的Webhook檢視器頁面預計不會超過1分鐘。

若要查看目前已排入佇列的Webhook事件，請導覽至左側導覽中的Webhook。 分子中具有數字的卡車圖示表示該網頁鈎的佇列事件。 按一下卡車圖示，即可查看已排入佇列的事件。

![](assets/fusion-webhook-queue-1866x567.png)


**未使用的Webhook現在將停用或刪除**

我們已對Workfront Fusion處理未使用WebHook的方式做了一些變更。 現在，如果下列任一情況適用，wWebhook就會自動停用：

* Webhook已超過5天未連接到任何情況。
* Webhook僅用於已停用超過30天的非作用中案例。

如果停用的WebHook未連線至任何案例，且已停用30天以上，系統就會自動刪除並取消註冊。
