---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 批准工時單
description: 審批工時單的過程使管理員能夠了解其直接報告的工作時間。 批准者可以驗證記錄的所有時間都已分配到正確的區域，並且該期間記錄了足夠的小時數。
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# 批准工時單

審批工時單的過程使管理員能夠了解其直接報告的工作時間。 批准者可以驗證記錄的所有時間都已分配到正確的區域，並且該期間記錄了足夠的小時數。

Adobe Workfront提供配置時間表批准以支援此區域的功能。

有關提交時間表的資訊，請參閱 [提交時間表以進行批准](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

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
   <td> <p>計劃 </p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫或授權類型，請聯絡您的Workfront管理員。

## 指定工時單批准者

時間表通常由職能管理人員或人力資源人員批准。 （項目經理通常不批准工時單。）

建立工時單配置檔案時定義了工時單審批者。 您必須擁有計畫許可證，才能指定為批准者。

有關指定時間表批准者的詳細資訊，請參閱 [建立或編輯工時單配置檔案](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) 在文章中 [建立、編輯和分配工時單配置檔案](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 批准工時單

您可以批准已提交且已指定為審批人的任何工時單。 提交時間表以進行批准時，時間表將列在 **核准** 區域 **首頁**  頁面。 如需詳細資訊，請參閱 [核准工作](../../review-and-approve-work/manage-approvals/approving-work.md).

如果Workfront管理員啟用了「用戶的工時單批准」和「用戶的工時單拒絕」事件處理程式，則在工時單被批准或拒絕後，將通知您。 如需啟用事件通知的相關資訊，請參閱 [Adobe Workfront中提供的事件通知](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

要批准時間表，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 按一下 **工時單**.
1. 選取 **我的時間表批准** 位於頁面的右上角，僅查看您批准的工時單

   或

   選取 **我的時間表批准** 在時間表清單頂部進行篩選。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >如果您的Workfront管理員或組管理員從「設定」區域的「清單控制項」或「佈局模板」中刪除了「我的時間表批准」篩選器，則「我的時間表批准」選項不會顯示在時間表清單的頂部或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   * [使用版面範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （選用）按一下 **搜尋** 圖示 ![](assets/search-icon.png) 在時間表清單的頂部，鍵入一個關鍵字以查找特定的時間表。 您可以搜尋時間範圍、擁有者或核准者的名稱。
1. 按一下要批准的時間表的時間範圍。 時間表開啟。

   >[!TIP]
   等待批准的工時單的狀態為 [!UICONTROL 已提交].


1. 按一下 **核准**

   或

   如果要拒絕工時單，請按一下 **拒絕** 在工時單的左下角。

   如果已批准，工時單狀態將更改為 **已關閉**.

   如果被拒絕，工時單狀態將更改為 **已拒絕**.
