---
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront通知
description: Adobe Workfront會在您的行動裝置上傳送電子郵件通知、應用程式內通知和通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: bfe45a29290631420c3a60d7dcbe470619094ca1
workflow-type: tm+mt
source-wordcount: '1301'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 通知

[!DNL Adobe Workfront] 在您的行動裝置上傳送電子郵件通知、應用程式內通知和通知。

## 電子郵件通知

[!DNL Workfront] 傳送數封電子郵件通知，以提醒使用者Workfront中的活動，並提供實用的資訊和連結。

>[!NOTE]
>
>如果您想要從沙箱環境接收電子郵件通知，您必須啟用該環境中使用者設定檔的電子郵件。

您可以從以下電子郵件接收通知 [!DNL Workfront]:

* [事件通知](#event-notifications)
* [每日摘要通知](#daily-digest-notifications)
* [已張貼留言的通知](#notification-of-posted-comments)
* [自動提醒](#automatic-reminders)
* [提醒通知](#reminder-notifications)
* [展示板通知](#boards-notifications)
* [其他 [!DNL Workfront] 電子郵件](#other-workfront-emails)

### 事件通知

事件通知預先定義於 [!DNL Workfront]. 這通常是由特定事件觸發。

事件通知啟動後 [!DNL Workfront] 管理員或群組管理員，您可以編輯 [!UICONTROL 通知] 偏好設定。 您也可以選擇是要在事件發生時接收通知，還是要接收匯總於每日摘要式電子郵件中的事件。

視 [!DNL Workfront] 管理員已為您的 [!DNL Workfront] 系統(如 [為系統中的每個人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))，則您可能只會在設定中看到這些通知的子集。

預設狀態會顯示當您建立新使用者時，新使用者預設會啟用哪些通知（每日、即時或兩者）。

有關事件通知的完整清單，以及在系統級別、組級別或用戶級別上如何啟用和配置事件通知的資訊，請參閱 [中可用的事件通知 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

有關如何選擇要接收的事件通知的資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>事件通知是唯一可設定為在每日摘要更新中傳送的通知。

### 每日摘要通知

如需每日摘要式電子郵件傳送所啟用之電子郵件通知的完整清單，以及電子郵件通知所有類別的相關資訊，請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] 不會針對 [!UICONTROL 其他] 和 [!DNL Goals] 事件的類別。 您無法停用這些類別的每日通知。

收到每日摘要通知時，需注意以下幾項事項：

* 每個 [!UICONTROL 通知] 區段 **[!UICONTROL 我的設定]** 面板會產生自己的每日摘要電子郵件。 您每天可以有最多的每日摘要電子郵件，以及為每日摘要電子郵件啟用的通知設定。\
   例如，如果您針對以下幾個動作選取接收每日摘要電子郵件， **[!UICONTROL 關於項目I的資訊] 擁有，** 您會收到一封電子郵件通知，列出此區域符合的所有事件。

* 每日摘要電子郵件中的通知會依各種條件分組。 例如，在 **[!UICONTROL 我擁有的專案的相關資訊]**，則會依專案名稱對事件分組。

   若 **[!UICONTROL 通訊]** 類別中，通知會依發生通訊的物件分組。

* 每日摘要電子郵件會列出針對特定區域(如 **我擁有的專案的相關資訊**)。
* 為每日摘要傳送選取的時區會符合您的時區，如瀏覽器所設定。
* 每日摘要電子郵件的主旨行中會包含區段的名稱，以及傳送日期。
* 至少一個事件必須觸發通知，才能傳送每日摘要。 如果未符合標示為每日摘要電子郵件的事件，則不會傳送每日摘要。

### 已張貼留言的通知

中的通知 [!UICONTROL 通訊] 類別會提醒您注意已張貼在 [!UICONTROL 更新] 特定項目的資料流。

的每日摘要電子郵件 [!UICONTROL 通訊] 會針對所有可用通知選取類別。

該資訊被匯總為發生通信的對象，並且每個對象顯示通信消息的總數。

如需設定電子郵件通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有關注釋的說明 [!UICONTROL 通訊] 電子郵件，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

若要深入了解 [!UICONTROL 通訊] 電子郵件，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

如需啟用每日摘要通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 自動提醒

自動提醒由 [!DNL Workfront] 管理員可提醒您在計畫完成日期之前、延遲或接近完成日期的任務和問題。 若是延遲通知，則會在每晚傳送電子郵件，直到任務或問題完成為止。 管理員配置這些後，就無法禁用它們。 此外，您無法變更自動提醒所觸發之電子郵件的內容或主旨行。

它們可傳送至下列一或多個項目：

* 指派給任務或問題的使用者
* 使用者的直接經理
* 直接經理的經理

自動提醒電子郵件會從您 [!DNL Workfront] 已選擇處理傳出電子郵件的管理員。

根據啟動的自動提醒，自動提醒電子郵件中提供以下類型的資訊：

* 建立任務或問題的日期
* 任務或問題名稱
* 任務或問題所在的項目的名稱
* 任務或問題的說明
* 指派給任務或問題的用戶清單
* 輸入任務或問題的用戶的名稱
* 任務或問題的優先順序
* 任務或問題逾期的日期

有關啟用自動提醒的資訊，請參閱 [設定自動提醒](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### 提醒通知

A [!DNL Workfront] 管理員(或 [!UICONTROL 計畫員] 訪問級別和對提醒通知的管理訪問)可以設計關於接近截止日期的提醒通知，並將它們附加到項目、任務、問題和時間表。 如需如何取得必要管理存取權限的詳細資訊，請參閱 [授予用戶對特定區域的管理訪問權限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>如果在用戶收到上述任何對象的提醒通知後，截止日期變更，則用戶不會收到其他提醒通知。

提醒通知會從以下電子郵件地址發送： [!DNL Workfront] 已選擇處理傳出電子郵件的管理員。

有關設定和啟用提醒通知的資訊，請參閱 [設定提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### 展示板通知

[!DNL Adobe Workfront] [!UICONTROL 展示板] 當您新增至展示板，以及指派資訊卡給您時，會傳送電子郵件給您。

您可以在「展示板」偏好設定中選取要接收的電子郵件。 如需詳細資訊，請參閱 [展示板電子郵件通知和偏好設定](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### 其他 [!DNL Workfront] 電子郵件

您可能會收到其他電子郵件 [!DNL Workfront] 無法設定。 下列電子郵件會由 [!DNL Workfront] 當符合下列條件時：

* 還原項目：當 [!DNL Workfront] 管理員從 [!UICONTROL 回收] Bin，系統會傳送電子郵件至 [!DNL Workfront] 管理員。
* 無法還原：當 [!DNL Workfront] 管理員嘗試從資源回收筒還原對象，但還原失敗，則會向 [!DNL Workfront] 管理員。

下列電子郵件只能在使用者設定檔層級設定。 無法在系統級別啟用或禁用它們：

* 完成個人任務：當您指派給其他人的個人任務完成時，您會收到電子郵件。
* 添加給用戶的注釋：當有人對您的使用者設定檔提出意見時，您會收到電子郵件。

## 應用程式內通知

您可以在 [!DNL Workfront] Web應用程式中，當某些事件發生時。

如需應用程式內通知的詳細資訊，請參閱 [檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 行動電子郵件應用程式中的電子郵件通知

您可以收到 [!DNL Workfront] 行動電子郵件應用程式中的電子郵件通知。

如果您有 [!DNL Workfront] 行動應用程式（安裝在您的手機上），點選電子郵件中的連結就會在 [!DNL Workfront] 行動應用程式。 這包括點選下列任一動作按鈕：

* [!UICONTROL 處理它]
* [!UICONTROL 評論]
* [!UICONTROL 進行核准決策]
* [!UICONTROL 查看所有通知]
* [!UICONTROL 新增]
* [!UICONTROL 開始使用]
* [!UICONTROL 查看更多詳細資料]

如需 [!DNL Workfront] 行動應用程式，請參閱 [使用 [!DNL Adobe Workfront] 行動應用程式](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
