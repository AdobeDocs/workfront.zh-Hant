---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 核准時間表
description: 核準時程表的程式可讓經理檢視其直接下屬的工作時間。 核准者可確認所有記錄時間均已分配至正確的區域，且期間已記錄足夠的時數。
author: Lisa
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# 核准時間表

<!--Audited: 8/2024-->

核準時程表的程式可讓經理檢視其直接下屬的工作時間。 核准者可確認所有記錄時間均已分配至正確的區域，且期間已記錄足夠的時數。

Adobe Workfront提供設定時程表核准的功能，以支援此區域。

如需有關提交時程表的資訊，請參閱[提交時程表以供核准](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td><p>對時程表和時數的管理存取</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 指定時程表核准者

時程表通常由功能經理或人力資源人員核准。 專案經理通常不會核準時程表。 專案經理可核准登入專案的時間，但團隊或人力資源經理應核準時程表。

時程表核准者會在建立時程表設定檔時定義。 您必須擁有計畫授權才能被指定為核准者。

如需指定時程表核准者的詳細資訊，請參閱文章[建立、編輯和指派時程表設定檔](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create)中的[建立或編輯時程表設定檔](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)小節。

## 核准時間表

若您被指定為核准者，則您可核准任何已提交的時程表。 在提交時程表以供核準時，該時程表會列在您&#x200B;**首頁**&#x200B;區域的&#x200B;**我的核准** Widget中。 如需詳細資訊，請參閱[核准工作](../../review-and-approve-work/manage-approvals/approving-work.md)。

如果已設定下列通知設定，則提交時程表以供核准的使用者會在時程表核准後收到電子郵件：

* Workfront管理員已啟用「使用者的時程表核准」和「使用者事件處理常式的時程表拒絕」 。 如需啟用事件通知的詳細資訊，請參閱[事件通知型別](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。
* 在使用者的設定檔頁面上啟用「我的時程表已核准」個人通知。 如需詳細資訊，請參閱[修改您自己的電子郵件通知](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

### 從時程表區域核準時程表

{{step1-to-timesheets}}

**時程表**&#x200B;區域隨即開啟。

1. （視條件而定）如果您上次存取的時間已開啟，請按一下畫面左上角的&#x200B;**回到時程表**。

1. 選取頁面右上角的&#x200B;**我的時程表核准**，僅檢視您核准的時程表

   或

   在時程表清單頂端選取&#x200B;**我的時程表核准**&#x200B;篩選器。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從設定區域的清單控制項或版面配置範本中移除了「我的時程表核准」篩選器，則「我的時程表核准」選項不會顯示在時程表清單頂端或篩選器清單中。
   >
   >如需詳細資訊，請參閱[使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （選擇性）按一下時程表清單頂端的&#x200B;**搜尋**&#x200B;圖示![](assets/search-icon.png)，然後輸入關鍵字以尋找特定時程表。 您可以搜尋時間範圍，或搜尋擁有者或核准者的名稱。
1. 按一下您要核準時程表的時間範圍。 時程表隨即開啟。

   >[!TIP]
   >
   >等待核准的時程表狀態為[!UICONTROL 已提交]。


1. 按一下&#x200B;**核准**

   或

   若要拒絕時程表，請按一下時程表左下角的&#x200B;**拒絕**。

   如果核准，時程表狀態會變更為&#x200B;**已關閉**。

   如果拒絕，時程表狀態會變更為&#x200B;**已拒絕**。

### 核准來自首頁區域的時程表

{{step1-to-home}}

「首頁」區域隨即開啟。

1. 確保您已將&#x200B;**我的核准** Widget新增到您的首頁區域。 如需詳細資訊，請參閱新首頁[中的](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)新增、編輯或移除Widget。
1. 在我的核准Widget中尋找時程表核准。
1. （選擇性）展開[核准]或[拒絕]按鈕右側的下拉式功能表，新增有關您決定的註解，然後按一下[新增]。****
1. 按一下下列其中一個按鈕，即可做出核准決定：

   * 核准
   * 拒絕

   核准已從&#x200B;**我的核准** Widget中移除。


