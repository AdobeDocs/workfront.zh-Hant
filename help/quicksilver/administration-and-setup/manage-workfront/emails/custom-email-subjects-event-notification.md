---
navigation-topic: notifications
title: 自訂事件通知的電子郵件主題
description: 您可以自訂事件通知所觸發之電子郵件的主旨行。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 4%

---

# 自訂事件通知的電子郵件主題

您可以自訂事件通知所觸發之電子郵件的主旨行：

變更主旨行會影響系統中的所有使用者，無論收件者的存取層級為何。 使用者可看見電子郵件主旨中包含的所有物件和欄位。

有些事件通知有多個主旨行，這表示這些事件通知可以根據功能有多個電子郵件主旨。

>[!IMPORTANT]
>
>刪除預設欄位時請小心，以備主題行引用多個對象時使用。 以下是包含此類主旨行的事件通知清單：
>
>* 有人將我加入定向更新
>* 有人將我的團隊加入定向更新
>* 執行緒參與者的工作項目註解
>* 給工作項目受指派人的工作項目註解
>


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

## 自訂事件通知的電子郵件主旨行 {#customize-email-subject-lines-for-event-notifications}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **電子郵件** > **通知**.

1. 按一下 **事件通知** 標籤。
1. 按一下您要自訂的事件通知名稱，以開啟 **事件通知** 框。
1. 在 **電子郵件主旨行** 框中，更改電子郵件主題中的文本和欄位，包括自定義欄位。

   新增的欄位名稱必須符合資料庫結構的駝峰式大小寫語法。 <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. 按一下 **更新** 儲存電子郵件的新主旨行。

## 自訂多物件電子郵件的電子郵件主旨行

某些事件通知有多個主旨行，視其觸發的物件而定。

例如，「有人將我納入定向更新」有兩個不同的主題行：第一種是任務、問題、模板任務和文檔（也稱為「referenceObject」），第二種是允許用戶進行注釋的對象，如產品組合、程式等（也稱為「topReferenceObject」）。

![](assets/Ev-not-mult-subj-lines.png)

如果在有關任務、問題、模板任務或文檔的對話中包括用戶，則將使用第一主題行生成電子郵件。 主旨行包含「referenceObject:name」，系統會定義物件，並在主旨欄位中顯示適當的名稱。 電子郵件主旨行看起來類似這樣：「對ABC項目任務123的評論。」

如果新增至專案對話，則會產生與第二個主旨的電子郵件。 在此，主旨行包含「topReferenceObject:name」，並再次指出Workfront識別已參考哪個物件，且會傳回該物件名稱，而非主旨中的「topReferenceObject:name」。 電子郵件主旨行看起來類似這樣：「對ABC項目的評論」

若要編輯電子郵件主旨行並將其他欄位新增至任一主旨行，請參閱 [自訂事件通知的電子郵件主旨行](#customize-email-subject-lines-for-event-notifications) 這篇文章。

## 自訂多動作電子郵件的電子郵件主旨行

某些事件通知也具有多個電子郵件主體，以概述對物件採取的不同動作。

例如，請求將檔案新增至問題是可觸發兩封不同電子郵件的事件：一個用於添加文檔的時間，一個用於編輯文檔的時間。

![](assets/ev-not-mult-subj-lines-diff-actions.png)

若要編輯電子郵件主旨行並將其他欄位新增至任一主旨行，請參閱 [自訂事件通知的電子郵件主旨行](#customize-email-subject-lines-for-event-notifications) 這篇文章。
