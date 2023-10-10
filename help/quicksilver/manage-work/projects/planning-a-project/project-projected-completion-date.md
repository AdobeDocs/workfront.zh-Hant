---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案、任務和問題的預計完成日期總覽
description: 預計完成日期是即時計算的指標，指出專案、任務或問題的完成時間。 當專案、任務或問題標示為「已完成」時，「預計完成日期」會變更為「實際完成日期」的日期。
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# 專案、任務和問題的預計完成日期總覽

預計完成日期是即時計算的指標，指出專案、任務或問題的完成時間。 當專案、任務或問題標示為「已完成」時，「預計完成日期」會變更為「實際完成日期」的日期。

以下小節說明如何決定專案、任務和問題的預計完成日期，以及如何找到它。

## 存取需求

<!--drafted for P&P:

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
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>複查或更高以檢視報告中的預計完成日期</p> <p>建立報告的計畫授權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視或更高專案存取權</p> <p>您必須擁有報告、儀表板、行事曆的編輯存取權，才能建立報告</p> <p>您必須擁有「篩選器」、「檢視」、「群組」的「編輯」存取權，才能建立報告或修改清單檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或更高的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## Adobe Workfront如何決定預計完成日期

「預計完成日期」是計算欄位，無法手動變更。

根據您檢視的物件，用來決定「預計完成日期」的條件會有所不同：

* **專案：** 專案的「預計完成日期」等於專案上最新作業的「預計完成日期」。

  例如，較高的完成百分比會將任務的「預計完成日期」移動至更接近當天。 如果任務的狀態為「新增」，且任務的「計畫完成日期」已關閉或已過，則「預計完成日期」會進一步移向未來。

* **工作：** 作業的「預計完成日期」是根據下列條件所決定：

   * **任務受指派人在任務上進行的進度更新：** 進度更新包括完成百分比的變更及任務狀態的變更。
   * **認可日期：** 如果任務受指派人指定認可日期，則預計完成日期會變更以符合認可日期。

     如需認可日期的詳細資訊，請參閱文章 [認可日期總覽](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **前置任務：** 如果前置任務沒有延遲，「預計完成日期」應該與「計畫完成日期」相符。 發生延遲時，相依任務顯示的「預計完成日期」會晚於「計畫完成日期」。

     有關任務的規劃完成日期的詳細資訊，請參閱 [任務計畫完成日期總覽](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >當任務的前置任務具有實際完成日期時，相依任務會收到如下案例所述的預計完成日期：
  >
  >
  >如果專案具有任務A、任務B和任務C，並且任務B是任務A的後繼任務，任務C是任務B的後繼任務，並且已將實際完成日期新增到任務A，則會自動重新計算任務B的預計完成日期(如果 **更新型別** 專案設定為「自動」與「變更時」)，但不會針對「作業C」重新計算。目前，基於效能原因，Workfront會針對從更新的「作業」往上或往下一個層次的任務，計算「預計完成日期」。 

* **問題：** 「問題預計完成日期」最初設定為與問題「計畫完成日期」相符。

  如果問題受指派人指定認可日期，則預計完成日期和計畫完成日期都會變更以符合認可日期。

  如需認可日期的詳細資訊，請參閱文章 [認可日期總覽](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 檢視預計完成日期

您可以在報告中檢視專案、任務和問題的預計完成日期。 您可以在Workfront的其他區域中檢視專案和任務的預計完成日期。 

* [檢視專案的預計完成日期](#view-the-projected-completion-date-of-a-project)
* [檢視任務的預計完成日期](#view-the-projected-completion-date-of-a-task)
* [檢視問題的預計完成日期](#view-the-projected-completion-date-of-an-issue)

### 檢視專案的預計完成日期 {#view-the-projected-completion-date-of-a-project}

1. 移至您要檢視預計完成日期的專案。
1. 按一下 **專案詳細資訊** 在左側面板中。
1. 找到 **預計完成日期** 中的欄位 **概觀** 區段。

### 檢視任務的預計完成日期 {#view-the-projected-completion-date-of-a-task}

1. 移至您要檢視「預計完成日期」的工作。
1. 按一下 **任務詳細資訊** 在左側面板中。
1. 找到 **預計完成日期** 中的欄位 **概觀** 區段。

### 檢視問題的預計完成日期 {#view-the-projected-completion-date-of-an-issue}

您只能在問題報告或清單檢視中檢視問題的預計完成日期。 建立清單檢視類似於在報告中建立檢視。

若要建立包含預計完成日期的問題報表，請執行下列步驟：

1. 建立問題報告，如文章所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 選取 **欄（檢視）** 標籤。
1. 按一下 **新增欄**，並開始輸入 **預計完成日期** 在 **顯示在此欄：** 欄位。

1. 當它出現在清單中時，在 **問題** 物件。 
1. 按一下 **儲存+關閉**.

   此 **預計完成日期** 欄會填入。 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
