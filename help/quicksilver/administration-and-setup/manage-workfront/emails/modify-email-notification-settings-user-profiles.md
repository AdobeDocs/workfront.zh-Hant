---
user-type: administrator
product-area: system-administration
keywords: 修改，電子郵件，通知，設定，批次，大量編輯，設定，多個，使用者
navigation-topic: emails-administration
title: 修改使用者設定檔中的電子郵件通知設定
description: 如果您是Adobe Workfront管理員或您具有允許編輯其他使用者設定的「規劃者」存取層級，您可以一次為多個使用者設定通知設定。 這包括指定使用者在發生事件時收到通知，還是如Adobe Workfront通知中所述，以每日摘要電子郵件收到。 如需有關編輯使用者所需存取層級的資訊，請參閱授予使用者存取權。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 91eb8770c07396b5772029e9d2370f0b1f10d4a1
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# 修改使用者設定檔中的電子郵件通知設定

如果您是Adobe Workfront管理員或您具有允許編輯其他使用者設定的「規劃者」存取層級，您可以一次為多個使用者設定通知設定。 這包括指定使用者在發生事件時收到通知，還是在一封每日摘要電子郵件中收到通知，如中所述 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md). 如需有關編輯使用者所需存取層級的資訊，請參閱 [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

大量設定通知設定時，您只能變更所選使用者共同擁有的設定。

>[!NOTE]
>
>您也可以一次為一位使用者設定電子郵件通知，包括您自己的設定檔。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


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

&#42;若要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

## 大量修改多個使用者的電子郵件通知設定

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png). 選取使用者，然後按一下 **編輯**.
1. 在 **編輯人員** 方塊中，按一下 **通知**.

1. 展開類別以檢視與該類別相關的通知設定。

   如果至少選取了一個通知與其他選定使用者的通知不匹配的使用者，則該通知的類別核取方塊包含水平線 ![](assets/straight-line-instead-of-checkmark.jpg) 而不是勾號。

1. 按一下您希望使用者每天或立即接收的任何通知，或清除您希望他們停止接收的任何通知。

   對於 **通訊** 類別中，您可以選取僅供即時傳送的個別通知。 您必須選取所有要在每日摘要中傳送的通知。

   當您修改通知設定時，標籤 **已編輯** 會為該通知設定顯示，通知您已修改該通知設定。

1. 如果您選取以每日摘要傳送通知，請在 **通知** 中的區段 **在以下時間後以電子郵件傳送每日摘要：** 功能表。

   選取傳送時間後， **在以下時間後以電子郵件傳送每日摘要：** 方塊以橘色框架顯示，表示傳送的時間已編輯。

   每日摘要包含符合在所選時間之前24小時通知標準的事件。 使用者會收到每種通知型別的一封每日摘要電子郵件。

   每日摘要可能會在您選取的時間後送達，端視系統中排入傳送佇列的電子郵件數量而定。 列出的時間是您瀏覽器設定中指定的當地時間。
