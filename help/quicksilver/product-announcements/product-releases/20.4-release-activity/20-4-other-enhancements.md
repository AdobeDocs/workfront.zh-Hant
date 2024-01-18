---
title: 20.4其他增強功能
description: 20.4其他增強功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4其他增強功能

本頁說明20.4版對「預覽」環境所做的所有其他增強功能。 這些增強功能將在2020年11月9日當週的生產環境中提供。

如需20.4版所有可用變更的清單，請參閱 [20.4版本總覽](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 管理員的新增功能：切換Workfront環境選項可用

為了提供更有效率、更方便的體驗，群組管理員和Workfront管理員現在可以從Workfront中的任何頁面，快速地在不同的Workfront環境之間切換，而無需登出。

在新的Workfront體驗中，「主要功能表」中會顯示「切換至Classic 」選項。

在Workfront Classic中，按一下「全域導覽列」右上角的設定檔圖片時，選單中會顯示切換到新體驗選項。

此功能現已包含在 [管理員基礎課程，第1部分學習路徑](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) 在Workfront One上。

## Workfront Proof的改良加密

我們正進行一些變更，以改善Workfront校訂應用程式的資料動態加密強度。 弱的TLS加密將於2020年11月11日淘汰。

存取Workfront時，請確定您使用支援的瀏覽器。 如需有關受支援瀏覽器的詳細資訊，請參閱 [Adobe Workfront瀏覽器需求](../../../workfront-basics/workfront-browser-requirements.md).

## 3個電子郵件範本的新外觀

為了改善可讀性和整體體驗，以下電子郵件範本具有新的外觀和風格：

* 新的工作請求
* 指派給您的依存性任務現已準備開始
* 具有前置任務完成的團隊電子郵件通知

若要在預覽環境中啟用電子郵件以進行測試，請參閱中的在預覽中管理電子郵件區段 [修改您自己的電子郵件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 團隊的新電子郵件通知

我們已新增下列團隊電子郵件通知：

* 指派給我的團隊之任務的前置任務已完成：當其其中一個任務的前置任務被標籤為完成時，指派的團隊會收到電子郵件通知。
* 指派給我的團隊之任務的所有前置任務已完成：指派的團隊會收到每個標示為完成之前置任務的電子郵件通知。

如需詳細資訊，請參閱 [通知：關於指派給我的工作的資訊](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## 管理員的新增功能：電子郵件通知增強功能

現在，只要按一下，您就可以在「設定」中啟用或停用事件電子郵件通知。 只需按一下通知名稱旁邊的開啟/關閉開關。

此外，請注意我們的現代樣式現在改善了在「電子郵件通知」區域中設定事件通知的體驗。

如需有關設定電子郵件通知的資訊，請參閱 [為系統中的每個人設定事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

此功能現已包含在 [電子郵件和應用程式內通知學習路徑](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) 在Workfront One上。

## 觸發事件訂閱更新的新API物件

已建立兩個新的API物件documentVersion和proofApproval，並將其設定為在檔案建立版本或核準時觸發事件訂閱更新。

如需與每個物件相關聯的完整欄位清單，請參閱 [事件訂閱資源欄位](../../../wf-api/api/event-sub-resource-fields.md).
