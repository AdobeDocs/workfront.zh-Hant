---
title: 21.4整合增強功能
description: 21.4整合增強功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 21.4整合增強功能

本頁說明在「預覽」環境中21.4版所進行的所有整合增強功能。 這些增強功能將於2021年10月4日當周在生產環境中提供。

如需21.4版所有可用變更的清單，請參閱 [21.4版本概觀](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 從Dropbox業務連結文檔

我們已將Dropbox業務新增為可用的檔案整合。 現在，您可以直接從Workfront記憶體取儲存在Dropbox業務中的檔案。

Dropbox業務允許您連結共用文檔並將文檔上傳到共用資料夾。 Dropbox(非Dropbox業務)僅允許文檔的所有者在Workfront中查看文檔。

您的Workfront管理員可為貴組織啟用此整合。

如需詳細資訊，請參閱 [從外部應用程式連結文檔](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

如需Workfront管理員如何啟用此選項的詳細資訊，請參閱 [配置文檔整合](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## 更新Workfront以Slack

Workfront中現在會顯示下列更新以進行Slack整合：

* Workfront的Slack有了新的外觀。
* 現在您會即時收到Workfront以取得Slack通知。

   例如，如果您被指派給任務，則在指派您後，您會立即收到該通知。 之前，通知可能會延遲，之後才會出現在Slack中。

此更新需要您重新授權Workfront，以整合Slack。 如需授權整合的詳細資訊，請參閱 [設定Adobe Workfront以Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

如需Workfront的詳細資訊，請參閱Slack通知 [以Slack接收Adobe Workfront通知](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## 在同意Adobe Workfront整合時，更清楚地查看帳戶存取的詳細資訊

Adobe Workfront整合的同意畫面現已更新。 現在，您可以查看整合功能可存取的特定動作和區域，以便您更清楚了解允許整合或應用程式存取的內容。

這個新的同意畫面適用於使用OAuth 2.0的任何Adobe Workfront整合。

如需特定整合的詳細資訊，請參閱該整合的檔案。

## 整合不再需要API金鑰驗證

Workfront整合功能最近已開始使用OAuth2，以提升安全性和可用性。 Workfront不再需要API金鑰才能進行整合驗證，這是移動的一部分。
