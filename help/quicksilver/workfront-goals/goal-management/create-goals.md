---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中建立目標
description: 無論您是執行長、經理或個人貢獻者，都可以在Adobe Workfront目標中建立目標，使您的工作與概述組織策略的目標一致。
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 5%

---

# 在Adobe Workfront目標中建立目標

無論您是執行長、經理或個人貢獻者，都可以在Adobe Workfront目標中建立目標，使您的工作與概述組織策略的目標一致。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
<tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> 
   <p>對於新計畫和授權結構：
  <ul><li>Ultimate計畫 </li></ul>
   </p>
<p>對於目前的計畫與授權結構： 
<ul><li> A Pro或更高版本 </li>
  <li>除了Adobe Workfront授權之外，還有Workfront目標授權。</li></ul></p>
   </td> 
  </tr>
  <tr>
 <td role="rowheader">Adobe Workfront授權*</td>
 <td>
 <p>新授權：投稿人或以上版本</p>
 或
 <p>目前授權：要求或以上</p> <p>如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
 <p> 新產品需求，下列其中一項： </p>
<ul>
<li>Select或Prime Adobe Workfront計畫以及額外的Adobe Workfront目標授權。</li>
<li>Ultimate Workfront計畫，預設包含Workfront目標。 </li></ul>
 <p>或</p>
 <p>目前產品需求： Adobe Workfront Goals的Workfront計畫和額外授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
<tr>
<td role="rowheader">存取層級</td>
<td> <p>編輯目標的存取權</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">物件許可權</td>
<td>
<p>檢視目標或更高許可權以檢視它</p>
<p>管理目標的許可權以編輯它</p>
<p>如需共用目標的相關資訊，請參閱<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>。 </p>
</td>
</tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 建立目標的准則

在開始使用Workfront目標之前，我們建議您先閱讀我們對於有效管理目標的最佳實務建議和准則。 如需建立和管理目標之指引的詳細資訊，請參閱[Adobe Workfront目標總覽](../../workfront-goals/goal-management/wf-goals-overview.md)。

## 建立目標

本文說明如何在Workfront目標中建立策略目標。 如需建立業務案例目標的相關資訊，請參閱[建立業務案例目標](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)。

您可以透過下列其中一種方式來建立策略目標：

* [從頭開始建立目標](#create-a-goal-from-scratch)
* [複製現有目標](#copy-an-existing-goal)
* [將結果或活動轉換為目標](#convert-a-result-or-activity-to-a-goal)

### 從頭開始建立目標 {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![Add goal box](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. 按一下右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   目標清單隨即顯示。
1. 按一下&#x200B;**新目標**。

   新目標方塊隨即顯示。

   ![新目標方塊](assets/new-goal-box-unshimmed.png)

1. 在下列欄位中輸入資訊：
   * **目標名稱**：輸入目標的名稱。 這是必填欄位。
   * **期間**：從&#x200B;**期間**&#x200B;下拉式欄位中選取預先定義的季度或年度

     或

     選取&#x200B;**啟用自訂日期**&#x200B;選項，然後為目標選取&#x200B;**開始**&#x200B;和&#x200B;**結束日期**。

     先前年度、目前年度及後續年度及其各自的季度會在「期間」下拉式欄位中列為預先定義的選項。

     目標的期間會指出您預期目標完成的時間範圍。

   * **目標擁有者**：開始輸入使用者、團隊、群組或組織的名稱，以指出誰是目標的擁有者。 系統預設會選取您作為目標的擁有者。
   * **描述**：輸入有關目標的額外資訊。
1. 按一下&#x200B;**建立目標**。

   新目標列在「目標」清單中，其狀態為&#x200B;**草稿**。

   您必須將目標與進度指示器建立關聯，才能啟動並開始處理目標。

   執行下列至少一項作業，準備要啟用的目標：
   * 新增結果

     如需新增結果的詳細資訊，請參閱[在Adobe Workfront目標中新增結果](../results-and-activities/add-results-to-goals.md)。
   * 新增活動

     如需新增活動的相關資訊，請參閱[在Adobe Workfront目標中新增活動](../results-and-activities/add-activities-to-goals.md)。
   * 對齊其他目標

     如需對齊目標的資訊，請參閱[在Adobe Workfront目標中連線來對齊目標](../goal-alignment/align-goals-by-connecting-them.md)。


### 複製現有目標 {#copy-an-existing-goal}

您可以複製現有目標來建立目標。

如需複製目標的相關資訊，請參閱[在Adobe Workfront目標中複製目標](../../workfront-goals/goal-management/copy-goals.md)。

### 將結果或活動轉換為目標 {#convert-a-result-or-activity-to-a-goal}

您可以將現有目標的結果或活動轉換為目標，以建立目標。 新目標會對齊原始目標。

如需有關將結果和活動轉換為目標的資訊，請參閱[將結果和活動轉換為目標以對齊目標](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)。

