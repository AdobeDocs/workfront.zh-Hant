---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 工作投入概觀
description: 工作投入概觀
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 0%

---

# 工作投入概觀

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

身為專案經理，您可以決定如何估計要在專案中完成任務所需的工作量。 使用下列其中一個指標，估計完成工作所需的工時量：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">規劃時數</td> 
   <td> <p> 手動數值輸入或Adobe Workfront計算，顯示指派給任務的資源完成所需的時數。 </p> <p>考量下列有關計畫時數的資訊： </p> 
    <ul> 
     <li>這是預設方法。 </li> 
     <li>您只能為「期間型別」為「已計算的任務指派」或「簡單」的任務手動更新計畫時數。 </li> 
    </ul> <p>如需計畫時數的詳細資訊，請參閱<a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">計畫時數總覽</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">工作投入 </td> 
   <td> <p>手動標籤，定義使用者需要少量、中量或大量的日常工作才能完成任務。<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>請考量下列有關工作投入的內容：</p> 
    <ul> 
     <li>此欄位僅適用於具有簡單期間型別的任務。 </li> 
     <li>您可以啟用此標籤的使用並在專案層級定義與其關聯的工作時間百分比。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

本文說明什麼是工作量，以及您在估計任務的工作量時應該如何使用它。

>[!NOTE]
>
>計畫時數與工作量會相互影響。 更新計畫時數可以更新工作量，更新工作量可以更新任務的計畫時數。

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
   <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案和任務的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案及其任務的許可權</p>  </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current: Plan </p>
   Or
   <p>New: Standard </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project and its tasks</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 使用工作量時的注意事項

