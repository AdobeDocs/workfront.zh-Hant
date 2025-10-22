---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 編輯時程表資訊
description: 作為具有時程表管理存取許可權的使用者，您可以在Adobe Workfront中編輯現有時程表的資訊。 例如，您可以編輯時程表的「擁有者」、「核准者」或時間範圍。
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 1%

---

# 編輯時程表資訊

作為具有時程表管理存取許可權的使用者，您可以在Adobe Workfront中編輯現有時程表的資訊。 例如，您可以編輯時程表的「擁有者」、「核准者」或時間範圍。

您可以編輯單一時程表上的資訊，也可以大量編輯多個時程表。

>[!IMPORTANT]
>
>如果使用者與週期性時程表相關聯，且時程表會自動產生，則您對現有時程表進行的變更不會反映在為未來日期產生的時程表中。 所有自動產生的時程表都會在時程表設定檔中建立設定。 如需詳細資訊，請參閱[建立週期性時程表](../create-and-manage-timesheets/create-timesheet-profiles.md)

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
   <td><p>對時程表的管理存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯時間表

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**時程表**。

   依預設會選取&#x200B;**全部**&#x200B;篩選器，以顯示您有權檢視的所有時程表。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選擇性）按一下&#x200B;**搜尋**&#x200B;圖示![](assets/search-icon.png)並輸入關鍵字及搜尋特定時間表。 例如，您可以搜尋時程表的時間範圍或擁有者名稱。

1. （選用）執行下列任一項作業，更新時程表清單中的篩選器：

   * 選取頁面右上角的&#x200B;**我的時程表核准**，僅檢視您核准的時程表

     或

     選取&#x200B;**我的時程表**&#x200B;以僅檢視您的時程表。

     這會套用我的時程表核准或我的時程表篩選器到時程表清單。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下「篩選」圖示![](assets/filter-nwepng.png)以套用不同的篩選，或建立新的篩選。 如需建立或更新篩選的資訊，請參閱[在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了「我的時程表核准」和「我的時程表」，則「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   >   * [使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （選擇性）按一下&#x200B;**檢視** ![](assets/view-icon.png)或&#x200B;**群組** ![](assets/grouping.png)圖示以套用不同的檢視或群組或建立新的檢視或群組。

   如需有關建立篩選器、檢視或群組的資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選取一或多個時間表，然後按一下時間表清單頂端的&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。
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
      <td>這是時程表的開始日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>結束日期</strong> </td> 
      <td> 這是時程表的結束日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>狀態</strong> </td> 
      <td> 這是時程表的狀態。
      以下為可能的時程表狀態選項： 
      <ul><li><b>開啟</b>：時程表已開啟，可以編輯小時專案。</li>
      <li><b>已提交</b>：已提交時程表以供指定核准者核准。</li>
      <li><b>已拒絕</b>：核准者未核準時程表，現在使用者可再次編輯時間專案。</li>
      <li><b>已關閉</b>：時程表已由使用者關閉或由核准者核准，因此現在已關閉。 您無法將時間新增至已關閉的時程表。</li>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>核准者</strong> </td> 
      <td> <p>核准者指核准與時程表相關聯之使用者之時程表的使用者。 只有對時程表具有管理存取許可權的使用者才能設定為核准者。 </p> <p>如需時程表管理許可權的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取權</a>。</p> <p>開始輸入時程表核准者的名稱，並在他們出現在清單中時選取他們。</p> <p>您可以在時程表上擁有多個核准者。 在這種情況下，在核准者核準時程表後，該時程表會被標籤為<strong>已關閉</strong>，並且會從所有剩餘核准者的時程表核准清單中消失。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>可以編輯時間</strong> </td> 
      <td> <p>如果您希望允許核准者編輯時程表上的小時，請選取此選項。</p> <p>當您選取多個時程表時，此選項不可用。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">加班</span> </td> 
      <td> <p>您可以選擇隱藏時程表上的「加班」方塊。</p> <p>此選項預設為停用。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。
