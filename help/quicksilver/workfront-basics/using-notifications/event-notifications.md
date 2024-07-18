---
content-type: overview
navigation-topic: notifications
title: 事件通知
description: 事件通知是由物件上各種型別的事件所觸發的電子郵件，例如專案、任務或問題。 當專案發生其他人需要知道的情況時，就會傳送這些訊息。 視事件而定，使用者會收到即時、每日或即時和每日相關電子郵件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# 事件通知

事件通知是由物件上各種型別的事件所觸發的電子郵件，例如專案、任務或問題。 當專案發生其他人需要知道的情況時，就會傳送這些訊息。 視事件而定，使用者會收到即時、每日或即時和每日相關電子郵件通知。

>[!NOTE]
>
>事件通知是數種[!DNL Adobe Workfront]通知型別之一。 如需所有[!DNL Workfront]通知型別的相關資訊，請參閱[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

## 設定事件通知

事件通知電子郵件可在下列層級進行設定。 事件通知的設定包含啟用或停用。

* **系統層級**： [!DNL Workfront]系統管理員可以在系統層級啟用和停用事件通知，如[設定系統內每個人的事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)中所述。

  依預設，所有群組都會繼承系統通知，但如果[!DNL Workfront]管理員允許，群組管理員可以變更群組層級上的某些設定，如下面的下一個專案符號專案所述。

* **群組層級**：群組管理員可以在[!DNL Workfront]管理員為群組解除鎖定此功能後，為其管理的群組設定事件通知。 如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 [!DNL Workfront]管理員也是如此（適用於任何群組）。 如需詳細資訊，請參閱[檢視並設定群組](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。

  >[!NOTE]
  >
  >這項功能最初僅供叢集4上的客戶使用，屬於分階段推出的一部分。 不久後，其他叢集即可使用該功能。 當這種情況發生時，本文將會更新。

* **使用者層級**：所有在整個系統內啟用的事件通知，都會列在每個使用者個別設定檔的[!UICONTROL 通知]區段中。 使用者可以在那裡啟用和停用他們的個人事件通知。

  [!DNL Workfront]管理員和具有編輯其他使用者存取權的使用者也可以在個別使用者的設定檔中啟用和停用通知。

  如需詳細資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

  >[!NOTE]
  >
  >使用者層級通知也包含[!DNL Workfront Goals]個通知。 但是，[!DNL Workfront]管理員或群組管理員無法設定[!DNL Workfront Goals]的通知。 每個使用者都必須在他們的設定檔中設定自己的[!DNL Workfront Goals]通知。 如果您有編輯使用者的許可權，也可以為其他人修改這些通知。 若要為您設定檔或您有權編輯的其他使用者啟用[!DNL Workfront Goals]通知，請參閱[通知：目標](../../workfront-basics/using-notifications/notifications-goals.md)。

  如需[!DNL Workfront]管理員可以設定哪些通知的詳細資訊，請參閱[為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。 [!DNL Workfront Goals]僅在新的[!DNL Adobe Workfront]體驗中可用。

## 事件通知內容

事件通知電子郵件包含所發生事件的相關資訊，且包含[!DNL Workfront]的連結，您可以在其中看到系統中的事件。 如需接收電子郵件通知的詳細資訊，請參閱[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

[!DNL Workfront]管理員無法變更電子郵件通知的內容，因為它們是由[!DNL Workfront]所設定。 但是，他們可以變更事件通知電子郵件的主旨行。 如需詳細資訊，請參閱[自訂事件通知的電子郵件主題](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md)。

如需所有[!DNL Workfront]個事件通知的清單，以及每個事件的簡短說明，以及預設為使用中或非使用中，請參閱 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)中可用的[事件通知。