* 當專案任務具有0個計畫時數，並且您啟用使用工作量自動計算專案上的任務計畫時數設定時，與他們相關聯的工作量的預設層級將為Medium。 計畫時數會自動更新簡易期間型別的任務。 如需詳細資訊，請參閱本文章的[工作量層級](#levels-of-work-effort)一節。
* 當專案任務的計畫時數超過0且您啟用使用工作量自動計算專案上的任務計畫時數設定時，工作量層級會根據計畫時數的量進行更新，而不會變更簡單期間型別任務的計畫時數量。 如需詳細資訊，請參閱本文中的[Workfront如何根據計畫時數計算工作量](#how-workfront-calculates-work-effort-based-on-planned-hours)一節。
* 當專案任務具有0個計畫時數，並且您啟用使用工作量以自動計算專案上的任務計畫時數設定，然後將工作量層級從Medium更新為小或大，計畫時數也會更新。 如需詳細資訊，請參閱本文中的[Workfront如何根據工作量計算計畫時數](#how-workfront-calculates-planned-hours-based-on-work-effort)一節。
* 當您內聯編輯任務並同時修改任務的計畫時數和工作投入欄位時，計畫時數將使用您指定的值更新，而工作投入值是根據您更新的計畫時數計算。
* 當您更新任務的工作量值時，「工期」不再根據計畫時數自動計算。 如需如何計算簡易期間工作的期間詳細資訊，請參閱[期間型別概觀：簡單](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)。
* 當您將任務的「期間型別」從「簡單」變更為任何其他型別時，「工作量」欄位會隱藏在任務上。 計畫時數保持不變。
* 您無法更新父系任務的工作量層級。 系統會根據任務的「計畫時數」（所有子系任務的累計），自動計算父系任務的「工作量」層級。 如需父系工作的相關資訊，請參閱[建立子工作](../../../manage-work/tasks/create-tasks/create-subtasks.md)。

## 啟用使用工作量而非計畫時數

1. 前往專案，按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**編輯**。
1. 按一下&#x200B;**工作設定**，然後選取選項&#x200B;**使用工作量自動計算工作計畫時數**。 預設會取消選取此選項。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   如需有關啟用專案上工作投入的詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)文章中的「任務設定」一節。

1. 按一下左側面板上的&#x200B;**任務**，然後按一下任務的名稱以存取它。
1. 按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**編輯**。 確保任務具有簡單期間型別。

   >[!TIP]
   >
   >您也可以更新任務詳細資訊區段中任務的工作量。

1. 在&#x200B;**總覽**&#x200B;區域中，按一下工作量下拉式功能表，以更正完成工作所需的工作量大小。

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   如需有關更新任務的「工作量」欄位的詳細資訊，請參閱下列文章：

   * [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)文章中的「概觀」區段
   * [在任務詳細資訊總覽區域中管理任務資訊](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## 工作量等級 {#levels-of-work-effort}

身為專案經理，您可以為您的專案識別三個層級的工作量。 每個工作量層級相當於使用者完成任務所需每日時間的百分比。

在設定工作量層級時，您必須問自己以下問題：「指派給此任務的使用者每天應該花費多少時間才能按時完成它？」

下表說明可能的工作投入層次及其預設的對應百分比。 身為專案經理，您可以更新百分比以符合組織的需求。 您可在編輯專案時執行此操作。 如需有關編輯專案的資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

作為Workfront管理員，您可以在「設定」的「專案偏好設定」區域中定義每工作日的典型小時數。 這是視為工作時間的每日時間量。 如需有關為您的Workfront執行個體設定專案偏好設定的資訊，請參閱[設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

>[!NOTE]
>
>在以下範例中，我們假設Workfront管理員已將每工作日一般時數設定為8小時。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>工作量等級</td> 
   <td>百分比值</td> 
  </tr> 
  <tr> 
   <td>小 </td> 
   <td>將完成一項任務所需的工作量設定為每日一般時數的25%。 這表示指派此層級工作投入的任務應在一天內最多需要2小時才能完成。 <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>媒體</td> 
   <td> <p>Medium完成任務的投入程度設定為每工作日一般時數的50%。 這表示指派此層級的工作量在一天內應該需要超過2小時且少於6小時來完成。<code>(0.50*80=4)</code> </p> <p>備註：當專案上啟用使用工作量自動計算任務計畫時數設定時，如果任務在啟用此設定之前有0個計畫時數，則此為任務的預設設定。 這會導致任務計畫時數更新為4小時。 </p> </td> 
  </tr> 
  <tr> 
   <td>大</td> 
   <td>完成一項任務所需的大量工作量，被設定為每工作日一般時數的75%。 這表示指派此層級的工作量任務應需要6小時或更多才能在一天內完成。 <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何根據工作量計算計畫時數 {#how-workfront-calculates-planned-hours-based-on-work-effort}

當您啟用使用工作量自動計算專案上的任務計畫時數設定時，Workfront會使用下列公式計算具有簡單期間型別之任務的計畫時數：

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

例如，持續時間為3天且Medium正在努力的任務有12個計畫時數：

```
Planned Hours = 3*4=12
```

其中每工作日一般時數值為8小時。

>[!TIP]
>
>當任務被指派給多個資源時，計畫時數會平均分配給每個資源任務持續時間的每一天。

## Workfront如何根據計畫時數計算工作量 {#how-workfront-calculates-work-effort-based-on-planned-hours}

當您啟用使用工作量自動計算專案上的任務計畫時數設定，且您已擁有該任務的計畫時數或編輯該任務的計畫時數時，Workfront會更新工作量值。

Workfront會使用以下公式，根據計畫時數更新工作量層級：

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

例如，如果您的任務具有2天的工期，而您將計畫時數從8小時更新為20小時，則該任務的工作量會從Medium更新為大型：

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## 找到任務和專案的工作量

* 專案的[工作量](#work-effort-for-projects)
* [任務的工作量](#work-effort-for-tasks)

### 專案的工作量 {#work-effort-for-projects}

您可以在下列區域找到專案上的「工作量」區段：

* 「編輯專案」方塊中的「任務設定」區域

### 任務的工作量 {#work-effort-for-tasks}

您可以在下列區域中找到任務的「工作量」欄位：

* 「編輯任務」方塊中的「概述」區域
* 「工作時間」區域中「工作詳細資訊」區段的「總覽」區域
* 任務清單或報告
