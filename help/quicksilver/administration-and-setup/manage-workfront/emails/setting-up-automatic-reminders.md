---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 設定自動提醒
description: 您可以設定自動提醒，以在所有任務或問題到期、延遲或接近計畫完成日期時觸發電子郵件通知。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sxv8RUKwTr-SABLfOrmTa0J9ToM62-1tF5rFEnu41UI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f283a5f64062e5878373527de46b0d993b545ba7
workflow-type: tm+mt
source-wordcount: 836
ht-degree: 4%

---

# 設定自動提醒

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為Adobe Workfront管理員，您可以設定自動提醒，以在所有任務、問題或其他指派的工作專案到期、延遲或接近計畫完成日期時觸發電子郵件通知。

在您設定這些設定後，使用者將無法停用自動提醒。 無論使用者在其「我的設定」區域中的通知設定為何，都會傳送自動提醒。

對於延遲通知，在任務或問題完成之前，每晚會傳送電子郵件。 這表示使用者每天都會在任務或問題未完成時收到通知。

自動提醒可以傳送至下列一或多個專案：

* 指派給任務或問題的使用者
* 使用者的直接管理員
* 直接管理員的管理員

>[!NOTE]
>
>您無法變更自動提醒所觸發之電子郵件的內容或主旨列。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
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

## 自動提醒功能的詳細資料

### 與其他型別提醒的區別

自動提醒是Workfront任務和問題的設定層級提醒功能，與物件層級提醒通知功能不同。 如需關於自動提醒與提醒通知之間差異的資訊，請參閱[自動提醒與提醒通知](/help/quicksilver/administration-and-setup/tips-tricks-and-troubleshooting/auto-reminders-vs-reminder-notifications.md)。

自動提醒也無法處理校訂和校訂決策，而是依照單獨的提醒流程進行。 有關校訂和校訂決定提醒的詳細資訊，請參閱[校訂通知和提醒](/help/quicksilver/workfront-proof/wp-emailsntfctns/wp-emails-and-notifications.md)下的文章。

## 使用自動提醒時的注意事項

使用自動提醒時，請考量下列事項：

* 逾期的電子郵件每天會以每位收件者的一個摘要電子郵件傳送，而非以個別電子郵件的形式依專案傳送。
* 啟用自動提醒可能會導致已逾期的問題或工作出現在下一個「逾期」摘要電子郵件中，無論專案逾期多久。
* 提醒僅適用於目前/作用中狀態的專案。
* 自動提醒設定中的「天數」是指可感知排程的工作日，而非經過的天數或行事曆時間。



## 設定自動提醒

{{step-1-to-setup}}

1. 按一下&#x200B;**電子郵件** > **自動提醒**。

1. 在&#x200B;**傳送延遲通知至**&#x200B;區域中，選取下列任一選項：

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
        <td>（在<b>傳送期限提醒給</b>區域。） 如果您希望指派給任務或問題的使用者收到臨近到期日的工作專案通知，請選取此選項。</td>
        <td></td>
    </tr>
   </table>

1. 選取工作專案到期日之前或之後的時間量，以選取自動提醒的傳送時間。

   從任務或問題的規劃完成日期計算時間。

   指定任務或問題的計畫完成日期要增加時間的分鐘數、小時數、天數、周數或月數。 選取&#x200B;**經過的分鐘數**、**經過的時數**、**經過的天數**&#x200B;或&#x200B;**經過的周數**，以新增排程中所指示的時間，包括任何週末、假日及非工作時間。

   例如，如果任務指派在星期五且持續時間為3天，則任務完成日期設定為星期一（假設星期六和星期日是週末）。 如果任務的持續時間為3天（未過），則任務完成日期設定為星期三。

   ![時間增量](assets/time-increments-for-automatic-reminder.png)

1. 按一下「**儲存**」。

## 接收自動提醒

如果您是自動提醒通知中的指定實體，則會在達到指定期限時收到電子郵件。 對於延遲通知，在任務或問題完成之前，每晚會傳送電子郵件。

具有特定相依性型別的任務可能會在指定的開始日期之後傳遞，即使這些任務已過期。 例如，如果任務的前置任務具有「完成 — 開始」(fs)相依性，即使任務已超過指定的開始日期，也不會包含在電子郵件中，因為您必須等到前置任務完成才能開始該任務。

如需接收自動提醒電子郵件的詳細資訊，請參閱[Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md)中的[自動提醒](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders)區段。

## 傳送自動提醒

在符合Workfront管理員所選取的時間時，立即傳送自動提醒。

如果您想要觸發手動傳送自動提醒電子郵件，可以使用「診斷」來執行。 如需在Workfront中存取及使用診斷的詳細資訊，請參閱[使用診斷來觸發自動化程式](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)。
