---
product-area: setup
navigation-topic: notifications
title: 啟用或停用您自己的事件通知
description: Adobe Workfront管理員會設定使用者在Workfront中發生事件時收到的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# 啟用或停用您自己的事件通知

您的Adobe [!DNL Workfront] 管理員會設定使用者在Workfront中發生事件時收到的事件通知(如 [[!UICONTROL 設定事件] 系統中每個人的通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md))。

您的群組管理員也可以設定要為您和家庭群組中的使用者啟動哪些事件通知。 若您的 [!UICONTROL 家庭組] 是子群組，您會收到為群組上方的頂層群組啟動的事件通知。

您可以透過設定您收到的通知來進一步自訂此項目。 您也可以選擇要在事件發生時接收通知，還是要在一封每日摘要電子郵件中接收。

如需電子郵件通知的詳細資訊，請參閱 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* 如果您啟動通知類型，然後發現您沒有收到該類型的通知，可能是因為該類型不適用於您的角色。
>* 此 [!DNL Workfront] 管理員或組管理員無法配置通知 [!DNL Workfront Goals]. 如需通知的詳細資訊，請參閱 [!DNL Workfront] 管理員可進行配置，請參閱 [為系統中的每個人配置事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). 如需設定 [!DNL Workfront Goals] 繼續閱讀本文。
>


## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 檢視及修改您的電子郵件通知設定

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下您的個人資料圖片旁的使用者名稱。

1. 按一下 **[!UICONTROL 更多]** 圖示 ![](assets/more-icon.png) ，然後按一下 **[!UICONTROL 編輯]**.

1. 在 **[!UICONTROL 編輯人員]** 框，轉到 **[!UICONTROL 通知]** 區段。

1. 按一下類別可檢視與該類別相關的通知設定。

   ![](assets/my-profile-notifications.png)

1. 選擇或取消選擇右側的複選框，以指定您是要每天接收通知，還是要立即接收通知，還是要同時接收通知。

   您也可以使用類別的核取方塊來啟用或停用該類別中的所有通知。

   >[!NOTE]
   >
   >如果您是專案的團隊成員，您會繼續收到專案的電子郵件通知，直到您從團隊中移除為止，即使您已無法存取專案亦然。 有關從團隊中刪除用戶的說明，請參閱 [從專案移除使用者](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   若 **[!UICONTROL 通訊]** 類別中，您只能選擇即時傳送的個別通知。 若要讓通知在每日摘要中傳送，您必須選取所有通知。

   如果已激活給定類別的所有電子郵件通知，則類別標題中的框將顯示為選定。 如果指定類別中的所有電子郵件通知都已停用，則會取消選取方塊。 如果某些通知已啟用，而其他通知已停用，則類別核取方塊會以直線顯示。\
   修改通知設定時，標籤 **[!UICONTROL 已編輯]** 會針對該通知設定顯示，讓您知道該通知設定已修改。

1. 如果您選取任何要以每日摘要傳送的通知，請在 **[!UICONTROL 通知]** 區段 **[!UICONTROL 之後的電子郵件每日摘要]** 功能表。

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   每日摘要包含在所選時間之前24小時符合通知標準的事件。 您會收到每種通知類型的每日摘要電子郵件。\
   每日摘要可能會在您選取的時間之後送達，具體取決於系統中排入佇列等候傳送的電子郵件數量。 列出的時間是瀏覽器設定中指定的本地時間。

1. （條件式和選用式）在預覽環境中修改電子郵件通知設定時，請啟用 **[!UICONTROL 從此測試環境接收電子郵件]** 設定以接收電子郵件。 預覽環境不會自動產生電子郵件。

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. 按一下 **[!UICONTROL 儲存變更]**.
