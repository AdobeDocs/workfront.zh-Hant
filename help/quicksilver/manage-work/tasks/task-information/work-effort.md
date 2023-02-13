---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 工作成果概觀
description: 工作成果概觀
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# 工作成果概觀

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more) </p>
-->

作為項目經理，您可以決定要如何估計項目中完成任務所需的工作量。 使用以下指標之一估計完成任務所需的工作量：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">計畫小時</td> 
   <td> <p> 手動輸入數值或Adobe Workfront計算，顯示分配給任務的資源完成該任務所需的小時數。 </p> <p>請考慮下列「計畫小時數」： </p> 
    <ul> 
     <li>這是預設方法。 </li> 
     <li>只有持續時間類型為「計算分配」或「簡單」的任務，您才能手動更新「計畫小時數」。 </li> 
    </ul> <p>如需「計畫小時數」的相關資訊，請參閱 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">計畫小時數概觀</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">工作量 </td> 
   <td> <p>一種手動標籤，定義用戶完成任務是否需要每天的小量、中量或大量工作。 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>請考量下列工作成果：</p> 
    <ul> 
     <li>此欄位僅適用於具有簡單持續時間類型的任務。 </li> 
     <li>您可以啟用此標籤的使用，並定義與其在專案層級相關聯的工作時間百分比。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

本文說明何謂「工作量」，以及在估計任務的工作量時應如何使用它。

>[!NOTE]
>
>「計畫小時數」和「工作量」相互影響。 更新計畫小時數可以更新工作量，而更新工作量可以更新任務的計畫小時數。

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案和工作的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案及其工作的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 使用工作量的考量事項

