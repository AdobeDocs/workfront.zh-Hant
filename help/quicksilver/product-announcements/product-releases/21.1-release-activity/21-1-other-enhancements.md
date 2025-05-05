---
content-type: release-notes
keywords: 備註，每季，更新
navigation-topic: product-releases
title: 21.1其他增強功能
description: 本頁說明21.1版對預覽環境所做的所有其他增強功能。 這些增強功能將在2021年2月15日當週的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1其他增強功能

本頁說明21.1版對預覽環境所做的所有其他增強功能。 這些增強功能將在2021年2月15日當週的生產環境中提供。

如需21.1版本可用的所有變更清單，請參閱[21.1版本概觀](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)。

## 更新事件訂閱失敗要求

我們正在更新事件訂閱失敗的可變停用需求。 除了現有需求，如果事件訂閱在2000次嘗試內無法成功傳遞，現在將軟性停用。 這是為了強化現有的70%失敗規則，在某些情況下，這可能會導致過多的失敗。

此外，我們將在2021年2月起新增硬停用需求。

如需新的軟式停用與硬式停用需求的詳細資訊，請參閱[常見問題集 — 事件訂閱](../../../wf-api/general/event-subs-faq.md)。

## 「每日摘要」可用的新團隊欄位

我們已將團隊核准和指派欄位新增到「需要動作的每日摘要」電子郵件。

如需詳細資訊，請參閱[通知：需要動作](../../../workfront-basics/using-notifications/notifications-action-needed.md)。

## 取代請求佇列中的POP電子郵件選項

我們正在將請求佇列的POP電子郵件選項取代為新的Workfront管理系統。 您仍可以透過電子郵件提交請求，但您需要在「請求佇列」區域中設定新的Adobe Workfront管理電子郵件地址。

這些變更可在「預覽」中測試。

電子郵件在所有預覽環境中都會自動停用。 若要啟用電子郵件以進行測試，請參閱[啟用來自預覽沙箱環境的電子郵件傳遞](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

如需詳細資訊，請參閱[讓使用者透過電子郵件將問題傳送到請求佇列專案](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md)。

如需我們為何進行此變更的詳細資訊，請參閱[新的Adobe Workfront受管系統，以21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md)取代請求佇列的POP電子郵件。

此功能現已包含在Workfront One上新Workfront體驗[&#128279;](https://experienceleague.adobe.com/zh-hant/docs/workfront-learn/tutorials-workfront/home)學習路徑的佇列管理中。

## 限制時程表上的小時編輯

為了提供對時程表和小時編輯的更多控制權，我們新增了設定，可讓您限制對時程表所有者和系統管理員進行小時編輯。

以前，在存取層級中啟用時程表和時數選項的使用者可以在任何時程表中編輯時數。

如需詳細資訊，請參閱[設定時程表和小時喜好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

## 改進時程表區域中的篩選器和檢視

當您新增專案、任務或問題至時程表時，我們已新增下列改善專案：

* 篩選器：我們已新增專案和問題的篩選器。 按一下「更多選項」以檢視這些篩選器。 以前，只有任務可使用篩選。
* 檢視：我們已將「檢視」和「群組」選項新增至「搜尋」頁面。

如需詳細資訊，請參閱[記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md)。

## 隱藏時程表中超時方塊

如果您沒有在Workfront中追蹤加班，現在可以隱藏加班方塊，以方便使用者混淆。 您可以隱藏單次使用時程表或時程表設定檔中的加班方塊：

* 單次使用時程表：當您選擇隱藏個別時程表中的加時方塊時，該時程表才會隱藏。 如需詳細資訊，請參閱[建立單次使用時程表](../../../timesheets/create-and-manage-timesheets/create-tmshts.md)。
* 時程表設定檔：當您選擇隱藏時程表設定檔中的超時方塊時，所有針對指派給該設定檔的使用者而建立的時程表都不會看到超時方塊。 如需詳細資訊，請參閱[建立、編輯和指派週期性時程表](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

以前您無法隱藏時程表上的加時方塊。

## 展開或摺疊階層連結導覽中的專案

為了讓您更輕鬆地檢視完整階層連結路徑，我們新增了展開和摺疊功能。

現在，任何截斷的專案會在含有「更多」文字的專案之前分組。 例如，「另外3個」表示有3個物件未顯示。

之前，您必須按一下省略符號，才能在下拉式選單中顯示任何截斷的物件。

若要檢視階層連結中的所有專案，請按一下階層連結開頭的「更多」以展開專案。 展開後，您可以按一下「較少」以再次收合專案。

## 階層連結導覽的新外觀

為協助使用者更能識別他們在Workfront中的位置，以及更輕鬆地在物件之間導覽，我們對階層連結導覽進行下列改進：

* 階層連結中的每個專案現在都包含物件標籤。
* 目前頁面現在包含在階層連結中，並以斜體顯示。
* 階層連結現在可使用鍵盤導覽和熒幕助讀程式導覽。
* 其他次要樣式變更

