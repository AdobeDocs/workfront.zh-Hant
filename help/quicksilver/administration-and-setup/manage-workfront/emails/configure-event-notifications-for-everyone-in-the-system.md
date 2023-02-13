---
title: 為系統中的每個人配置事件通知
description: 事件通知會在發生特定事件時觸發傳送給使用者的電子郵件。 身為Adobe Workfront管理員或具有計畫員存取層級的使用者，您可以為系統中的所有使用者設定事件通知。 事件通知的設定包括啟用或停用。
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 為系統中的每個人配置事件通知

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

事件通知會在發生特定事件時觸發傳送給使用者的電子郵件。 身為Adobe Workfront管理員或具有計畫員存取層級的使用者，您可以為系統中的所有使用者設定事件通知。 事件通知的設定包括啟用或停用。

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

根據您啟用的事件，以及使用者在自己的設定檔上保持啟用狀態，當發生事件時，使用者會收到即時、每日或即時和每日電子郵件通知。

您必須先在Workfront例項的「設定」區域中，指定要讓所有使用者收到哪些通知。 在「設定」區域中啟動通知後，通知會針對其設定檔頁面中的每位使用者顯示為已啟動。

在「設定」區域中激活通知，並且通知出現在用戶的配置檔案頁面中後，具有計畫許可證的個人用戶或其他用戶也可以在用戶配置檔案中配置激活的通知，以控制特定用戶接收哪些通知以及接收的頻率。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

如需您可啟用和停用的所有事件通知清單，請參閱 [Adobe Workfront中提供的事件通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

如需解除鎖定事件通知以便群組管理員為其群組進行設定的相關資訊，請參閱 [解鎖或鎖定所有組的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) 和 [檢視及設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>計畫員或更高版本，具有提醒通知的管理訪問權限</p> <p>有關授予計畫用戶管理訪問權限的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 配置所有用戶的事件通知

您必須先在Workfront的「設定」區域中啟用通知，使用者才能在其設定檔中啟用或停用通知。

>[!TIP]
>
>您無法從「設定」區域啟用Workfront目標的通知。 使用者只能在其設定檔中啟用這些通知。 擁有計畫許可證的用戶可以為其他用戶激活它們。 如需為使用者啟用Workfront目標通知的相關資訊，請參閱 [通知：目標](../../../workfront-basics/using-notifications/notifications-goals.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **電子郵件** > **通知**.

1. 請確定 **事件通知** 標籤。
1. 按一下事件名稱左側的開關以開啟或關閉它。

   若要查看事件的預設通知狀態，請參閱 [事件通知](../../../workfront-basics/using-notifications/event-notifications.md).

1. （選用）按一下事件通知的名稱，以自訂電子郵件通知的主旨行。

   如需自訂電子郵件通知主旨行的詳細資訊，請參閱 [自訂事件通知的電子郵件主題](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. （選用）如果您想要解除鎖定電子郵件通知的設定，讓群組管理員可以為其群組個別設定，請按一下按鈕 ![](assets/lock-toggle-button.png) 到通知的右側，將其切換到解鎖位置 ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >此功能最初只適用於叢集4的客戶，作為分階段轉出的一部分。 此後不久，它將可供其他集群使用。 此文章會隨此情況而更新。

   如需詳細資訊，請參閱 [解鎖或鎖定所有組的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
