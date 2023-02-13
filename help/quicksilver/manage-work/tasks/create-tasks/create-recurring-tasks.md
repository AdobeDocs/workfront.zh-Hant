---
product-area: projects
navigation-topic: create-tasks
title: 建立循環任務
description: 您可以為必須在單一專案中重複的工作建立週期性任務。
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# 建立循環任務

您可以為必須在單一專案中重複的工作建立週期性任務。

有關循環任務的一般資訊，包括編輯現有循環任務的影響，請參閱 [循環任務概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 有關訪問任務的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予任務的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為專案貢獻權限，並提供新增工作或更新版本</p> <p>建立任務時，您會自動獲得該任務的「管理」權限</p> <p> 有關任務權限的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共用任務 </a>. </p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立循環任務

>[!NOTE]
>
>無法通過修改現有任務來建立循環任務。 您必須從頭建立任務。

1. 前往您要建立循環任務的專案，然後按一下 **工作** 區段。
1. 按一下 **新任務**.

   將顯示「新任務」對話框。

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. 按一下 **更多選項** 然後在 **任務名稱** 欄位。
1. 繼續以添加新任務時相同的方式更新任務。 有關添加新任務的詳細資訊，請參閱 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)
1. 按一下 **概述** 中。
1. 向下捲動至 **定期計畫** 區段，然後選取 **將此作為循環任務** 選項。

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. 在 **頻率** 下拉清單，選擇您希望任務發生的時間單位數和時間單位類型。 從下列選項中選取：

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
      <td> <p>根據您選取的順序，每天、每2天、每3天等重複此工作。 您可以設定任務，最多每6天重複一次。 預設設定為1天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>工作日</strong> </td> 
      <td> <p> 任務會根據您選取的順序，每個工作日、每2個工作日、每3個工作日等重複。 您可以將任務配置為最多每6個工作日重複一次。</p> <p>此選項使用由系統管理員定義的預設計畫，如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>週</strong> </td> 
      <td> <p> 任務每週、每2週、每3週等重複，具體取決於您選擇的順序。</p> <p>在 <strong>重複</strong> 欄位，選擇您希望每個任務發生的星期。 您可以選取多天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>月</strong> </td> 
      <td> <p>任務每月、每2個月、每3個月等重複，具體取決於您選擇的順序。 您可以選擇1至12個月。 </p> <p>在 <strong>重複</strong> 欄位中，在希望任務發生時從以下選項中選擇：</p> 
       <ul> 
        <li> <p><strong>每個月 &lt;month date=""&gt;</strong> </p> <p>您可以選取1至30天，或選取 <strong>最近</strong>. 例如，您可以選取「每月30日」。 </p> </li> 
        <li> <p><strong>每月 &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>在第一個下拉式功能表中，您可以為當月的一週數選取介於1到4之間的數字，或選取「最後」。 </p> <p>在第二個下拉式功能表中，您可以選取一週中的任一天。 </p> <p>例如，您可以選取「每月2日星期二」。 </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果您有與項目計畫相關聯的計畫例外，則循環任務在例外期間無法啟動。 計畫例外期間發生的循環任務將安排在例外之後的第一個工作日開始。 有關計畫例外的詳細資訊，請參閱文章 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. 在 **開始** 欄位中，選擇要開始循環任務的日期和時間。
1. 在 **結束** 欄位中，選擇要完成循環任務的日期和時間

   或

   選擇 **after `<number>` 發生次數** 指示循環任務應發生的次數。 Workfront會為任務建立與您在此欄位中指定的數目相同的重複次數。

1. 按一下 **建立任務。**

   任務清單隨即顯示。 循環任務建立為父項，所有循環都是其子項。 Workfront會使用您為父代輸入的名稱，後跟數字自動生成子任務的名稱。 有關從父循環任務自動填寫的欄位的詳細資訊，請參閱 [循環任務概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. （可選）修改每個循環任務，就像修改項目中的任何其他任務一樣。

   例如，您可以添加分配、前置任務、持續時間，並修改有關任務的任何其他資訊，包括自定義欄位。

   >[!IMPORTANT]
   >
   >在單獨修改子項之後修改父項週期可能導致子項之間或子項與父項之間的不同資訊。 如需詳細資訊，請參閱 [循環任務概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
