---
user-type: administrator
product-area: system-administration
keywords: 修改，電子郵件，通知，設定，批次，大量編輯，設定，多個，使用者
navigation-topic: emails-administration
title: 修改使用者設定檔中的電子郵件通知設定
description: 如果您是Adobe Workfront管理員，或您具有允許編輯其他使用者設定的「供需規劃員」存取層級，則可以一次為多個使用者設定通知設定。 這包括指定使用者在事件發生時收到通知，還是如Adobe Workfront通知中所述，在每日摘要電子郵件中收到通知。 如需編輯使用者所需存取層級的詳細資訊，請參閱授予使用者存取許可權。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# 修改使用者設定檔中的電子郵件通知設定

如果您是Adobe Workfront管理員，或您具有允許編輯其他使用者設定的「供需規劃員」存取層級，則可以一次為多個使用者設定通知設定。 這包括指定使用者是否在事件發生時收到通知，或是在一封每日摘要電子郵件中收到通知，如中所述 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md). 如需有關編輯使用者所需存取層級的資訊，請參閱 [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

大量設定通知設定時，您只能變更所選使用者通用的設定。

您也可以一次為一位使用者設定電子郵件通知，包括您自己的設定檔。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫或授權型別，請連絡Workfront管理員。

## 大量修改多個使用者的電子郵件通知設定

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png). 選取使用者，然後按一下 **編輯**.
1. 在 **編輯人員** 方塊中，按一下 **通知**.

1. 展開類別以檢視與該類別相關的通知設定。

   如果至少選取了一個使用者，而該使用者的通知與其他選定使用者的通知不符，則該通知的類別核取方塊會包含水平線 ![](assets/straight-line-instead-of-checkmark.jpg) 而不是勾號。

1. 按一下您希望使用者每天或立即收到的任何通知，或清除您希望他們停止接收的任何通知。

   對於 **通訊** 類別時，您可以選取僅供立即傳送的個別通知。 您必須選取所有要在每日摘要中傳送的通知。

   修改通知設定時，標籤 **已編輯** 會為該通知設定顯示，通知您已修改該通知設定。

1. 如果您選取要以每日摘要形式傳送通知，請在 **通知** 中的區段 **在以下時間後以電子郵件傳送每日摘要：** 功能表。

   選取傳送時間後， **在以下時間後以電子郵件傳送每日摘要：** 方塊以橘色框架顯示，表示傳送時間已編輯。

   每日摘要包含符合在選定時間前24小時通知標準的事件。 使用者會收到每種通知型別的每日摘要電子郵件。

   每日摘要可能會在您選取的時間之後到達，端視系統中排入傳送佇列的電子郵件數量而定。 所列出的時間是瀏覽器設定中指定的當地時間。
