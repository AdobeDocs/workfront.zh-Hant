---
product-area: requests
navigation-topic: create-requests
title: 讓使用者透過電子郵件將問題傳送到請求佇列專案
description: 您可以設定專案，讓使用者能透過電子郵件將問題新增至專案。
author: Alina, Courtney
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---

# 讓使用者透過電子郵件將問題傳送到請求佇列專案

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

您可以設定專案，讓使用者能透過電子郵件將問題新增至專案。 您只能允許在專案指定為「請求佇列」時，將問題以電子郵件傳送至專案。 有關創建請求佇列專案的更多資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 許可證</td> 
   <td> <p>新：貢獻者或以上</p>
   或
   <p>當前：請求或更高</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級組態</td> 
   <td> <p>編輯存取問題</p>  </td> 
  </tr> 
 </tbody> 
</table>

有關此表中資訊的更多詳細資訊，請參閱 [Workfront 文件中](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)的訪問要求。

+++

## 先決條件

設定項目以允許使用者透過電子郵件向專案新增問題需要以下條件：

* 通過電子郵件將問題發送給此帳戶的用戶必須是具有 Workfront 許可證的活動使用者。
* 通過電子郵件將問題發送給此帳戶的用戶必須對專案具有「添加問題」許可權。
* 外部使用者無法透過電子郵件將問題傳送到請求佇列，因為他們無權建立問題。
* 只有來自與作用中Workfront使用者相關聯之電子郵件地址的電子郵件，才允許將問題傳送至專案。 從與Workfront帳戶無關的電子郵件轉寄至使用中Workfront使用者電子郵件的電子郵件無法在專案下建立問題，因為原始寄件者的電子郵件地址必須與使用中Workfront帳戶相關聯。
* 專案已設定為請求佇列。
* 與項目關聯的電子郵件帳戶未連結到 Workfront 用戶 帳戶。

## 在 Workfront 中設定專案

>[!NOTE]
>
>啟用電子郵件佇列設定時，請記住下列事項：
>
>* Workfront允許所有叢集的每個請求佇列都有一個唯一的電子郵件。 如果您選擇停用您的要求佇列，只要您建立的電子郵件地址仍在錄取電子郵件地址方塊中，就會保留該地址。 如果您選擇停止使用錄取電子郵件，您必須從錄取電子郵件欄位中刪除它，以便將來可以使用。
>
>* 如果請求佇列有多個佇列主題或主題群組，Workfront會隨機選取要傳送電子郵件請求的佇列主題，使電子郵件請求難以管理。
>我們建議您設定為透過電子郵件接收請求的專案不應有多個佇列主題。 如果提交的請求是針對不同的資源或專案，您應該在提交後手動路由或移動這些請求。

1. 轉到要啟用以通過電子郵件接收問題的專案。
1. 按兩下 **左側面板中的佇列詳細資訊** 。 您可能需要先按兩下 **顯示更多** 。
1. 在“佇列類型”**區域中，選擇**“Publish作為說明請求佇列&#x200B;**”。**

1. 向下滾動到「 **電子郵件佇列設定** 區域，然後選擇」 **啟用通過電子郵件接收**&#x200B;請求」。

1. 在「 **接收電子郵件位址** 」框中輸入電子郵件地址的開頭。

   您必須建立唯一的電子郵件位址。 我們建議使用您的公司姓名作為您的接收電子郵件位址的一部分。

   >[!CAUTION]
   >
   >* 如果刪除包含請求佇列的專案，則無法從回收站中恢復此電子郵件位址。
   >
   >* 由於此電子郵件地址必須是唯一的，因此如果刪除，將來可能無法使用。
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. （選擇） **選擇轉發所有無法通過電子郵件提交**&#x200B;的問題，然後在下面的框中輸入轉發電子郵件位址。

   此電子郵件位址接收有關無法提交到專案的電子郵件的資訊。

1. 按一下「**儲存**」。現在，當具有有效Workfront帳戶的使用者傳送電子郵件至此電子郵件地址時，Workfront專案中就會建立一個問題。

   >[!NOTE]
   >
   >使用者必須擁有在專案中建立問題的存取權，才能透過電子郵件提交。 您可以在「進階設定」下的「共用」對話方塊中授與此存取權。
   >
   >外部使用者無法透過電子郵件將問題傳送到請求佇列，因為他們無權建立問題。

## 在 Workfront 中接收問題

當 Workfront 用戶向 Workfront 發送電子郵件時，會發生以下情況：

* 電子郵件的主旨行將成為問題名稱。
* 電子郵件的正文將成為問題的說明。
* 如果電子郵件中附加了任何文件，這些檔將附加到 Workfront 中的問題。
* 發送電子郵件的用戶將成為 Workfront 中新問題的主要連絡人。
* 電子郵件的正文文本不能超過 4,000 個字元。
* 電子郵件附件的總大小不得超過 7 MB。
