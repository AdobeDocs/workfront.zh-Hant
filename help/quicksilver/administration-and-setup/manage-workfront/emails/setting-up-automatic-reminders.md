---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 設定自動提醒
description: 設定自動提醒
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# 設定自動提醒

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

身為Adobe Workfront管理員，您可以設定自動提醒，以在所有任務或問題都到期、延遲或接近計畫完成日期時觸發電子郵件通知。 配置這些設定後，用戶無法禁用自動提醒。

若是延遲通知，則會在每晚傳送電子郵件，直到任務或問題完成為止。

自動提醒可以發送到以下一個或多個：

* 指派給任務或問題的使用者
* 使用者的直接經理
* 直接經理的經理

>[!NOTE]
>
>您無法變更自動提醒所觸發之電子郵件的內容或主旨行。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>系統管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定自動提醒

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **電子郵件** >**自動提醒**.

1. 在 **將延遲通知傳送至** 中，選擇以下任一選項：

   <table>
    <tr>
        <td>「已分配給」用戶</td>
        <td>如果希望將用戶分配給某個任務或問題來接收有關其工作項延遲的延遲通知，請選擇此選項。</td>
        <td></td>
    </tr>
    <tr>
        <td>使用者的管理員</td>
        <td>如果您希望使用者的管理員收到有關其直接報表工作項目延遲的延遲通知，請選取此選項。</td>
        <td></td>
    </tr>
    <tr>
        <td>經理的管理員</td>
        <td>如果希望直接經理的經理收到其直接報表用戶的工作項目延遲通知，請選擇此選項。</td>
        <td></td>
    </tr>
    <tr>
        <td>「已分配給」用戶</td>
        <td>(在 <b>將截止時間提醒發送至</b> )。 如果希望將用戶分配給任務或問題，以接收有關其工作項接近到期日的通知，請選擇此選項。</td>
        <td></td>
    </tr>
</table>

1. 通過選擇工作項的到期日之前或之後的時間量，選擇自動提醒發送的時間。

   時間從任務或問題的計畫完成日期計算。

   指定分鐘、小時、天、周或月數，以將時間添加到任務或問題的「計畫完成日期」。 選擇 **已用分鐘數**, **已用小時數**, **已用天數**，或 **已用周數** 添加時間，包括任何週末、節假日和非工作小時，如計畫中所示。

   例如，如果在星期五分配了任務，且任務的持續時間為3天，則任務完成日期將設定為星期一（假設星期六和星期日是週末）。 如果任務的持續時間為3天（未過），則任務完成日期設定為星期三。

   ![](assets/time-increments-for-automatic-reminder.png)

1. 按一下&#x200B;**儲存**。

## 接收自動提醒

如果您是「自動提醒」通知中的指定實體，您會在達到指定的期限時收到電子郵件。 若是延遲通知，則會在每晚傳送電子郵件，直到任務或問題完成為止。

具有特定相依性類型的任務可能會在指定的開始日期之後傳送，即使這些任務已過期。 例如，如果某個任務具有「完成 — 開始」(fs)相關性的前置任務，則即使它已通過指定的開始日期，它也不會包含在電子郵件中，因為在前置任務完成之前，您無法啟動該任務。

如需接收自動提醒電子郵件的詳細資訊，請參閱 [自動提醒](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) 區段 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## 傳送自動提醒

當符合Workfront管理員選取的時間時，就會立即傳送自動提醒。

如果要觸發手動發送自動提醒電子郵件，可使用診斷程式執行。 有關在Workfront中訪問和使用診斷的詳細資訊，請參見 [使用診斷程式觸發自動化流程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
