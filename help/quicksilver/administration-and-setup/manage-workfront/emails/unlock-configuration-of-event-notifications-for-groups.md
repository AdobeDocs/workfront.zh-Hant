---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 解鎖或鎖定所有群組的事件通知設定
description: 如果您是Adobe Workfront管理員，您可以解除鎖定或重新鎖定群組管理員為其管理的最上層群組設定事件通知的能力。 事件通知的設定包含啟用或停用。
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# 解鎖或鎖定所有群組的事件通知設定

如果您是Adobe Workfront管理員，您可以解除鎖定或重新鎖定群組管理員為其管理的最上層群組設定事件通知的能力。 事件通知的設定包含啟用或停用。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

管理員為群組設定事件通知時，該設定會影響該群組或其子群組之一為其主群組的使用者。 在其使用者設定檔中，這些使用者會看到為其主群組啟用的事件通知，而不是在整個系統內啟用的事件通知。 如需詳細資訊，請參閱 [檢視和設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Workfront管理員可以解除鎖定和重新鎖定Adobe Workfront Classic和新Adobe Workfront體驗中事件通知的設定。 但群組管理員只能在新的Adobe Workfront體驗中為群組設定該事件通知。 使用Adobe Workfront Classic的群組管理員可以切換至新的Adobe Workfront Experience，為群組設定未鎖定的事件通知，然後切換回Adobe Workfront Classic以檢視生效的變更。
>* 子群組會繼承其上頂層群組的群組層級事件通知設定。
>

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>系統管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解鎖或重新鎖定設定事件通知的功能

>[!IMPORTANT]
>
>當您重新鎖定通知時，系統中的所有群組都會繼承與您設定的完全相同的通知。 這會覆寫群組管理員可能對其群組所做的任何變更，因此建議您先與他們商議。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **電子郵件** > **通知**.

1. 確定 **事件通知** 標籤已開啟。
1. 按一下通知右側的圖示，將其切換至已鎖定 ![「鎖定」圖示](assets/lock-toggle-button.png) 或已解鎖 ![「解除鎖定」圖示](assets/unlock-toggle-button.png) 位置。

   或

   如果您想要一次解除鎖定或鎖定多個通知，請選取通知，然後按一下解除鎖定 ![「解除鎖定」圖示](assets/unlock-icon-toolbar.png) 或鎖定 ![「鎖定」圖示](assets/lock-icon-locked-qs.png) 按鈕顯示在清單上方的工具列中。

1. 按一下「**儲存**」。
1. （選擇性）如果要為最上層群組設定事件通知，而不是將此工作留給群組管理員，您可以執行下列任一項作業：

   * 刪除 **系統事件通知** 在通知清單上方的搜尋方塊中，搜尋並選取最上層群組的名稱，以列出其通知，然後在顯示的清單中啟動或停用已解鎖的通知。
   * 按一下 **群組** 在左側功能表中，按一下最上層群組的名稱。 按一下 **事件通知** 然後，在左側面板中設定「已解除鎖定」事件通知，如中所述 [檢視和設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
