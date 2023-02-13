---
title: 20.4其他增強功能
description: 20.4其他增強功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 20.4其他增強功能

本頁面說明在「預覽」環境中20.4版所做的所有其他增強功能。 這些增強功能將於2020年11月9日當周在生產環境中提供。

如需20.4版所有可用變更的清單，請參閱 [20.4版本概觀](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 管理員新功能：可使用切換Workfront環境選項

為獲得更有效率且更方便的體驗，群組管理員和Workfront管理員現在可以在Workfront中任何頁面的不同Workfront環境之間快速切換，而無須登出。

在新的Workfront體驗中，主功能表中會顯示「切換至傳統版」選項。

在Workfront Classic中，按一下全域導覽列右上角的設定檔圖片時，功能表中會顯示「切換至新體驗」選項。

此功能現已納入 [管理員基礎知識，第1部分學習路徑](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront一號。

## 改善Workfront Proof的加密

我們正在進行一些變更，以提升Workfront校對應用程式的動態資料加密強度。 弱TLS加密將於2020年11月11日淘汰。

存取Workfront時，請確定您使用的是支援的瀏覽器。 如需支援瀏覽器的詳細資訊，請參閱 [Adobe Workfront瀏覽器需求](../../../workfront-basics/workfront-browser-requirements.md).

## 3個電子郵件範本的全新外觀

為了改善可讀性和整體體驗，下列電子郵件範本有新的外觀和風格：

* 新的工作請求
* 您被分配的從屬任務現在已準備好開始
* 完成前置任務的團隊電子郵件通知

若要在您的「預覽」環境中啟用電子郵件以用於測試用途，請參閱在預覽中管理電子郵件區段，位於 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 適用於團隊的新電子郵件通知

我們已為團隊新增下列電子郵件通知：

* 已完成分配給我團隊的任務的前身：當其任務的前身標籤為完成時，被指派的團隊會收到電子郵件通知。
* 已完成分配給我團隊的任務的所有前置任務：被指派的團隊會收到每個被標示為完成的前任的電子郵件通知。

如需詳細資訊，請參閱 [通知：關於分配給我的工作的資訊](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## 管理員新增功能：電子郵件通知增強功能

現在，只要按一下，您就可以在「設定」中啟用或停用事件電子郵件通知。 只需按一下通知名稱旁的開/關開關即可。

此外，請注意我們的現代樣式，現在可改善「電子郵件通知」區域中設定事件通知的體驗。

如需設定電子郵件通知的詳細資訊，請參閱 [為系統中的每個人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

此功能現已納入 [電子郵件和應用程式內通知學習路徑](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) Workfront一號。

## 觸發事件訂閱更新的新API物件

已建立兩個新的API物件documentVersion和proofApproval，且已設定為在檔案版本控制或核準時觸發事件訂閱更新。

有關與每個對象關聯的欄位的完整清單，請參見 [事件訂閱資源欄位](../../../wf-api/api/event-sub-resource-fields.md).
