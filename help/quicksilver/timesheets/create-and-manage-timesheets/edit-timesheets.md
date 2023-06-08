---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 編輯時程表資訊
description: 作為具有時程表管理存取許可權的使用者，您可以在Adobe Workfront中編輯現有時程表的資訊。 例如，您可以編輯擁有者、核准者或時程表的時間範圍。
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 2%

---

# 編輯時程表資訊

作為具有時程表管理存取許可權的使用者，您可以在Adobe Workfront中編輯現有時程表的資訊。 例如，您可以編輯擁有者、核准者或時程表的時間範圍。

您可以編輯單一時間表上的資訊，也可以大量編輯多個時間表。

>[!IMPORTANT]
>
>如果使用者與時程表設定檔相關聯，並且時程表是自動產生的，則您對現有時程表所做的變更不會反映在針對未來日期產生的時程表中。 所有自動產生的時程表都會在時程表設定檔中建立設定。 如需詳細資訊，請參閱 [建立週期性時程表](../create-and-manage-timesheets/create-timesheet-profiles.md)


## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須擁有時程表的管理存取權。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取權</a>.</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 編輯時間表

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **時間表**.

   此 **全部** 依預設，會選取篩選條件，以顯示您有權檢視的所有時程表。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （可選）按一下 **搜尋** 圖示 ![](assets/search-icon.png) 和輸入關鍵字並搜尋特定時程表。 例如，您可以搜尋時程表時間範圍或擁有者名稱。

1. （可選）執行下列任一項作業，以更新時程表清單中的篩選器：

   * 選取 **我的時程表核准** 位於頁面的右上角，僅檢視您核准的時程表

     或

     選取 **我的時間表** 以僅檢視您的時程表。

     這會將「我的時程表核准」或「我的時程表」篩選器套用至時程表清單。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下篩選圖示 ![](assets/filter-nwepng.png) 以套用不同的篩選器，或建立新的篩選器。 如需建立或更新篩選器的相關資訊，請參閱 [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了「我的時程表核准」和「我的時程表」篩選器，則「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單或篩選器清單的頂端。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   * [使用版面配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （可選）按一下&#x200B;**檢視** ![](assets/view-icon.png) 或 **分組** ![](assets/grouping.png) 圖示可套用不同的檢視或群組，或是建立新的檢視或群組。

   如需建立篩選器、檢視或群組的相關資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選取一或多個時程表，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png) 位於時程表清單頂端。
1. 檢視或指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>所有者</strong> </td> 
      <td> <p>這是為其建立時程表的使用者名稱。 您無法編輯此欄位。 </p> <p>當您選取多個時程表時，該欄位未顯示。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>開始日期</strong> </td> 
      <td>這是時間表開始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>結束日期</strong> </td> 
      <td> 這是時程表的結束日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>核准者</strong> </td> 
      <td> <p>核准者是核准與時程表相關聯之使用者之時程表的使用者。 只有對時程表具有管理存取許可權的使用者才能設定為核准者。 </p> <p>如需時程表管理許可權的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取權</a>.</p> <p>開始輸入時程表核准者的名稱，並在他們出現在清單中時選取他們。</p> <p>您在一個時程表上可以有多個核准者。 在此情況下，當核准者核準時程表後，該時程表會標籤為 <strong>已關閉</strong> 並且它會從所有剩餘核准者的時程表核准清單中消失。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可編輯時間</strong> </td> 
      <td> <p>如果您想要允許核准者編輯時程表上的時數，請選取此選項。</p> <p>當您選取多個時程表時，此選項不可用。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td> <p>您可以選擇隱藏時程表上的「加班」方塊。</p> <p>此選項預設為停用。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下儲存。
