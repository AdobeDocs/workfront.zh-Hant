---
product-area: requests
navigation-topic: create-requests
title: 讓使用者將問題透過電子郵件傳送至「請求佇列」專案
description: 讓使用者將問題透過電子郵件傳送至「請求佇列」專案
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: ca3c28174dca24f14a75869bdc209569d8d8d1a0
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 讓使用者將問題透過電子郵件傳送至「請求佇列」專案

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

您可以設定專案，讓使用者透過電子郵件將問題新增至專案。 只有在將專案指定為「請求佇列」時，才可將問題以電子郵件傳送至專案。 如需建立「請求佇列」專案的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

設定專案時需具備下列必要條件，才能讓使用者透過電子郵件將問題新增至專案。

啟用此功能之前，必須符合下列條件：

* 將問題透過電子郵件傳送至此帳戶的使用者必須是具有Workfront授權的有效使用者。
* 外部使用者無法將問題透過電子郵件傳送至請求佇列，因為他們沒有建立問題的存取權。
* 將問題透過電子郵件傳送給此帳戶的使用者，必須擁有專案的新增問題權限。
* 來自與作用中Workfront使用者相關聯的電子郵件地址的電子郵件是唯一可傳送問題至專案的電子郵件。
* 專案會設為「請求佇列」。
* 與專案相關聯的電子郵件帳戶不會連結至Workfront使用者帳戶。

## 在Workfront中設定專案

>[!NOTE]
>
>啟用電子郵件佇列設定時，請記住下列事項：
>
>* Workfront允許所有叢集中每個請求佇列使用一封唯一的電子郵件。 如果您選擇停用請求佇列，只要您建立的電子郵件地址仍位於「接收電子郵件地址」方塊中，就會保留該電子郵件地址。 如果您選擇停止使用取用電子郵件，則必須從取用電子郵件欄位中刪除該電子郵件，以便供日後使用。
>
>* 如果請求佇列有多個佇列主題或主題群組，Workfront會隨機選取電子郵件請求所要前往的佇列主題，導致無法管理已傳送的請求。
   >我們建議您設定用來透過電子郵件接收請求的專案，應該不要有多個佇列主題。 如果提交的請求是針對不同的資源或項目，則您應在提交後手動傳送或移動這些請求。


1. 前往您要啟用的專案，透過電子郵件接收問題。
1. 按一下 **隊列詳細資訊** 中。 您可能需要按一下 **顯示更多** 第一個。
1. 在 **隊列類型** 區域，選擇 **發佈為說明請求佇列**.

1. 向下捲動至 **電子郵件佇列設定** 區域，然後選取 **透過電子郵件啟用請求接收**.

1. 在 **接收電子郵件地址** 框。

   您必須建立唯一的電子郵件地址。 建議您使用公司名稱作為接收電子郵件地址的一部分。

   >[!CAUTION]
   >
   >* 如果刪除包含請求隊列的項目，則無法從資源回收筒恢復此電子郵件地址。
   >
   >* 由於此電子郵件地址必須是唯一的，因此如果刪除，它將來可能不可用。

   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. （選用）選取 **轉寄所有無法透過電子郵件提交的問題**，然後在下方的方塊中輸入轉送電子郵件地址。

   此電子郵件地址會接收有關無法提交至專案的電子郵件的資訊。

1. 按一下&#x200B;**儲存**。現在，具有作用中Workfront帳戶的使用者傳送電子郵件給此電子郵件地址時，Workfront專案中會產生問題。

   >[!NOTE]
   >
   >使用者必須有權限在專案中建立問題，才能透過電子郵件提交。 您可以在「進階設定」下的「共用」對話方塊中授予此存取權。
   >
   >外部使用者無法將問題透過電子郵件傳送至請求佇列，因為他們沒有建立問題的存取權。

## 在Workfront接收問題

Workfront使用者傳送電子郵件至Workfront時，會發生下列情況：

* 電子郵件的主旨行會變成「問題名稱」。
* 電子郵件的內文會變成問題說明。
* 如果有任何檔案附加至電子郵件，這些檔案會附加至Workfront中的問題。
* 傳送電子郵件的使用者會成為Workfront中新問題的主要連絡人。
* 電子郵件的內文不能超過4,000個字元。
* 電子郵件附件總計不能超過7 MB。
