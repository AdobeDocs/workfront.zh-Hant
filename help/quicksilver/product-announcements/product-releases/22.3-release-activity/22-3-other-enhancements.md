---
title: 22.3版本時間範圍內的其他更新
description: 22.3版本時間範圍內的其他更新
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3其他增強功能

本頁說明22.3版對預覽環境所做的所有其他增強功能。 這些增強功能已在2022年7月11日當週的生產環境中推出。 如需22.3版所有可用變更的清單，請參閱 [22.3版本總覽](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 已更新時程表

我們持續改進並更新您使用時程表的體驗。 以下是此更新包含的一些功能：

* 符合新Workfront體驗的新外觀。

* 自動儲存功能可在您新增時數及小時評論時自動儲存它們。

* 更直覺式的頁面配置，以符合其他物件頁面。 例如，我們在時程表中新增了左側面板。 時程表更新現在會顯示在左側面板的更新區段中。 您也可以從時程表頁面刪除時程表，並將時程表新增至您的最愛清單。

* 搜尋專案、任務或問題並將其新增到時程表時，獲得更好的體驗。 這符合Workfront中所有其他清單的體驗。

* 「摘要」面板可供任務和問題使用，以直接從時程表新增評論或更新資訊。


在目前的更新中，我們也已棄用下列功能：

* 從更新建立任務已移除。 自2018.2發行版本以來，此功能已從所有其他物件的更新區域移除，但仍可在時程表更新流中使用。

* 「從時程表新增費用」。 「偏好設定已從設定的時程表和時數偏好設定區域移除，您無法再從時程表記錄費用。 您仍然可以從任務和專案頁面記錄費用。


如需詳細資訊，請參閱下列文章：

* [瞭解時程表配置](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [設定時程表和小時偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## 左側導覽面板的增強功能

我們已對Adobe Workfront的左側導覽面板進行數個增強功能。

* 左側導覽面板的外觀和感覺已更新為Adobe設計標準，包括色彩和字型。

* 面板底部的「新增自訂區段」連結已重新命名為「新增儀表板」，以便更妥善地說明其功能。

## 在您的自訂OAuth2應用程式中啟用自動重新整理權杖輪換

為了讓您更能掌控自訂OAuth2應用程式的安全性，我們新增了啟用重新整理權杖輪換的選項。 啟用此選項後，每次使用重新整理權杖時，您的應用程式都會自動建立並傳送新的重新整理權杖，並停用舊的。

您的應用程式必須在每次重新整理後儲存新的重新整理Token。 Workfront不會儲存此重新整理Token。

先前，重新整理權杖會在自訂OAuth2應用程式設定中設定的一段時間後過期。

如需詳細資訊，請參閱 [為Workfront整合建立OAuth2應用程式](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## 在單頁網頁應用程式的自訂OAuth2整合中使用PKCE

您現在可以使用PKCE在自訂整合中建立單頁網頁應用程式。 PKCE是安全的授權流程，非常適用於動態重新整理應用程式（例如行動應用程式），但在所有OAuth2使用者端都很有價值。 PKCE不使用靜態使用者端密碼，而是使用動態產生的字串，消除了使用者端密碼洩漏的風險。

之前，自訂OAuth2應用程式的可用選項是使用使用者的名稱和密碼或使用者端密碼。

如需詳細資訊，請參閱 [為Workfront整合建立OAuth2應用程式](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
