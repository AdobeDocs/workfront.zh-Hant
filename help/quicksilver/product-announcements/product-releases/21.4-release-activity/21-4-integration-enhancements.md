---
title: 21.4整合增強功能
description: 21.4整合增強功能
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
TQID: https://experienceleague.adobe.com/dCRr9YQiXiX82Jw7wyeT786T8oJ74-u6kOuevYy-SWY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 367
ht-degree: 0%

---

# 21.4整合增強功能

本頁說明21.4版對預覽環境所做的所有整合增強功能。 這些增強功能將在2021年10月4日當週的生產環境中提供。

如需21.4版本可用的所有變更清單，請參閱[21.4版本總覽](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md)。

## 從Dropbox Business連結檔案

我們已將Dropbox商務新增為可用的檔案整合。 現在，您可以直接從Workfront內部存取儲存在Dropbox Business中的檔案。

Dropbox Business可讓您連結共用檔案，並將檔案上傳至共用資料夾。 Dropbox （非Dropbox Business）僅允許檔案擁有者在Workfront中檢視檔案。

您的Workfront管理員可為貴組織啟用此整合。

如需詳細資訊，請參閱[從外部應用程式連結檔案](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

如需Workfront管理員如何啟用此選項的詳細資訊，請參閱[設定檔案整合](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)。

## 適用於Slack的Workfront更新

用於Slack整合的Workfront現在會顯示下列更新：

* 適用於Slack的Workfront有全新的外觀。
* 現在您會即時收到Slack的Workfront通知。

  例如，如果您被指派給任務，您會在被指派後立即收到該通知。 之前，通知出現在Slack中可能會有延遲。

此更新需要您重新授權Workfront以進行Slack整合。 如需授權整合的資訊，請參閱[設定Slack的Adobe Workfront](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

如需有關適用於Slack通知的Workfront的詳細資訊，請參閱[在Slack中接收Adobe Workfront通知](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)。

## 在同意Adobe Workfront整合時，可更清楚檢視帳戶存取的詳細資訊

Adobe Workfront整合的同意畫面現已更新。 現在，您可以檢視整合功能可存取的特定動作和區域，以便更清楚瞭解您允許整合或應用程式存取的內容。

這個新的同意畫面適用於使用OAuth 2.0的任何Adobe Workfront整合。

如需特定整合的詳細資訊，請參閱該整合的檔案。

## 整合不再需要使用API金鑰驗證

Workfront整合最近開始使用OAuth2來提高安全性和可用性。 在此移動中，Workfront不再需要API金鑰以進行整合驗證。
