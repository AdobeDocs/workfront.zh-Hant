---
content-type: overview
navigation-topic: notifications
title: 事件通知
description: 事件通知是由物件上各種類型的事件（例如專案、工作或問題）所觸發的電子郵件。 當專案中發生其他人需要了解的情況時，就會傳送這些訊息。 根據事件，使用者會收到即時、每日或即時和每日電子郵件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 事件通知

事件通知是由物件上各種類型的事件（例如專案、工作或問題）所觸發的電子郵件。 當專案中發生其他人需要了解的情況時，就會傳送這些訊息。 根據事件，使用者會收到即時、每日或即時和每日電子郵件通知。

>[!NOTE]
>
>事件通知是以下幾種類型之一 [!DNL Adobe Workfront] 通知。 關於所有 [!DNL Workfront] 通知類型，請參閱 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 設定事件通知

事件通知電子郵件可依下列層級設定。 事件通知的設定包括啟用或停用。

* **系統級別**:A [!DNL Workfront] 管理員可以在系統層級啟用和停用事件通知，如 [為系統中的每個人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   所有組預設會繼承系統通知，但組管理員可能可以更改組級別上的某些配置（如果允許） [!DNL Workfront] 管理員，如下方下一個項目中所述。

* **群組層級**:群組管理員可以在 [!DNL Workfront] 管理員解除鎖定群組的此功能。 如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 對於 [!DNL Workfront] 管理員（適用於任何群組）。 如需詳細資訊，請參閱 [檢視及設定群組的事件通知](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

   >[!NOTE]
   >
   >此功能最初只適用於叢集4的客戶，作為分階段轉出的一部分。 此後不久，它將可供其他集群使用。 此文章會隨此情況而更新。

* **使用者層級**:所有在系統範圍內激活的事件通知都列在每個用戶的 [!UICONTROL 通知] 區段。 使用者可以在那裡啟用和停用其個別事件通知。

   [!DNL Workfront] 具有編輯其他使用者存取權的管理員和使用者，也可以在個別使用者的設定檔中啟用和停用通知。

   如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >使用者層級通知也包含 [!DNL Workfront Goals] 通知。 不過， [!DNL Workfront] 管理員或組管理員無法配置通知 [!DNL Workfront Goals]. 每個使用都必須自行設定 [!DNL Workfront Goals] 通知。 如果您有編輯使用者的存取權，您也可以修改其他使用者的這些通知。 啟用 [!DNL Workfront Goals] 若要了解您的設定檔或您有權編輯的其他使用者的通知，請參閱 [通知：目標](../../workfront-basics/using-notifications/notifications-goals.md).

   如需通知的詳細資訊，請參閱 [!DNL Workfront] 管理員可進行配置，請參閱 [為系統中的每個人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] 僅在新 [!DNL Adobe Workfront] 體驗。

## 事件通知內容

事件通知電子郵件包含所發生事件的相關資訊，並包含的連結 [!DNL Workfront] 您可在此處查看系統中的事件。 如需接收電子郵件通知的詳細資訊，請參閱 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] 管理員無法更改電子郵件通知的內容，因為這些通知由 [!DNL Workfront]. 不過，他們可以變更事件通知電子郵件的主旨行。 如需詳細資訊，請參閱 [自訂事件通知的電子郵件主題](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

若要查看 [!DNL Workfront] 事件通知，以及每個事件的簡短說明，以及預設為使用中或非使用中的事件，請參閱 [中可用的事件通知 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
