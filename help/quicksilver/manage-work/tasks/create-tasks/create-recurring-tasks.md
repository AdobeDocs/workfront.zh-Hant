---
product-area: projects
navigation-topic: create-tasks
title: 建立週期性任務
description: 您可以為必須重複的任務建立週期性任務，作為單一專案的一部分。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# 建立週期性任務

<!--Audited: 01/2024-->

您可以為必須重複的任務建立週期性任務，作為單一專案的一部分。

如需週期性任務的一般資訊，包括編輯現有週期性任務的影響，請參閱 [遞回任務總覽](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準</p> 
   <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務與專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>為專案貢獻許可權，並可新增任務或以上專案</p> 
   <p>建立任務時，您會自動收到該任務的「管理」許可權</p> 
   <p> 如需工作許可權的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共用任務 </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需存取需求的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 建立週期性任務

>[!NOTE]
>
>您無法藉由修改現有任務來建立週期性任務。 您必須從頭開始建立工作。

1. 前往您要建立週期性任務的專案，然後按一下 **任務** 區段。
1. 按一下 **建立任務**.

   「新增工作」對話方塊隨即顯示。

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. 按一下 **更多選項** 然後，在 **任務名稱** 欄位。
1. 以新增任務時的相同方式繼續更新任務。 如需新增工作的詳細資訊，請參閱 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   為新週期性任務指定的持續時間和計畫時數是每個事件的持續時間和計畫時數。 父系任務的期間是介於最早任務的「計劃開始日期」與最近任務的「計畫完成日期」之間的時間。 父系任務的計畫時數是所有發生次數的所有計畫時數總計。

1. 按一下 **概觀** 在左側面板中。
1. 向下捲動至 **遞回排程** 區段，然後選取 **將此設為遞回任務** 選項。

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. 在 **頻率** 下拉式清單，選取您想要執行工作時的時間單位數以及時間單位型別。 從下列選項中選取：

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
      <td role="rowheader"><strong>日</strong> </td> 
      <td> <p>任務會每天、每2天、每3天等重複一次，視您選取的步調而定。 您可以將工作設定為每隔6天重複執行一次。 預設值為1天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>工作日</strong> </td> 
      <td> <p> 任務會根據您選取的步調在每個工作日、每2個工作日、每3個工作日等重複。 您可以將工作設定為每隔6個工作日重複執行一次。</p> <p>此選項使用系統管理員定義的預設排程，如中所述 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>周</strong> </td> 
      <td> <p> 任務會每週、每兩週、每三週等重複，視您選取的步調而定。</p> <p>在 <strong>重複</strong> 欄位中，選取一週中您想要每個任務發生的日期。 您可以選取多天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>月</strong> </td> 
      <td> <p>根據您選取的步調，任務會每月、每2個月、每3個月等重複。 您可以選取1到12個月。 </p> <p>在 <strong>重複</strong> 欄位中，當您想要進行工作時，從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>每個月的第天 &lt;month date=""&gt;</strong> </p> <p>您可以從1到30選取天數，也可以選取 <strong>上次</strong>. 例如，您可以選取「每月30日」。 </p> </li> 
        <li> <p><strong>每個月的 &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>在第一個下拉式功能表中，您可以選取月份中周數的介於1到4之間的數字，或選取「最後」。 </p> <p>在第二個下拉式功能表中，您可以選取一週的任何一天。 </p> <p>例如，您可以選取「每個月在第2個星期二」。 </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果您有與專案排程相關的「排程例外」，則週期性任務無法在例外期間開始。 排程例外期間發生的週期性作業，會排定在例外之後的第一個營業日開始。 如需排程例外的詳細資訊，請參閱文章 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. 在 **開始** 欄位中，選取您想要循環任務開始的日期和時間。
1. 在 **結束** 欄位，選取您想要完成週期性任務的日期和時間

   或

   選取 **晚於 `<number>` 發生次數** 以指出週期性任務應該發生的次數。 Workfront會為任務建立與您在此欄位中指定的數字相同的遞回次數。

1. 按一下 **建立任務。**

   工作清單隨即顯示。 遞回任務會建立為父項，而所有遞回任務都是其子項。 Workfront會使用您為父系輸入的名稱（後面接著數字），自動產生子系工作的名稱。 週期性任務會放置在任務清單的末尾。

   如需有關從父遞回任務自動填寫哪些欄位的詳細資訊，請參閱 [遞回任務總覽](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. （選用）修改每個週期性任務，就像修改專案中任何其他任務一樣。

   例如，您可以新增工作分派、前置任務、持續時間，以及修改關於任務的任何其他資訊，包括自訂欄位。

   >[!IMPORTANT]
   >
   >在個別修改子項之後，修改父項週期可能會導致子項之間或子項與父項之間產生不同的資訊。 如需詳細資訊，請參閱 [遞回任務總覽](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
