---
content-type: release-notes
keywords: 附註，每季，更新
navigation-topic: product-releases
title: 21.1其他增強功能
description: 本頁說明在「預覽」環境中21.1版所做的所有其他增強功能。 這些增強功能將於2021年2月15日當周在生產環境中提供。
author: Luke
feature: Product Announcements
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 21.1其他增強功能

本頁說明在「預覽」環境中21.1版所做的所有其他增強功能。 這些增強功能將於2021年2月15日當周在生產環境中提供。

如需21.1版所有可用變更的清單，請參閱 [21.1版本概觀](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 事件訂閱失敗要求的更新

我們正在更新事件訂閱失敗的軟禁用要求。 除了現有需求，如果「事件訂閱」在2000次嘗試內都未成功傳送，現在將會軟性停用。 這是為了加強現有的70%故障規則，在某些情況下，這會導致過多的故障。

此外，我們將自2021年2月起新增硬停用要求。

有關新的軟禁用和硬禁用要求的其他資訊，請參閱 [常見問題集 — 事件訂閱](../../../wf-api/general/event-subs-faq.md).

## 「每日摘要」提供的「新團隊」欄位

已將「團隊核准」和「指派」欄位新增至「需要動作的每日摘要」電子郵件。

如需詳細資訊，請參閱 [通知：需要的行動](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## 替換請求隊列中的POP電子郵件選項

我們正在將請求隊列的POP電子郵件選項替換為新的Workfront管理系統。 您仍可以透過電子郵件提交請求，但您需要在「請求佇列」區域中設定新的Adobe Workfront管理電子郵件地址。

這些變更可在預覽中測試。

所有預覽環境中都會自動停用電子郵件。 若要啟用電子郵件以用於測試用途，請參閱 [啟用從預覽沙箱環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

如需詳細資訊，請參閱 [讓使用者將問題透過電子郵件傳送至「請求佇列」專案](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

如需進行此變更的原因的詳細資訊，請參閱 [新Adobe Workfront管理系統以21.1取代請求佇列的POP電子郵件](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

此功能現已納入 [新Workfront體驗中的佇列管理](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) Workfront一號的學習路徑。

## 在工時單上限制小時編輯

為了對工時單和工時編輯提供更多控制，我們添加了一個設定，允許您限制對工時單所有者和系統管理員進行工時編輯。

以前，在訪問級別啟用了「工時單和工時」選項的用戶可以編輯任何工時單上的工時。

如需詳細資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## 改進「工時單」區域中的篩選器和視圖

在將項目、任務或問題添加到時間表時，我們添加了以下改進：

* 篩選器：我們已新增專案和問題的篩選器。 按一下「更多」選項可檢視這些篩選器。 以前，只有「任務」可用篩選。
* 檢視：已將「檢視」和「分組」選項新增至「搜尋」頁面。

如需詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 在工時單中隱藏加班框

如果您不在Workfront中追蹤加班，現在可以隱藏加班方塊以減輕使用者混淆。 您可以隱藏一次性工時單或工時單配置檔案的加班框：

* 一次性工時單：當您選擇隱藏單個工時單中的超時框時，該框僅對該工時單隱藏。 如需詳細資訊，請參閱 [建立單次使用的工時單](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* 時間表配置檔案：當您選擇隱藏「工時單配置檔案」中的超時框時，為分配給該配置檔案的用戶建立的所有將來時間表將看不到超時框。 如需詳細資訊，請參閱 [建立、編輯和分配工時單配置檔案](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

以前，您無法在工時單上隱藏超時框。

## 展開或折疊階層連結導覽中的項目

為了更輕鬆檢視完整的階層連結路徑，我們新增了展開和折疊功能。

現在，任何截斷的項目都會在專案前分組，並加上文字「更多」。 例如，「3個以上」表示有3個物件沒有顯示。

之前，您必須按一下省略號，才能在下拉式選單中顯示任何截斷的物件。

若要檢視階層連結中的所有項目，請按一下階層連結開頭的「更多」以展開項目。 展開後，您可以按一下「較少」，再次折疊項目。

## 階層連結導覽的新外觀和風格

為協助使用者更清楚地識別他們在Workfront的位置，並更輕鬆地在物件之間導覽，我們已改善階層連結導覽：

* 階層連結中的每個項目現在都包含物件標籤。
* 目前的頁面現在包含在階層連結中，且為斜體。
* 階層連結現在提供鍵盤導覽和螢幕助讀程式導覽功能。
* 其他次要樣式變更

