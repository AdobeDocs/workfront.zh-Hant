---
user-type: administrator
product-area: system-administration
keywords: 修改，電子郵件，通知，設定，批次，大量編輯，設定，多個，使用者
navigation-topic: emails-administration
title: 修改多位使用者的電子郵件通知設定
description: 本文為Workfront或群組管理員提供有關如何更新其他使用者的電子郵件通知的資訊。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# 修改多位使用者的電子郵件通知設定

<!-- Audited: 12/2023 -->

如果您是Adobe Workfront管理員或您具有允許編輯其他使用者設定的「規劃者」存取層級，您可以一次為多個使用者設定通知設定。 這包括指定使用者是否在事件發生時收到通知，或如[Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md)中所述，在每日摘要電子郵件中收到通知。 如需有關編輯使用者所需存取層級的資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

您也可以一次為一位使用者設定電子郵件通知，包括您自己的設定檔。 如需詳細資訊，請參閱[修改您自己的電子郵件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>新計畫：標準 </p>
 <p>或</p> 
<p>目前計畫：計畫 </p> 
</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 修改多個使用者的電子郵件通知設定

大量設定通知設定時，您只能變更所選使用者共同擁有的設定。

當您修改通知設定時，該通知設定會顯示標籤&#x200B;**已編輯**，通知您已修改該通知設定。

若要修改多個使用者的電子郵件通知設定：

{{step-1-to-users}}

1. 選取使用者，然後按一下[編輯]。****
1. 在出現的&#x200B;**編輯人員**&#x200B;方塊中，按一下&#x200B;**通知**。

1. 展開類別以檢視與該類別相關的通知設定。

   如果至少選取了一個使用者，但通知與其他選取的使用者的通知不符，則該通知的類別核取方塊包含水平線![Line而不是核取記號](assets/straight-line-instead-of-checkmark.jpg)。


1. 按一下您希望使用者每天或立即接收的任何通知，或清除您希望他們停止接收的任何通知。

   >[!NOTE]
   >
   >   對於&#x200B;**通訊**&#x200B;類別，您只能選取即時傳遞的個別通知。 您必須選取所有要在每日摘要中傳送的通知。


1. 如果您選取以每日摘要傳送通知，請在&#x200B;**電子郵件每日摘要**&#x200B;後選單的&#x200B;**通知**&#x200B;區段頂端選取您想要摘要傳送的當天時間。

   ![每日摘要時間](assets/daily-digest-time.png)

   每日摘要包含符合在所選時間之前24小時通知標準的事件。 使用者會收到每種通知型別的一封每日摘要電子郵件。

   每日摘要可能會在您選取的時間後送達，端視系統中排入傳送佇列的電子郵件數量而定。 列出的時間是您瀏覽器設定中指定的當地時間。
