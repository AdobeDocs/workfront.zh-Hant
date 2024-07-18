---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 將活動新增至Adobe Workfront目標中的目標
description: 活動會測量目標的進度。 若無關聯的結果、活動或校準的目標，即無法啟用目標，且無法記錄進度。
author: Alina
feature: Workfront Goals
exl-id: 4d6ef324-4b5c-402b-b64d-b1a2a7d2ab57
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---

# 將活動新增至Adobe Workfront目標中的目標

活動會測量目標的進度。 如果不關聯結果、活動、專案或校準的目標，您就無法啟動目標，也無法記錄其進度。

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
  <ul><li>終極計畫 </li>
  或
  <li>適用於Prime或選取Adobe Workfront計畫的Adobe Workfront目標的其他授權。 </li></ul> </p>
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
<li>預設包含Workfront目標的Ultimate Workfront計畫。 </li></ul>
 <p>或</p>
 <p>目前產品需求： Adobe Workfront Goals的Workfront計畫和額外授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">存取層級*</td>
 <td> <p>編輯目標的存取權</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  <p>如需共用目標的相關資訊，請參閱<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>。 </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先決條件

您必須有現有目標，才能在其中新增活動。

如需建立目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。

>[!IMPORTANT]
>
>一個目標不能有超過1000個活動、結果或校準的目標。

如需活動的詳細資訊，請參閱[開始使用Adobe Workfront目標中的結果和活動](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)。

## 將活動新增至目標

<!--
Adding activities to goals differs depending on which environment you use.

### Add an activity to a goal in the Production environment

1. Go to the goal for which you want to add an activity and click the name to open the **Goal Details** panel.
1. Click **Add activities**.

   ![](assets/add-activity-inside-goal-details-highlighted-350x152.png)

1. From the **Activity Type** drop-down menu, select the type of activity you want to associate with your goal.&nbsp;Select **Manual progress bar** or **Project**. Manual progress bar is the default selection. 
1. (Conditional) Depending on which activity type you selected, do the following:

   1. If you selected **Manual progress bar**:

      1. Start typing a name for your activity in the **Activity** field. 
      1. (Optional) If you want to set the activity owner as someone other than yourself, click your name in the **Owner** field and begin typing the name of the user that you want to assign as the activity owner, then click it when it appears in the drop-down list.

         >[!NOTE]
         >
         >You cannot assign a team or group as an activity owner.

         When you update the progress of an activity, the progress of the goal automatically updates.

   1. If you selected **Project**:

      1. Click the **Connect projects** field.

         Existing projects that you have access to View display in the Connect projects list. Projects that are in a status of Dead do not display in the list. 
      
      1. Click the name of a project to add it as an activity to the goal. You can select several projects at one time.

         Workfront uses the project percent complete of all the attached projects to calculate the progress of the goal.

         For more information about associating projects with goals, see [Add projects to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

         >[!TIP]
         >
         >   
         >   * The owner of the project becomes the owner of this activity. If the project has no owner, then the activity has no owner. 
         >   * You cannot manually update the progress of a project. Workfront calculates the progress of the project based on the project percent complete. When the project percent complete updates in Workfront this also updates the connected project in Workfront Goals including the percent complete of the goal. 
         >   
         >

1. Click **Save**.

   The activity is saved for the selected goal. After you activate the goal, the progress of the goal automatically updates when you update the progress of an activity or when the percent complete of a project updates. For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

-->


1. 按一下&#x200B;**主要功能表** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。
1. 從目標清單中，按一下目標的名稱以開啟目標的頁面。
1. 按一下左側面板中的&#x200B;**進度指示器**。
1. 從[新增進度指示器]下拉式功能表，按一下[建立活動] ****。

   「新增活動」方塊開啟。

   ![](assets/new-activity-box-unshimmed.png)

1. 在活動名稱欄位中輸入活動的名稱。 這是必填欄位。
1. （選擇性）如果要將活動指派給其他使用者，請從&#x200B;**活動擁有者**&#x200B;欄位中移除您的名稱。 依預設，您是您建立之活動的擁有者。

   >[!NOTE]
   >
   >您無法將團隊、群組或公司指派為活動擁有者。

1. 按一下&#x200B;**建立活動**&#x200B;以儲存活動並將其新增至選取的目標。

   活動會顯示在目標頁面的「活動」群組下方的進度指示器區段。





