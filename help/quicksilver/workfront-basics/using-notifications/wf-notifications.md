---
content-type: overview;reference
navigation-topic: notifications
title: 通知總覽
description: Adobe Workfront會在您的行動裝置上傳送電子郵件通知、應用程式內通知和通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 1%

---

# 通知總覽

<!--Audited: 12/2023-->

[!DNL Adobe Workfront]會在您的行動裝置上傳送電子郵件通知、應用程式內通知和通知。

## 電子郵件通知

[!DNL Workfront]會傳送電子郵件通知以提醒使用者有關Workfront中的活動，並提供有用的資訊和連結。

若要變更電子郵件通知的偏好設定，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

>[!NOTE]
>
>如果您想要接收來自沙箱環境的電子郵件通知，您必須在該環境中啟用來自您的使用者設定檔的電子郵件。

您可以從[!DNL Workfront]收到下列電子郵件通知：

* [事件通知](#event-notifications)
* [每日摘要通知](#daily-digest-notifications)
* [已張貼評論的通知](#notification-of-posted-comments)
* [自動提醒](#automatic-reminders)
* [提醒通知](#reminder-notifications)
* [面板通知](#boards-notifications)
* [其他 [!DNL Workfront] 封電子郵件](#other-workfront-emails)

### 事件通知

事件通知通常由某些預先定義事件觸發，例如將任務指派給您，或獲得您所做評論的回覆。

在您的[!DNL Workfront]管理員或群組管理員在您的[!DNL Workfront]系統中啟動事件通知後，您可以在使用者設定檔中編輯[!UICONTROL 通知]偏好設定，以選取您想要收到的通知。 您也可以選擇要在事件發生時收到通知，還是要接收在一封每日摘要電子郵件中摘要的事件。

您可能在您的設定中只看到這些通知的子集，取決於[!DNL Workfront]管理員如何為您的[!DNL Workfront]系統設定事件通知。 如需詳細資訊，請參閱[設定系統中每個人的事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

預設狀態顯示當您建立新使用者時，新使用者預設已啟用哪些通知（每日、即時或兩者）。

如需事件通知的完整清單，以及如何在系統層級、群組層級或使用者層級啟用和設定事件通知的詳細資訊，請參閱[可在 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)中使用的事件通知。

如需有關如何選擇您要接收哪些事件通知的詳細資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

>[!NOTE]
>
>事件通知是唯一可設定為在每日摘要更新中傳送的通知。

### 每日摘要通知

每日摘要通知是一封電子郵件，其中包含您在電子郵件之前24小時內收到的特定型別的所有通知。

如需為每日摘要電子郵件傳遞啟用哪些電子郵件通知的完整清單，以及有關電子郵件通知所有類別的資訊，請參閱[事件通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications)。

>[!NOTE]
>
>[!UICONTROL Workfront]未針對[!UICONTROL 雜項]和[!DNL Goals]事件類別傳送任何每日摘要通知。 您無法停用這些類別的每日通知。

接收每日摘要通知時，請注意幾件事：

* 您的&#x200B;**[!UICONTROL 我的設定]**&#x200B;面板中的每個[!UICONTROL 通知]區段都會產生自己的每日摘要電子郵件。 您可以設定每天的每日摘要電子郵件，數量與每天摘要電子郵件啟用的通知設定數量相同。\
   例如，如果您選擇接收&#x200B;**[!UICONTROL 我擁有的專案資訊]下數個動作的每日摘要電子郵件，**，您會收到一封電子郵件通知，列出此區域符合的所有事件。

* 每日摘要電子郵件中的通知會依各種條件分組。 例如，在&#x200B;**[!UICONTROL 我擁有的專案相關資訊]**&#x200B;的情況下，事件會依專案名稱分組。

  對於&#x200B;**[!UICONTROL 通訊]**&#x200B;類別，通知會依發生通訊的物件分組。

  >[!NOTE]
  >
  >在「通訊」類別中，您可以選取僅供即時傳送的個別通知。 若要在每日摘要中傳送通知，您必須選取所有通知。

* 每日摘要電子郵件會列出在特定區域之動作（例如&#x200B;**我擁有之專案的資訊**）在選定傳送時間前24小時內發生的事件。
* 為每日摘要傳送選取的時間時區與您的時區相符，因為它是根據瀏覽器上的設定而定。
* 每日摘要電子郵件的主旨行中有區段名稱，以及傳送日期。
* 必須至少有一個事件觸發通知，才能傳遞每日摘要。 如果不符合標籤為每日摘要電子郵件的事件，則不會傳送每日摘要。

### 已張貼評論的通知

[!UICONTROL 通訊]類別中的通知會提醒您特定專案的[!UICONTROL 更新]資料流中已張貼的評論。

已針對所有可用通知選取[!UICONTROL 通訊]類別的每日摘要電子郵件。

會針對發生通訊的物件摘要資訊，並顯示每個物件的通訊訊息總數。

若要回複評論或在Workfront中檢視評論：

1. 按一下電子郵件中的&#x200B;**[!UICONTROL 註解]**&#x200B;按鈕。

   物件的[!UICONTROL 更新]區域會開啟，並以藍色框示特定註解。

   回複方塊已開啟，您可用來回覆註解。

如需有關設定電子郵件通知的詳細資訊，包括啟用每日摘要通知，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)中的[檢視並修改您的電子郵件通知設定](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings)。

### 自動提醒

您的[!DNL Workfront]管理員已啟用自動提醒，提醒您過期、延遲或接近計畫完成日期的任務和問題。 對於延遲通知，在任務或問題完成之前，每晚會傳送電子郵件。 管理員設定這些專案後，您就無法停用它們。 此外，您無法變更自動提醒所觸發之電子郵件的內容或主旨列。

此提醒可以傳送給以下其中一位或多位：

* 指派給任務或問題的使用者
* 使用者的直接管理員
* 直接管理員的管理員

自動提醒電子郵件是從您的[!DNL Workfront]管理員選取要處理外寄電子郵件的電子郵件地址傳送。

根據啟用的自動提醒而定，自動提醒電子郵件中有以下型別的資訊：

* 任務或問題的建立日期
* 任務或問題名稱
* 任務或問題所在的專案名稱
* 任務或問題的說明
* 指派給任務或問題的使用者清單
* 輸入任務或問題的使用者名稱
* 任務或問題的優先順序
* 任務或問題逾期的日期

如需啟用自動提醒的資訊，請參閱[設定自動提醒](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md)。

### 提醒通知

[!DNL Workfront]管理員（或具有[!UICONTROL 規劃師]存取層級以及提醒通知的管理存取權的使用者）可以設計有關臨近截止日期的提醒通知，並手動將其與專案、任務、問題和時程表建立關聯。

>[!IMPORTANT]
>
>如果在使用者收到上述任何物件的提醒通知後截止日期改變，使用者不會收到另一個提醒通知。

提醒通知是從[!DNL Workfront]管理員選取要處理外寄電子郵件的電子郵件地址傳送。

如需設定和啟用提醒通知的詳細資訊，請參閱[設定提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md)。

如需有關如何取得必要管理存取權的資訊，請參閱[授予使用者對特定區域的管理存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

### 面板通知

[!DNL Adobe Workfront] [!UICONTROL 展示板]會在您將您新增至展示板時，以及當卡片指派給您時，傳送電子郵件給您。 您可以選取要在展示板偏好設定中接收的電子郵件。

如需詳細資訊，請參閱[面板電子郵件通知和偏好設定](/help/quicksilver/agile/get-started-with-boards/boards-emails.md)。

### 其他[!DNL Workfront]封電子郵件

您可能會從[!DNL Workfront]收到無法設定的其他電子郵件。

當滿足下列條件時，[!DNL Workfront]會自動傳送下列電子郵件：

* 還原專案：當[!DNL Workfront]系統管理員從[!UICONTROL 資源回收]資料匣還原物件時，會傳送電子郵件給[!DNL Workfront]系統管理員。
* 無法還原：當[!DNL Workfront]管理員嘗試從資源回收筒還原物件時，還原失敗，系統會傳送電子郵件給[!DNL Workfront]管理員。

以下電子郵件只能在使用者設定檔層級設定。 無法在系統層級啟用或停用這些功能：

* 完成個人工作：當您指派給其他人的個人工作完成時，您將會收到電子郵件。
* 新增至使用者的評論：當有人對您的使用者設定檔發表評論時，您將會收到電子郵件。

## 應用程式內通知

當某些事件發生時，您可以在[!DNL Workfront]網頁應用程式內接收通知。

如需應用程式內通知的詳細資訊，請參閱[檢視及管理應用程式內通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)。

## 行動電子郵件應用程式中的電子郵件通知

您可以在行動裝置上的行動電子郵件應用程式中接收[!DNL Workfront]電子郵件通知。

如果您的手機上已安裝[!DNL Workfront]行動應用程式，點選電子郵件中的連結會在[!DNL Workfront]行動應用程式中開啟這些連結。 這包括點選下列任一動作按鈕：

* [!UICONTROL 處理它]
* [!UICONTROL 註解]
* [!UICONTROL 進行核准決定]
* [!UICONTROL 檢視所有通知]
* [!UICONTROL 新增]
* [!UICONTROL 開始使用]
* [!UICONTROL 檢視更多詳細資料]

如需[!DNL Workfront]行動應用程式的詳細資訊，請參閱[使用 [!DNL Adobe Workfront] 行動應用程式](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md)。