* 如果項目任務具有0個計畫小時，並且您啟用了「使用工作」以自動計算項目上的任務「計畫小時數」設定，則與它們關聯的預設工作級別將為「中」。 計畫小時數會自動更新為「簡單持續時間類型」任務。 如需詳細資訊，請參閱  [工作量](#levels-of-work-effort) 這篇文章。
* 如果項目任務的「計畫小時數」超過0，並且您啟用了「使用工作」以自動計算項目上的任務「計畫小時數」設定，則「工作」層將根據「計畫小時數」量更新，而不會更改「簡單持續時間類型」任務的「計畫小時數」量。 如需詳細資訊，請參閱 [Workfront如何根據計畫小時計算工作量](#how-workfront-calculates-work-effort-based-on-planned-hours) 這篇文章。
* 如果項目任務具有0個計畫小時，並且您啟用了「使用工作」以自動計算項目上的任務計畫小時數設定，然後將「工作」級別從「中」更新為「小」或「大」，則「計畫小時數」也會更新。 如需詳細資訊，請參閱 [Workfront如何根據工作量計算計畫小時數](#how-workfront-calculates-planned-hours-based-on-work-effort) 這篇文章。
* 當您內嵌編輯任務並同時修改任務的「計畫時數」和「工作精力」欄位時，「計畫時數」將用您指定的值更新，而「工作精力」值則根據您更新的「計畫時數」計算。
* 更新任務的「工作量」值時，「持續時間」不再根據「計畫小時數」自動計算。 有關如何計算簡單持續時間任務的持續時間的詳細資訊，請參閱 [持續時間類型概觀：簡單](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* 將任務的「持續時間類型」從「簡單」更改為任何其他類型時，「工作工作」欄位將隱藏在任務上。 計畫小時數保持不變。
* 無法更新父任務的「工作」級別。 系統會根據任務的計畫小時數自動計算父任務的「工作量」級別，該小時數是所有子任務的匯總。 有關父任務的資訊，請參閱 [建立子任務](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## 啟用使用工作量而非計畫小時數

1. 前往專案，然後按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯**.
1. 按一下 **任務設定**，然後選取選項&#x200B;**使用工作量自動計算任務計畫小時數**. 預設會取消選取此選項。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   如需在專案上啟用工作成果的詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md) 文章。

1. 按一下 **工作** 在左側面板上，按一下要存取之任務的名稱。
1. 按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯**. 確保任務具有「簡單持續時間類型」。

   >[!TIP]
   >
   >您也可以在「任務詳細資訊」部分中更新任務的「工作量」。

1. 在 **概述** 區域中，按一下「工作成果」下拉菜單以更正完成任務所需的工作量。

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   有關更新任務的「工作成果」欄位的詳細資訊，請參閱以下文章：

   * 此 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md) 文章
   * [在「任務詳細資訊概覽」區域中管理任務資訊](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## 工作量 {#levels-of-work-effort}

身為專案經理，您可以為專案找出三個層級的「工作量」。 每個工作層級相當於使用者完成工作所需的每日時間百分比。

設定工作精力等級時，您必須自問：「分配給此任務的用戶每天應花費多少時間完成該任務？」 

下表說明工作量的可能級別及其預設對應百分比。 身為專案經理，您可以更新百分比以符合組織的需求。 編輯專案時即可執行此動作。 如需編輯專案的相關資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

您是Workfront管理員，可在「設定」的「專案偏好設定」區域中定義每個工作日的典型小時數。 這是被視為工作時間的每日時間量。 如需為Workfront執行個體設定專案偏好設定的相關資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>在下列範例中，我們假設Workfront管理員已將每個工作日的典型小時數設為8小時。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>工作量</td> 
   <td>百分比值</td> 
  </tr> 
  <tr> 
   <td>小 </td> 
   <td>完成任務所需的小量工作量設定為每天典型小時數的25%。 這表示指派此工作層級的任務一天最多需要2小時，才能在一天內完成。 <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>中</td> 
   <td> <p>完成任務的中度工作量設定為每工作日典型小時數的50%。 這表示指派此工作層級的任務在一天內應需要超過2小時且少於6小時才能完成。 <code>(0.50*80=4)</code> </p> <p>注意：在項目上啟用了「使用工作量自動計算任務計畫小時數」設定時，如果任務在啟用此設定之前具有0個計畫小時數，則此設定為任務的預設設定。 這會使「計畫小時數」任務更新為4小時。 </p> </td> 
  </tr> 
  <tr> 
   <td>大</td> 
   <td>完成任務的工作量設定為每個工作日典型小時數的75%。 這表示指派此工作層級的任務應花費6小時或更長時間，才能在一天內完成。 <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何根據工作量計算計畫小時數 {#how-workfront-calculates-planned-hours-based-on-work-effort}

當您啟用「使用工作量」以自動計算項目上的任務「計畫小時數」設定時，Workfront會使用以下公式計算具有「簡單持續時間類型」的任務的「計畫小時數」：

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

例如，持續時間為3天、工作量為中的任務有12個計畫小時：

```
Planned Hours = 3*4=12
```

其中，每個工作日的典型小時數值為8小時。

>[!TIP]
>
>將任務分配給多個資源時，計畫小時數將平均分配給任務持續時間的每一天的每個資源。

## Workfront如何根據計畫小時計算工作量 {#how-workfront-calculates-work-effort-based-on-planned-hours}

如果啟用「使用工作量」以自動計算項目上的任務「計畫小時數」設定，並且任務上已經有「計畫小時數」，或者編輯任務上的「計畫小時數」，Workfront將更新「工作量」值。

Workfront使用下列公式根據計畫小時更新工作量級別：

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

例如，如果您的任務的持續時間為2天，並且您將計畫小時數從8小時更新為20小時，則任務的工作量將從中更新為大：

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## 查找任務和項目的工作

* [專案的工作成果](#work-effort-for-projects)
* [任務的工作量](#work-effort-for-tasks)

### 專案的工作成果 {#work-effort-for-projects}

您可以在以下區域找到專案的「工作量」區段：

* 「編輯項目」框中的「任務設定」區域

### 任務的工作量 {#work-effort-for-tasks}

您可以在以下區域找到任務的「工作成果」欄位：

* 「編輯任務」框中的「概述」區域
* 「工作時間」區域中「任務詳細資訊」部分的「概覽」區域
* 任務清單或報告
