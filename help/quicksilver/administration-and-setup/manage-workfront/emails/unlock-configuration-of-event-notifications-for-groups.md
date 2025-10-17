---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 解鎖或鎖定所有群組的事件通知設定
description: 如果您是Adobe Workfront管理員，您可以解除鎖定或重新鎖定群組管理員為其管理的最上層群組設定事件通知的能力。 事件通知的設定包含啟用或停用。
author: Courtney, Becky
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 解鎖或鎖定所有群組的事件通知設定

如果您是Adobe Workfront管理員，您可以解除鎖定或重新鎖定群組管理員為其管理的最上層群組設定事件通知的能力。 事件通知的設定包含啟用或停用。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

管理員為群組設定事件通知時，該設定會影響該群組或其子群組之一為其主群組的使用者。 在其使用者設定檔中，這些使用者會看到為其主群組啟用的事件通知，而不是在整個系統內啟用的事件通知。 如需詳細資訊，請參閱[檢視並設定群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。

>[!NOTE]
>
>* Workfront管理員可以解除鎖定和重新鎖定Adobe Workfront Classic和新Adobe Workfront體驗中事件通知的設定。 但群組管理員只能在新的Adobe Workfront體驗中為群組設定該事件通知。 使用Adobe Workfront Classic的群組管理員可以切換至新的Adobe Workfront Experience，為群組設定未鎖定的事件通知，然後切換回Adobe Workfront Classic以檢視生效的變更。
>* 子群組會繼承其上頂層群組的群組層級事件通知設定。
>

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>系統管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解鎖或重新鎖定設定事件通知的功能

>[!IMPORTANT]
>
>當您重新鎖定通知時，系統中的所有群組都會繼承與您設定的完全相同的通知。 這會覆寫群組管理員可能對其群組所做的任何變更，因此建議您先與他們商議。

{{step-1-to-setup}}

1. 按一下&#x200B;**電子郵件** > **通知**。

1. 請確定&#x200B;**事件通知**&#x200B;索引標籤已開啟。
1. 按一下通知右側的圖示，可將其切換至鎖定的![鎖定圖示](assets/lock-toggle-button.png)或解除鎖定的![解除鎖定圖示](assets/unlock-toggle-button.png)位置。

   或

   若要一次解除鎖定或鎖定多個通知，請選取通知，然後按一下清單上方工具列中顯示的[解除鎖定![解除鎖定]圖示](assets/unlock-icon-toolbar.png)或[鎖定![鎖定]圖示](assets/lock-icon-locked-qs.png)按鈕。

1. 按一下「**儲存**」。
1. （選擇性）如果要為最上層群組設定事件通知，而不是將此工作留給群組管理員，您可以執行下列任一項作業：

   * 在通知清單上方的搜尋方塊中刪除&#x200B;**系統事件通知**，搜尋並選取最上層群組的名稱以列出其通知，然後在顯示的清單中啟動或停用已解除鎖定的通知。
   * 按一下左側功能表中的&#x200B;**群組**，然後按一下最上層群組的名稱。 按一下左側面板中的&#x200B;**事件通知**，然後設定解除鎖定的事件通知，如[檢視及設定群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知中所述。
