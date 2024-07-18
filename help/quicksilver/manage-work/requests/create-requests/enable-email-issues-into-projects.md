---
product-area: requests
navigation-topic: create-requests
title: 讓使用者透過電子郵件將問題傳送到請求佇列專案
description: 讓使用者透過電子郵件將問題傳送到請求佇列專案
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 9cda6fd41ba7fcb9b9f412a7c2b7ffd39f3fe189
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# 讓使用者透過電子郵件將問題傳送到請求佇列專案

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

您可以設定專案，讓使用者能透過電子郵件將問題新增至專案。 只有當專案被指定為「請求佇列」時，您才可允許以電子郵件將問題傳送到專案。 如需有關建立請求佇列專案的詳細資訊，請參閱[建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯問題的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

設定專案需要以下先決條件，以允許使用者透過電子郵件將問題新增至專案。

在啟用此功能之前，必須滿足以下條件：

* 透過電子郵件將問題傳送到此帳戶的使用者必須是具有Workfront授權的有效使用者。
* 透過電子郵件將問題傳送到此帳戶的使用者必須具有專案的「新增問題」許可權。
* 外部使用者無法透過電子郵件將問題傳送到請求佇列，因為他們無權建立問題。
* 只有來自與作用中Workfront使用者相關聯之電子郵件地址的電子郵件，才允許將問題傳送至專案。 從與Workfront帳戶無關的電子郵件轉寄至使用中Workfront使用者電子郵件的電子郵件無法在專案下建立問題，因為原始寄件者的電子郵件地址必須與使用中Workfront帳戶相關聯。
* 專案已設定為請求佇列。
* 與專案相關聯的電子郵件帳戶未連結至Workfront使用者帳戶。

## 在Workfront中設定專案

>[!NOTE]
>
>啟用電子郵件佇列設定時，請記住下列事項：
>
>* Workfront允許所有叢集的每個請求佇列都有一個唯一的電子郵件。 如果您選擇停用您的要求佇列，只要您建立的電子郵件地址仍在錄取電子郵件地址方塊中，就會保留該地址。 如果您選擇停止使用錄取電子郵件，您必須從錄取電子郵件欄位中刪除它，以便將來可以使用。
>
>* 如果請求佇列有多個佇列主題或主題群組，Workfront會隨機選取要傳送電子郵件請求的佇列主題，使電子郵件請求難以管理。
>我們建議您設定為透過電子郵件接收請求的專案不應有多個佇列主題。 如果提交的請求是針對不同的資源或專案，您應該在提交後手動路由或移動這些請求。

1. 前往您要啟用的專案，透過電子郵件接收問題。
1. 按一下左側面板中的&#x200B;**佇列詳細資料**。 您可能需要先按一下&#x200B;**顯示更多**。
1. 在&#x200B;**佇列型別**&#x200B;區域中，選取&#x200B;**Publish作為說明要求佇列**。

1. 向下捲動至&#x200B;**電子郵件佇列設定**&#x200B;區域，然後選取&#x200B;**啟用透過電子郵件要求錄取**。

1. 在&#x200B;**錄取電子郵件地址**&#x200B;方塊中輸入電子郵件地址的開頭。

   您必須建立唯一的電子郵件地址。 建議您使用公司名稱作為錄取電子郵件地址的一部分。

   >[!CAUTION]
   >
   >* 如果刪除包含請求佇列的專案，則無法從資源回收筒復原此電子郵件地址。
   >
   >* 由於此電子郵件地址必須是唯一的，因此若將其刪除，未來可能無法使用。
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. （選擇性）選取&#x200B;**轉寄所有無法透過電子郵件提交的問題**，然後在下列方塊中輸入轉寄電子郵件地址。

   此電子郵件地址會接收無法提交至專案的電子郵件相關資訊。

1. 按一下「**儲存**」。現在，當具有有效Workfront帳戶的使用者傳送電子郵件至此電子郵件地址時，Workfront專案中就會建立一個問題。

   >[!NOTE]
   >
   >使用者必須擁有在專案中建立問題的存取權，才能透過電子郵件提交。 您可以在「進階設定」下的「共用」對話方塊中授與此存取權。
   >
   >外部使用者無法透過電子郵件將問題傳送到請求佇列，因為他們無權建立問題。

## 在Workfront中接收問題

當Workfront使用者傳送電子郵件至Workfront時，會發生下列情況：

* 電子郵件的「主旨」行會變成「問題名稱」。
* 電子郵件內文會變成問題的說明。
* 如果電子郵件有任何附加檔案，這些檔案會附加至Workfront中的問題。
* 傳送電子郵件的使用者會成為Workfront新問題的主要聯絡人。
* 電子郵件的內文不可超過4,000個字元。
* 電子郵件附件總計不得超過7 MB。
