---
product-area: projects
navigation-topic: create-tasks
title: 建立週期性任務
description: 您可以為必須重複的任務建立週期性任務，作為單一專案的一部分。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# 建立週期性任務

<!--Audited: 01/2024-->

您可以為必須重複的任務建立週期性任務，作為單一專案的一部分。

如需週期性任務的一般資訊，包括編輯現有週期性任務的影響，請參閱[週期性任務概觀](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>為專案貢獻許可權，並可新增任務或以上專案</p> 
   <p>建立任務時，您會自動收到該任務的「管理」許可權</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p> 
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> 
   <p>When you create a task you automatically receive Manage permissions to the task</p> 
   <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator. For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## 建立週期性任務

>[!NOTE]
>
>您無法藉由修改現有任務來建立週期性任務。 您必須從頭開始建立工作。

1. 前往您要建立週期性任務的專案，然後按一下左側面板中的「**任務**」區段。
1. 按一下&#x200B;**新增工作**。

   「新增工作」對話方塊隨即顯示。

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. 按一下&#x200B;**其他選項**，然後在&#x200B;**工作名稱**&#x200B;欄位中輸入工作的名稱。
1. 以新增任務時的相同方式繼續更新任務。 如需新增任務的詳細資訊，請參閱[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

   >[!TIP]
   >
   >   為新週期性任務指定的持續時間和計畫時數是每個事件的持續時間和計畫時數。 父系任務的期間是介於最早任務的「計劃開始日期」與最近任務的「計畫完成日期」之間的時間。 父系任務的計畫時數是所有發生次數的所有計畫時數總計。

1. 按一下左側面板中的&#x200B;**概觀**。
1. 向下捲動至&#x200B;**遞回排程**&#x200B;區段，然後選取&#x200B;**將此工作設為遞回工作**&#x200B;選項。

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. 在&#x200B;**頻率**&#x200B;下拉式清單中，選取您想要工作發生的時間單位數以及時間單位型別。 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>遞迴類型</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>天</strong> </td> 
      <td> <p>任務會每天、每2天、每3天等重複一次，視您選取的步調而定。 您可以將工作設定為每隔6天重複執行一次。 預設值為1天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>工作日</strong> </td> 
      <td> <p> 任務會根據您選取的步調在每個工作日、每2個工作日、每3個工作日等重複。 您可以將工作設定為每隔6個工作日重複執行一次。</p> <p>此選項使用系統管理員定義的預設排程，如<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>中所述。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>周</strong> </td> 
      <td> <p> 任務會每週、每兩週、每三週等重複，視您選取的步調而定。</p> <p>在<strong>重複</strong>欄位中，選取您想要每個工作發生的日期。 您可以選取多天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>個月</strong> </td> 
      <td> <p>根據您選取的步調，任務會每月、每2個月、每3個月等重複。 您可以選取1到12個月。 </p> <p>在<strong>重複</strong>欄位中，當您想要工作發生時，從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>每個月的&lt;month date&gt;</strong>日 </p> <p>您可以選取從1到30的天數，也可以選取<strong>last</strong>。 例如，您可以選取「每月30日」。 </p> </li> 
        <li> <p>每月<strong>的&lt;number&gt; &lt;day of the week&gt;</strong> </p> <p>在第一個下拉式功能表中，您可以選取月份中周數的介於1到4之間的數字，或選取「最後」。 </p> <p>在第二個下拉式功能表中，您可以選取一週的任何一天。 </p> <p>例如，您可以選取「每個月在第2個星期二」。 </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果您有與專案排程相關的「排程例外」，則週期性任務無法在例外期間開始。 排程例外期間發生的週期性作業，會排定在例外之後的第一個營業日開始。 如需排程例外狀況的詳細資訊，請參閱文章[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

1. 在&#x200B;**開始**&#x200B;欄位中，選取您想要開始週期性工作的日期和時間。
1. 在&#x200B;**結束**&#x200B;欄位中，選取您想要完成週期性工作的日期和時間

   或

   選取&#x200B;**次發生`<number>`之後的**，以指出週期性工作應該發生的次數。 Workfront會為任務建立與您在此欄位中指定的數字相同的遞回次數。

1. 按一下&#x200B;**建立任務。**

   工作清單隨即顯示。 遞回任務會建立為父項，而所有遞回任務都是其子項。 Workfront會使用您為父系輸入的名稱（後面接著數字），自動產生子系工作的名稱。 週期性任務會放置在任務清單的末尾。

   如需從父遞回任務自動填寫哪些欄位的詳細資訊，請參閱[遞回任務總覽](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md)。

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. （選用）修改每個週期性任務，就像修改專案中任何其他任務一樣。

   例如，您可以新增工作分派、前置任務、持續時間，以及修改關於任務的任何其他資訊，包括自訂欄位。

   >[!IMPORTANT]
   >
   >在個別修改子項之後，修改父項週期可能會導致子項之間或子項與父項之間產生不同的資訊。 如需詳細資訊，請參閱[週期性工作概觀](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md)。
