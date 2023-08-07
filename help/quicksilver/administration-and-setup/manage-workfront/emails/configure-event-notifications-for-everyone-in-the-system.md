---
title: 為系統中的每個人設定事件通知
description: 事件發生時，事件通知會觸發電子郵件傳送給使用者。 作為Adobe Workfront管理員或具有供需規劃員存取層級的使用者，您可以為系統中的所有使用者設定事件通知。 事件通知的設定包含啟用或停用。
author: Caroline, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 3d4ba0396c5a59b1109ec70a6e85b77d0d093bf5
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 為系統中的每個人設定事件通知

<!--look for the "hidden" addition below for the tab redesign - August 2023-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

事件發生時，事件通知會觸發電子郵件傳送給使用者。 作為Adobe Workfront管理員或具有供需規劃員存取層級的使用者，您可以為系統中的所有使用者設定事件通知。 事件通知的設定包含啟用或停用。

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

根據您啟用的事件以及使用者在自己的設定檔上持續啟用的情況，使用者會在事件發生時收到即時、每日或即時和每日電子郵件通知。

您必須先在Workfront執行個體的「設定」區域中指定要讓所有使用者收到的通知。 在設定區域中啟動通知後，其設定檔頁面中會顯示為每個使用者設為已啟動。

在「設定」區域中啟用通知且通知顯示在使用者的設定檔頁面後，個別使用者或具有Plan授權的其他使用者也可以在使用者設定檔中設定啟用的通知，以控制特定使用者收到哪些通知以及通知的頻率。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

如需您可以啟用和停用之所有事件通知的清單，請參閱 [Adobe Workfront中可用的事件通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

如需有關解除鎖定事件通知以便群組管理員可以為其群組設定該通知的資訊，請參閱 [解鎖或鎖定所有群組的事件通知設定](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) 和 [檢視和設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>計畫者或以上，具有提醒通知的管理存取權</p> <p>有關授予「計畫」使用者管理存取權的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 為所有使用者設定事件通知

您必須先在Workfront的設定區域中啟用通知，使用者才能在其設定檔中啟用或停用通知。

>[!TIP]
>
>您無法從設定區域啟動Workfront目標的通知。 使用者只能在其設定檔中啟動這些通知。 擁有Plan授權的使用者可以為其他使用者啟用這些授權。 如需為使用者啟用Workfront目標通知的相關資訊，請參閱 [通知：目標](../../../workfront-basics/using-notifications/notifications-goals.md).

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **電子郵件** > **通知**.

   <!--hidden shot for the tab redesign - make live in August 2023:
   ![](assets/notifications-area-under-setup-emails.png)
   -->

1. 確定 **事件通知** 標籤已開啟。
1. 按一下事件名稱左側的開關，以開啟或關閉事件。

   若要檢視事件的預設通知狀態，請參閱 [事件通知](../../../workfront-basics/using-notifications/event-notifications.md).

1. （選用）按一下事件通知的名稱，以自訂電子郵件通知的主旨行。

   如需自訂電子郵件通知主旨行的詳細資訊，請參閱 [自訂事件通知的電子郵件主題](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. （可選）如果您想要解除鎖定電子郵件通知的設定，讓群組管理員可以為其群組個別進行設定，請按一下按鈕 ![](assets/lock-toggle-button.png) 在通知的右側，將其切換至解除鎖定的位置 ![](assets/unlock-toggle-button.png).

   >[!NOTE]
   >
   >這項功能最初僅供叢集4上的客戶使用，屬於分階段推出的一部分。 不久後，其他叢集即可使用該功能。 當這種情況發生時，本文將會更新。

   如需詳細資訊，請參閱 [解鎖或鎖定所有群組的事件通知設定](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).
