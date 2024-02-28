---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 設定自動提醒
description: 設定自動提醒
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 4%

---

# 設定自動提醒

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為Adobe Workfront管理員，您可以設定自動提醒，以在所有任務或問題到期、延遲或接近計畫完成日期時觸發電子郵件通知。 在您設定這些設定後，使用者將無法停用自動提醒。

對於延遲通知，在任務或問題完成之前，每晚會傳送電子郵件。

自動提醒可以傳送至下列一或多個專案：

* 指派給任務或問題的使用者
* 使用者的直接管理員
* 直接管理員的管理員

>[!NOTE]
>
>您無法變更自動提醒所觸發之電子郵件的內容或主旨列。

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

## 設定自動提醒

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **電子郵件** >**自動提醒**.

1. 在 **傳送延遲通知至** 區域，選取下列任一選項：

   <table>
    <tr>
        <td>「指派至」使用者</td>
        <td>如果您希望指派給任務或問題的使用者收到關於其工作專案延遲的延遲通知，請選取此選項。</td>
        <td></td>
    </tr>
    <tr>
        <td>使用者的管理員</td>
        <td>如果您希望使用者的經理收到其直接下屬工作專案延遲的延遲通知，請選取此選項。</td>
        <td></td>
    </tr>
    <tr>
        <td>經理的管理員</td>
        <td>如果您希望直屬經理的經理收到其直屬下屬使用者之一工作專案延遲的延遲通知，請選取此選項。</td>
        <td></td>
    </tr>
    <tr>
        <td>「指派至」使用者</td>
        <td>(在 <b>傳送期限提醒至</b> 區域。) 如果您希望指派給任務或問題的使用者收到臨近到期日的工作專案通知，請選取此選項。</td>
        <td></td>
    </tr>
</table>

1. 選取工作專案到期日之前或之後的時間量，以選取自動提醒的傳送時間。

   從任務或問題的規劃完成日期計算時間。

   指定任務或問題的計畫完成日期要增加時間的分鐘數、小時數、天數、周數或月數。 選取 **經過的分鐘數**， **經過的時數**， **經過的天數**，或 **經過的周數** 新增時間，包括排程中所指示的任何週末、假日及非工作時間。

   例如，如果任務指派在星期五且持續時間為3天，則任務完成日期設定為星期一（假設星期六和星期日是週末）。 如果任務的持續時間為3天（未過），則任務完成日期設定為星期三。

   ![](assets/time-increments-for-automatic-reminder.png)

1. 按一下「**儲存**」。

## 接收自動提醒

如果您是自動提醒通知中的指定實體，則會在達到指定期限時收到電子郵件。 對於延遲通知，在任務或問題完成之前，每晚會傳送電子郵件。

具有特定相依性型別的任務可能會在指定的開始日期之後傳遞，即使這些任務已過期。 例如，如果任務的前置任務具有「完成 — 開始」(fs)相依性，即使任務已超過指定的開始日期，也不會包含在電子郵件中，因為您必須等到前置任務完成才能開始該任務。

如需有關接收自動提醒電子郵件的詳細資訊，請參閱 [自動提醒](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) 中的區段 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## 傳送自動提醒

在符合Workfront管理員所選取的時間時，立即傳送自動提醒。

如果您想要觸發手動傳送自動提醒電子郵件，可以使用「診斷」來執行。 如需在Workfront中存取及使用診斷的詳細資訊，請參閱 [使用診斷來觸發自動化流程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
