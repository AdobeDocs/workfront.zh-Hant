---
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront通知
description: Adobe Workfront會在您的行動裝置上傳送電子郵件通知、應用程式內通知和通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 1%

---

# [!DNL Adobe Workfront] 通知

[!DNL Adobe Workfront] 會在您的行動裝置上傳送電子郵件通知、應用程式內通知和通知。

## 電子郵件通知

[!DNL Workfront] 會傳送許多電子郵件通知，以提醒使用者有關Workfront中的活動，並提供有用的資訊和連結。

若要變更電子郵件通知的偏好設定，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>如果您想要接收來自沙箱環境的電子郵件通知，您必須在該環境中啟用來自您的使用者設定檔的電子郵件。

您可以收到以下電子郵件通知，來自 [!DNL Workfront]：

* [事件通知](#event-notifications)
* [每日摘要通知](#daily-digest-notifications)
* [已張貼評論的通知](#notification-of-posted-comments)
* [自動提醒](#automatic-reminders)
* [提醒通知](#reminder-notifications)
* [面板通知](#boards-notifications)
* [其他 [!DNL Workfront] 電子郵件](#other-workfront-emails)

### 事件通知

事件通知預先定義於 [!DNL Workfront]. 它們通常由特定事件觸發。

在您的啟動事件通知後 [!DNL Workfront] 管理員或群組管理員，您可以透過編輯您的檔案來選擇要接收哪些收件者 [!UICONTROL 通知] 您的使用者設定檔中的偏好設定。 您也可以選擇要在事件發生時收到通知，還是要接收在一封每日摘要電子郵件中摘要的事件。

取決於 [!DNL Workfront] 管理員已為您的設定事件通知 [!DNL Workfront] 系統（如所述） [為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))，則您可能在設定中只看到這些通知的子集。

預設狀態顯示當您建立新使用者時，新使用者預設已啟用哪些通知（每日、即時或兩者）。

如需事件通知的完整清單，以及如何在系統層級、群組層級或使用者層級啟用和設定這些通知的相關資訊，請參閱 [事件通知位於 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

如需如何選擇要接收之事件通知的詳細資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>事件通知是唯一可設定為在每日摘要更新中傳送的通知。

### 每日摘要通知

如需為每日摘要電子郵件傳送啟用哪些電子郵件通知的完整清單，以及有關電子郵件通知所有類別的資訊，請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] 不會針對以下專案傳送任何每日摘要通知 [!UICONTROL 其他] 和 [!DNL Goals] 事件類別。 您無法停用這些類別的每日通知。

接收每日摘要通知時，請注意幾件事：

* 每個 [!UICONTROL 通知] 區段 **[!UICONTROL 我的設定]** 面板會產生自己的每日摘要電子郵件。 您可以設定每天的每日摘要電子郵件，數量與每天摘要電子郵件啟用的通知設定數量相同。\
   例如，如果您選取接收底下數個動作的每日摘要電子郵件 **[!UICONTROL 專案一的相關資訊] 擁有，** 您會收到一封電子郵件通知，列出此區域符合的所有事件。

* 每日摘要電子郵件中的通知會依各種條件分組。 例如，若為 **[!UICONTROL 關於我擁有的專案資訊]**，則事件會依專案名稱分組。

  對於 **[!UICONTROL 通訊]** 類別中，通知會依發生通訊的物件分組。

* 每日摘要電子郵件會列出某個特定區域(例如 **關於我擁有的專案資訊**)在選取的傳送時間前24小時內。
* 為每日摘要傳送選取的時間時區與您的時區相符，因為它是根據瀏覽器上的設定而定。
* 每日摘要電子郵件的主旨行中有區段名稱，以及傳送日期。
* 必須至少有一個事件觸發通知，才能傳遞每日摘要。 如果不符合標籤為每日摘要電子郵件的事件，則不會傳送每日摘要。

### 已張貼評論的通知

中的通知 [!UICONTROL 通訊] 類別警示您已在下列欄位中張貼的評論： [!UICONTROL 更新] 特定專案的資料流。

的每日摘要電子郵件 [!UICONTROL 通訊] 已針對所有可用通知選取類別。

會針對發生通訊的物件摘要資訊，並顯示每個物件的通訊訊息總數。

如需設定電子郵件通知的詳細資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有關註解的指示 [!UICONTROL 通訊] 電子郵件，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

若要深入瞭解 [!UICONTROL 通訊] 電子郵件，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

如需啟用每日摘要通知的詳細資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 自動提醒

自動提醒功能由您的啟用 [!DNL Workfront] 管理員警示您到期、延遲或接近計畫完成日期的任務和問題。 對於延遲通知，在任務或問題完成之前，每晚會傳送電子郵件。 管理員設定這些專案後，您就無法停用它們。 此外，您無法變更自動提醒所觸發之電子郵件的內容或主旨列。

它們可以傳送到以下一個或多個專案：

* 指派給任務或問題的使用者
* 使用者的直接管理員
* 直接管理員的管理員

自動提醒電子郵件會從您設定的電子郵件地址 [!DNL Workfront] 已選取管理員來處理外寄電子郵件。

根據啟用的自動提醒而定，自動提醒電子郵件中有以下型別的資訊：

* 任務或問題的建立日期
* 任務或問題名稱
* 任務或問題所在的專案名稱
* 任務或問題的說明
* 指派給任務或問題的使用者清單
* 輸入任務或問題的使用者名稱
* 任務或問題的優先順序
* 任務或問題逾期的日期

如需啟用自動提醒的詳細資訊，請參閱 [設定自動提醒](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### 提醒通知

A [!DNL Workfront] 管理員(或具有 [!UICONTROL 計畫者] 存取層級和管理提醒通知的存取權)可以設計有關臨近截止時間的提醒通知，並將其附加到專案、任務、問題和時間表。 如需有關如何取得所需管理存取許可權的詳細資訊，請參閱 [授予使用者管理特定區域的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>如果在使用者收到上述任何物件的提醒通知後截止日期改變，使用者不會收到另一個提醒通知。

提醒通知是從以下位置的電子郵件地址傳送： [!DNL Workfront] 已選取管理員來處理外寄電子郵件。

如需設定和啟用提醒通知的詳細資訊，請參閱 [設定提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### 面板通知

[!DNL Adobe Workfront] [!UICONTROL 展示板] 會在您將您新增至展示板以及將卡片指派給您時傳送電子郵件給您。

您可以選取要在展示板偏好設定中接收的電子郵件。 如需詳細資訊，請參閱 [面板電子郵件通知和偏好設定](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### 其他 [!DNL Workfront] 電子郵件

您可能會收到其他電子郵件 [!DNL Workfront] 無法設定的。 以下電子郵件是由自動傳送 [!DNL Workfront] 當滿足下列條件時：

* 還原專案：當 [!DNL Workfront] 管理員從還原物件 [!UICONTROL 回收] 在收件匣中，會傳送電子郵件至 [!DNL Workfront] 管理員。
* 無法還原：當 [!DNL Workfront] 管理員嘗試從資源回收筒還原物件，還原失敗時，會傳送電子郵件至 [!DNL Workfront] 管理員。

以下電子郵件只能在使用者設定檔層級設定。 無法在系統層級啟用或停用這些功能：

* 完成個人工作：當您指派給其他人的個人工作完成時，您將會收到電子郵件。
* 新增至使用者的評論：當有人對您的使用者設定檔發表評論時，您將會收到電子郵件。

## 應用程式內通知

您可以在內接收通知 [!DNL Workfront] 網頁應用程式（當特定事件發生時）。

如需應用程式內通知的詳細資訊，請參閱 [檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 行動電子郵件應用程式中的電子郵件通知

您可以 [!DNL Workfront] 行動裝置上行動電子郵件應用程式中的電子郵件通知。

如果您擁有 [!DNL Workfront] 安裝在您手機上的行動應用程式，點選電子郵件中的連結會在以下位置開啟它們： [!DNL Workfront] 行動應用程式。 這包括點選下列任一動作按鈕：

* [!UICONTROL 處理它]
* [!UICONTROL 評論]
* [!UICONTROL 進行核准決策]
* [!UICONTROL 查看所有通知]
* [!UICONTROL 新增]
* [!UICONTROL 開始使用]
* [!UICONTROL 查看更多詳細資料]

如需關於的詳細資訊 [!DNL Workfront] 行動應用程式，請參閱 [使用 [!DNL Adobe Workfront] 行動應用程式](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
