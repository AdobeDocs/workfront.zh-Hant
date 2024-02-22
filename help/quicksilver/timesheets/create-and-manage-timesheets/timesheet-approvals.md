---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 核准時間表
description: 核準時程表的程式可讓經理檢視其直接下屬的工作時間。 核准者可確認所有記錄時間均已分配至正確的區域，且期間已記錄足夠的時數。
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# 核准時間表

核準時程表的程式可讓經理檢視其直接下屬的工作時間。 核准者可確認所有記錄時間均已分配至正確的區域，且期間已記錄足夠的時數。

Adobe Workfront提供設定時程表核准的功能，以支援此區域。

如需有關提交時程表的資訊，請參閱 [提交時程表以供核准](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

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
   <td> <p>計劃 </p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

## 指定時程表核准者

時程表通常由功能經理或人力資源人員核准。 （專案經理通常不會核準時程表。）

時程表核准者會在建立時程表設定檔時定義。 您必須擁有計畫授權才能被指定為核准者。

如需有關指定時程表核准者的詳細資訊，請參閱區段 [建立或編輯週期性時程表](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) 在文章中 [建立、編輯和指派週期性時程表](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 核准時間表

若您被指定為核准者，則您可核准任何已提交的時程表。 當時程表提交進行核準時，時程表會列在 **核准** 區域在您的 **首頁**  頁面。 如需詳細資訊，請參閱 [核准工作](../../review-and-approve-work/manage-approvals/approving-work.md).

如果Workfront管理員已啟用「使用者的時程表核准」和「使用者的時程表拒絕」事件處理常式，在核准或拒絕時程表後，您會收到通知。 如需啟用事件通知的詳細資訊，請參閱 [事件通知型別](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

若要核準時程表：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 按一下 **時間表**.
1. 選取 **我的時程表核准** 在頁面的右上角，僅檢視您核准的時程表

   或

   選取 **我的時程表核准** 在時程表清單頂端篩選。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從設定區域的清單控制項或版面配置範本中移除了「我的時程表核准」篩選器，則「我的時程表核准」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   >   * [使用版面配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （可選）按一下 **搜尋** 圖示 ![](assets/search-icon.png) 在時程表清單頂端並輸入關鍵字，以找出特定時程表。 您可以搜尋時間範圍，或搜尋擁有者或核准者的名稱。
1. 按一下您要核準時程表的時間範圍。 時程表隨即開啟。

   >[!TIP]
   >
   >等待核准的時程表狀態為 [!UICONTROL 已提交].


1. 按一下 **核准**

   或

   如果您要拒絕時程表，請按一下 **拒絕** 在時程表的左下角。

   如果核准，時程表狀態會變更為 **已關閉**.

   如果拒絕，時程表狀態會變更為 **已拒絕**.
