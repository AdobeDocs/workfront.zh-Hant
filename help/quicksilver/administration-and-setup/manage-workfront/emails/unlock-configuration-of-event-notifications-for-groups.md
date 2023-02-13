---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 解鎖或鎖定所有組的事件通知配置
description: 如果您是Adobe Workfront管理員，您可以解除鎖定或重新鎖定群組管理員為其管理的頂層群組設定事件通知的能力。 事件通知的設定包括啟用或停用。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 解鎖或鎖定所有組的事件通知配置

如果您是Adobe Workfront管理員，您可以解除鎖定或重新鎖定群組管理員為其管理的頂層群組設定事件通知的能力。 事件通知的設定包括啟用或停用。

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

管理員為組配置事件通知時，該配置將影響該組或其子組中的一個為其「主組」的用戶。 這些使用者在其使用者設定檔中會看到為其首頁群組啟動的事件通知，而非為全系統啟動的事件通知。 如需詳細資訊，請參閱 [檢視及設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Workfront管理員可解除鎖定並重新鎖定Adobe Workfront Classic和新Adobe Workfront體驗中事件通知的設定。 但群組管理員只能在新的Adobe Workfront體驗中為群組設定該事件通知。 使用Adobe Workfront Classic的群組管理員可切換至新的Adobe Workfront體驗來設定群組的解除鎖定事件通知，然後切換回Adobe Workfront Classic以查看生效的變更。
>* 子組從上面的頂級組繼承組級事件通知配置。
>


## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>系統管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解除鎖定或重新鎖定設定事件通知的功能

>[!IMPORTANT]
>
>當您重新鎖定通知時，系統中的所有群組都會以您設定的方式繼承通知。 這會覆寫群組管理員可能為群組所做的任何變更，因此最好先與他們協商。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **電子郵件** > **通知**.

1. 請確定 **事件通知** 標籤。
1. 按一下通知右側的圖示，將其切換至解除鎖定 ![](assets/lock-toggle-button.png) 或已鎖定 ![](assets/unlock-toggle-button.png) 位置。

   或

   如果要一次解除鎖定或鎖定多個通知，請選取這些通知，然後按一下「解除鎖定」 ![](assets/unlock-icon-toolbar.png) 或鎖定 ![](assets/lock-icon-locked-qs.png) 按鈕。

1. 按一下&#x200B;**儲存**。
1. （可選）如果要為頂層組配置事件通知，而不是將此任務留給組的管理員，可以執行以下操作之一：

   * 刪除 **系統事件通知** 在通知清單上方的搜索框中，搜索並選擇頂級組的名稱以列出其通知，然後激活或取消激活顯示清單中的解鎖通知。
   * 按一下 **群組** 在左側功能表中，按一下頂層群組的名稱。 按一下 **事件通知** 在左側面板中，然後設定解除鎖定事件通知，如 [檢視及設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
