---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1其他增強功能
description: 本頁說明2020.1版中對Workfront一般區域進行的所有增強功能。 這些增強功能目前可在「預覽」環境中取得，並將於2020年3月底或4月初在「生產」環境中取得。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1其他增強功能

本頁說明2020.1版中對Workfront一般區域進行的所有增強功能。 這些增強功能目前可在「預覽」環境中取得，並將於2020年3月底或4月初在「生產」環境中取得。

如需2020.1版所有可用變更的清單，請參閱[2020.1版總覽](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md)。

## 將校樣新增至允許清單所需變更

>[!NOTE]
>
>此功能已從2020.1版本中移除。 稍後將可供使用。

校訂網域正在從proofhq.com變更為workfront.com。

如果您的防火牆或郵件伺服器設定為僅允許特定廠商存取，您必須將下列額外URL新增至允許清單，以確保貴組織中的使用者可在瀏覽器校訂檢視器和案頭校訂檢視器中檢視Workfront中的校訂：

&#42;.workfront.com

&#42;proofhq.com URL也是必要的。

如需更新允許清單的詳細資訊，請參閱[設定防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

>[!NOTE]
>
>此更新僅適用於Workfront內的校訂，不適用於使用Workfront Proof獨立應用程式。

## 更新Workfront Cookie行為以維持與Chrome的相容性

為了與即將推出的Google Chrome更新(Chrome v80)保持相容性，我們已更新Workfront平台以確保可正確傳送包含請求的Cookie。

此Chrome更新會變更SameSite Cookie屬性的預設值。 如果您想要測試Workfront執行個體在Google Chrome更新後的行為，請調整Chrome中的標幟，並啟用下列選項：

* &quot;預設SameSite Cookie&quot;
* 「不含SameSite的Cookie必須是安全的」

## Workfront註解同步至Jira

適用於Jira整合的Workfront現在會將您的Workfront註解同步至Jira的原生註解流。

之前，您可以將Jira的評論同步至Workfront，但不能將Workfront的評論同步至Jira。

如需詳細資訊，請參閱[設定Jira的Adobe Workfront](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 已移除FlashPortfolio最佳化工具

我們已移除針對所有客戶，從Workfront Classic環境切換新舊版(根據Flash)Portfolio最佳化工具的功能。 舊版Portfolio最佳化工具是一項過時的功能，現今的新工具可提供相同的功能。

如需專案組合最佳化工具的相關資訊，請參閱https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

如需有關在Workfront中棄用Flash型工具的資訊，請參閱[在Adobe Workfront中取代Flash型工具](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md)。
