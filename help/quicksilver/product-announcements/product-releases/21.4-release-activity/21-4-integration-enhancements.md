---
title: 21.4整合增強功能
description: 21.4整合增強功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4整合增強功能

本頁說明21.4版對預覽環境所做的所有整合增強功能。 這些增強功能將在2021年10月4日當週的生產環境中提供。

如需21.4版本可用的所有變更清單，請參閱[21.4版本總覽](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md)。

## 從Dropbox企業連結檔案

我們已將Dropbox Business新增為可用的檔案整合。 現在，您可以直接從Workfront內部存取儲存在Dropbox Business中的檔案。

「Dropbox業務」可讓您連結共用檔案，並將檔案上傳至共用資料夾。 Dropbox (而非Dropbox企業)只允許檔案的擁有者在Workfront中檢視檔案。

您的Workfront管理員可為貴組織啟用此整合。

如需詳細資訊，請參閱[從外部應用程式連結檔案](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

如需Workfront管理員如何啟用此選項的詳細資訊，請參閱[設定檔案整合](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)。

## 更新適用於Slack的Workfront

下列更新現在可在Workfront中看到，以進行Slack整合：

* 適用於Slack的Workfront有全新的外觀。
* 現在您會即時收到Workfront的Slack通知。

  例如，如果您被指派給任務，您會在被指派後立即收到該通知。 以前，通知出現在Slack中之前可能會有所延遲。

此更新需要您重新授權Workfront進行Slack整合。 如需授權整合的資訊，請參閱[為Slack設定Adobe Workfront](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

如需有關Slack通知之Workfront的詳細資訊，請參閱[在Slack中接收Adobe Workfront通知](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)。

## 在同意Adobe Workfront整合時，可更清楚檢視帳戶存取的詳細資訊

Adobe Workfront整合的同意畫面現已更新。 現在，您可以檢視整合功能可存取的特定動作和區域，以便更清楚瞭解您允許整合或應用程式存取的內容。

這個新的同意畫面適用於使用OAuth 2.0的任何Adobe Workfront整合。

如需特定整合的詳細資訊，請參閱該整合的檔案。

## 整合不再需要使用API金鑰驗證

Workfront整合最近開始使用OAuth2來提高安全性和可用性。 在此移動中，Workfront不再需要API金鑰以進行整合驗證。
