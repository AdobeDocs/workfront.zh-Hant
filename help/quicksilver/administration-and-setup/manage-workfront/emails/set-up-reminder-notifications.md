---
title: 設定提醒通知
description: 設定提醒通知
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 1%

---

# 設定提醒通知

提醒通知會根據指定的條件傳送電子郵件給收件者。 作為Adobe Workfront管理員或具有計畫員訪問級別和管理權限的用戶，您可以手動將提醒通知與工作項（如項目、任務、問題和工時單）關聯。

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

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
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>計畫員或更高版本，具有提醒通知的管理訪問權限</p> <p>有關授予計畫用戶管理訪問權限的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 自訂提醒電子郵件

您可以使用包含自訂電子郵件主旨和內文的自訂電子郵件自訂提醒通知。 電子郵件內文可包含自訂HTML。

或者，您可以使用提醒通知隨附的預設電子郵件。 預設電子郵件使用提醒通知名稱作為電子郵件主旨，以及電子郵件內文中的物件名稱，包括觸發通知的事件。

如果要自定義提醒電子郵件，則需要建立電子郵件模板並將其附加到提醒通知。

如需如何建立電子郵件範本的詳細資訊，請參閱 [設定電子郵件範本](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## 建立提醒通知

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **電子郵件** > **通知**.

1. 按一下 **提醒通知** ，然後按一下 **新提醒通知**.

1. 在下拉清單中，按一下要與提醒通知關聯的對象類型。

   例如，如果要將提醒通知附加到時間表，請按一下 **工時單**.

1. 在 **新提醒通知** 框中，指定以下資訊。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">提醒通知名稱</td> 
      <td>指定提醒通知的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">符合資格的期間</td> 
      <td> <p>指定日期之前或之後的小時數、工作日數、天數（日曆日）、周數或月數， <strong>計時</strong> 欄位。</p> <p><b>附註</b>:  
        <ul> 
         <li> <p>提醒通知從指定日期後24小時開始，並在滿足所有條件後開始。</p> </li> 
         <li> <p>項目、任務和問題的提醒通知會在美國山區時間的午夜觸發。 從該日期起，符合提醒通知資格的所有物件都會在該時間後不久向指定使用者觸發通知。</p> </li> 
         <li> <p>工時單的提醒通知會根據您的時區和工時單的「終止日期」、「起始日期」或「上次更新日期」在指定時間發送。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間</td> 
      <td> <p>選取觸發要排程的提醒通知的事件。</p> <p>如果提醒通知是用於項目、任務或問題，則可用選項與完成日期或開始日期相關。 提醒通知會考慮項目、任務和問題的「完成」和「開始」日期上的時間戳。</p> <p>如果提醒通知是用於工時單，則可用選項與終止日期、起始日期或上次更新日期相關。 工時單的提醒通知考慮了工時單結束、開始和上次更新日期的時間戳。 時間表從開始日期的午夜開始（上午12:00），直到結束日期的午夜之前結束（晚上11:59）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">條件</td> 
      <td> <p>選擇條件，以使提醒通知可以計畫。 除非滿足條件選擇，否則不會排程提醒通知。</p> <p>根據您在步驟4中選取的物件類型，可使用下列條件選項：</p> 
       <ul> 
        <li><strong>當前項目不完整：</strong> （可用於任務和問題提醒）僅當提醒通知關聯的對象狀態不是「完成」且項目狀態為「當前」時，才計畫發送提醒通知。</li> 
        <li><strong>當前項目中的所有項目：</strong>（可用於任務和問題提醒）無論對象狀態如何，並且僅當提醒通知關聯的項目狀態為「當前」時，系統才計畫發送提醒通知。</li> 
        <li><strong>未完成項目：</strong> （可用於專案提醒）當專案狀態為「完成」以外的任何值時，系統會排程傳送提醒通知。</li> 
        <li><strong>完成專案：</strong> （可用於項目提醒）計畫在項目狀態為「完成」時發送提醒通知。</li> 
        <li><strong>開啟工時單：</strong> （可用於時間表提醒）時間表狀態為「開啟」時，將排程發送提醒通知。</li> 
        <li><strong>已提交工時單：</strong> （可用於時間表提醒）提醒通知計畫在提交時間表狀態時發送。</li> 
        <li><strong>未結工時單或每週少於40小時：</strong> （可用於時間表提醒）當時間表狀態為「開啟」或時間表記錄時間少於40小時時，將排程發送提醒通知。</li> 
        <li><strong>電子郵件範本：</strong> 從下拉式清單中，選取要附加至提醒的電子郵件範本。<br>如需如何建立電子郵件範本的資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">設定電子郵件範本</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收件者</td> 
      <td>選取您要接收通知的使用者類型。 從各種對象利害關係方（如所有者、批准者或受託人）中選擇。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。
1. 將提醒通知附加到工作項，如 [將提醒通知附加到對象](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## 接收提醒通知

當附加提醒通知的項目符合條件時，就會觸發電子郵件通知給提醒通知中定義的使用者。

有關接收提醒通知的詳細資訊，請參閱 [提醒通知](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) 區段 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## 測試提醒通知傳送

提醒通知會在每天午夜、山區時間觸發。 所有符合提醒通知資格的物件會在通知完成後不久觸發通知給指定使用者。

若要手動觸發提醒通知，必須先滿足提醒的條件。\
例如，如果將提醒設定為在項目的計畫完成日期後一小時觸發，則該時間必須在設定提醒時和現在之間經過。 任何在啟動提醒之前已傳遞計畫完成日期的項目都不會觸發通知。

若要手動觸發提醒通知：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **診斷** 在Workfront左下角。

1. 按一下 **發送提醒通知** 並等待畫面頂端的確認訊息已傳送。

   提醒通知中指定的使用者會收到電子郵件。
