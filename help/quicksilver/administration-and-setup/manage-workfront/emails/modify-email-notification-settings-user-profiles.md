---
user-type: administrator
product-area: system-administration
keywords: 修改，電子郵件，通知，設定，批量，批量編輯，配置，多個，用戶
navigation-topic: emails-administration
title: 修改使用者設定檔中的電子郵件通知設定
description: 如果您是Adobe Workfront管理員，或您有計畫員存取層級可讓您編輯其他使用者的設定，則可一次為多個使用者設定通知設定。 這包括指定使用者是否會在事件發生時收到通知，或是依照Adobe Workfront通知所述，在每日摘要式電子郵件中收到通知。 有關編輯用戶所需的訪問級別的資訊，請參閱授予用戶訪問權限。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# 修改使用者設定檔中的電子郵件通知設定

如果您是Adobe Workfront管理員，或您有計畫員存取層級可讓您編輯其他使用者的設定，則可一次為多個使用者設定通知設定。 這包括指定使用者是否會在事件發生時收到通知，或是在一封每日摘要電子郵件中收到通知，如 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md). 如需編輯使用者所需的存取層級相關資訊，請參閱 [授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

批量配置通知設定時，您只能更改所選用戶的共同設定。

您也可以一次為一個使用者設定電子郵件通知。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請聯絡您的Workfront管理員。

## 大量修改多個使用者的電子郵件通知設定

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png). 選取使用者，然後按一下 **編輯**.
1. 在 **編輯人員** 框，按一下 **通知**.

1. 展開類別以檢視與該類別相關的通知設定。

   如果至少選擇了一個用戶，其中通知與其他選定用戶的通知不匹配，則該通知的類別複選框包含水準行 ![](assets/straight-line-instead-of-checkmark.jpg) 而不是勾號。

1. 按一下您希望用戶每天或即時收到的任何通知，或清除您希望用戶停止接收的任何通知。

   若 **通訊** 類別中，您只能選擇即時傳送的個別通知。 您必須選取要在每日摘要中傳送的所有通知。

   修改通知設定時，標籤 **已編輯** 會針對該通知設定顯示，讓您知道該通知設定已修改。

1. 如果您選取要以每日摘要傳送的通知，請選取要將摘要傳送到 **通知** 區段 **之後的電子郵件每日摘要** 功能表。

   選取傳送時間後， **之後的電子郵件每日摘要** 方塊會以橘色框架顯示，指出已編輯傳送的時間。

   每日摘要包含在所選時間之前24小時符合通知標準的事件。 使用者會收到每種通知類型的每日摘要電子郵件。

   每日摘要可能會在您選取的時間之後送達，具體取決於系統中排入佇列等候傳送的電子郵件數量。 列出的時間是瀏覽器設定中指定的本地時間。
