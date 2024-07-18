---
navigation-topic: notifications
title: 自訂事件通知的電子郵件主題
description: 您可以自訂事件通知所觸發之電子郵件的主旨列。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 4%

---

# 自訂事件通知的電子郵件主題

您可以自訂事件通知所觸發之電子郵件的主旨列：

變更主旨行會影響系統中的所有使用者，無論收件者的存取層級為何。 使用者會看到電子郵件主旨中包含的所有物件和欄位。

有些事件通知具有多個主旨行，這表示這些事件通知根據其功能可以有多個電子郵件主旨。

>[!IMPORTANT]
>
>當主旨列參考多個物件時，刪除預設欄位時請務必謹慎。 以下是包含這類主旨行的事件通知清單：
>
>* 有人將我加入定向更新
>* 有人將我的團隊加入定向更新
>* 將工作項目評論發給討論串參與者
>* 將工作項目評論發給受託人
>

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
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>計畫者或以上，具有提醒通知的管理存取權</p> <p>如需有關授與計畫使用者管理存取權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授與使用者對特定區域的管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 自訂事件通知的電子郵件主旨行 {#customize-email-subject-lines-for-event-notifications}

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**電子郵件** > **通知**。

1. 按一下「**事件通知**」標籤。
1. 按一下您要自訂之事件通知的名稱以開啟&#x200B;**事件通知**&#x200B;方塊。
1. 在&#x200B;**電子郵件主旨列**&#x200B;方塊中，變更電子郵件主旨中的文字和欄位，包括自訂欄位。

   新增的欄位名稱必須符合資料庫結構的駝峰式大小寫語法。<!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. 按一下&#x200B;**更新**&#x200B;以儲存您電子郵件的新主旨列。

## 自訂多物件電子郵件的電子郵件主旨行

有些事件通知會根據其觸發的物件而擁有多個主旨列。

例如，「有人將我包含在定向更新中」有兩個不同的主題行：第一個用於任務、問題、範本任務和檔案（也稱為「referenceObject」），第二個用於允許使用者進行評論的物件，例如投資組合、方案等（也稱為「topReferenceObject」）。

![](assets/Ev-not-mult-subj-lines.png)

如果使用者包含在工作、問題、範本工作或檔案的對話中，將產生包含第一個主旨行的電子郵件。 主旨列包含「referenceObject：name」，系統會定義物件並在主旨欄位中顯示適當的名稱。 電子郵件主旨列看起來類似這樣：「對專案ABC上的任務123發表評論」。

如果新增至專案交談，將會產生具有第二個主旨的電子郵件。 在此處，主旨列包含「topReferenceObject：name」，Workfront會再次識別參考的物件，並傳回該物件名稱，而非主旨中的「topReferenceObject：name」。 電子郵件主旨列看起來類似這樣：「對專案ABC發表評論」。

若要編輯電子郵件主旨行並將其他欄位新增至主旨行，請參閱本文中的[自訂事件通知的電子郵件主旨行](#customize-email-subject-lines-for-event-notifications)。

## 自訂多動作電子郵件的電子郵件主旨列

有些事件通知也有多個電子郵件主題，可概述對物件採取的不同動作。

例如，請求將檔案新增至問題中，是可能觸發兩封不同電子郵件的事件：一封用於檔案新增時，另一封用於檔案編輯時。

![](assets/ev-not-mult-subj-lines-diff-actions.png)

若要編輯電子郵件主旨行並將其他欄位新增至主旨行，請參閱本文中的[自訂事件通知的電子郵件主旨行](#customize-email-subject-lines-for-event-notifications)。
