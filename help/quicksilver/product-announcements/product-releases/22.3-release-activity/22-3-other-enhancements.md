---
title: 22.3版本期間的其他更新
description: 22.3版本期間的其他更新
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 22.3其他增強功能

本頁說明在「預覽」環境中22.3版所做的所有其他增強功能。 這些增強功能已於2022年7月11日當周在生產環境中推出。 如需22.3版所有可用變更的清單，請參閱 [22.3版本概觀](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 更新工時單

我們將繼續改進和更新您使用工時單的體驗。 以下是此更新包含的部分功能：

* 符合新Workfront體驗的新外觀與風格。

* 自動儲存功能可在您新增記錄的小時和小時留言時自動儲存。

* 更符合其他物件頁面的直覺式頁面配置。 例如，我們已將左面板新增至時間表。 時間表更新現在顯示在左側面板的「更新」部分中。 您也可以從時間表頁中刪除時間表，並將時間表添加到您的收藏夾清單中。

* 在搜索項目、任務或問題並將其添加到時間表時提供更好的體驗。 這會符合Workfront中其他所有清單中的體驗。

* 「摘要」面板可用於任務和問題，以便直接從時間表添加註釋或更新資訊。


在目前的更新中，我們也已棄用下列功能：

* 已移除從更新建立任務。 自2018.2版本以來，已從所有其他對象的「更新」區域中移除此功能，但時間表更新流中仍可使用此功能。

* 「從時間表中添加費用」。 「首選項已從「設定」的「時間表和小時首選項」區域中刪除，您無法再從時間表記錄費用。 您仍然可以從任務和項目頁記錄費用。


如需詳細資訊，請參閱下列文章：

* [了解工時單佈局](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [配置工時單和小時首選項](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## 左側導覽面板的增強功能

我們已對Adobe Workfront的左側導覽面板進行數項增強。

* 左側導覽面板的外觀和風格已更新為Adobe設計標準，包括顏色和字型。

* 面板底部的「新增自訂區段」連結已重新命名為「新增控制面板」，以更好地說明其功能。

## 在您的自訂OAuth2應用程式中啟用自動重新整理代號旋轉

為讓您更能控制自訂OAuth2應用程式的安全性，我們已新增至啟用重新整理代號旋轉的選項。 啟用此選項時，每次使用重新整理Token時，您的應用程式都會自動建立並傳送新的重新整理Token，並停用舊的Token。

您的應用程式必須在每次重新整理後儲存新的重新整理Token。 Workfront不會儲存此重新整理Token。

之前，在自訂OAuth2應用程式設定中設定的設定時間長度後，重新整理代號會過期。

如需詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## 在針對單頁Web應用程式的定製OAuth2整合中使用PKCE

您現在可以使用PKCE在自定義整合中建立單頁Web應用程式。 PKCE是一種安全的授權流，它與動態刷新應用程式（如移動應用程式）的效能良好，但在所有OAuth2客戶端中都很有價值。 PKCE不使用靜態客戶端密碼，而是使用動態生成的字串，從而消除了洩露的客戶端密碼的風險。

之前，自訂OAuth2應用程式的可用選項會使用使用者名稱和密碼，或用戶端密碼。

如需詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
