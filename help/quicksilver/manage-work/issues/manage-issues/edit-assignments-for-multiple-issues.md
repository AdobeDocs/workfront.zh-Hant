---
product-area: projects
navigation-topic: manage-issues
title: 修改清單中多個問題的使用者指派
description: 修改清單中多個問題的使用者指派
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

# 修改清單中多個問題的使用者指派

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

您可以同時修改多個問題的使用者指派。 如需有關編輯問題或一次指派一個問題的資訊，另請參閱下列文章：

* [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md)
* [指派問題](../../../manage-work/issues/manage-issues/assign-issues.md)

如需指派問題的一般資訊，請參閱[修改問題指派的概觀](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)。

>[!NOTE]
>
>您必須至少擁有問題的「貢獻者」許可權，才能為問題指派作業。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯問題的存取權</p> <p>檢視專案和任務的或更高存取權以指派一個問題</p> </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>管理問題的許可權</p> <p>指派多個問題時，為問題所在的專案或任務貢獻許可權或以上。</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 修改多個問題的指派

1. 前往問題清單，其中包含您要修改其指派的問題。
1. （選用）建立篩選器，只顯示指派給您要修改之受指派人的問題。

   例如，您可以建立篩選器，以僅顯示與作為受託人的特定角色有關的問題。  然後，您可以使用特定使用者來取代角色。 請執行下列動作：

   1. 按一下&#x200B;**篩選器**&#x200B;下拉式清單，然後按一下&#x200B;**新增篩選器**。

   1. 在第一個欄位中，開始輸入&#x200B;**指派角色**，然後從清單中選擇&#x200B;**指派角色：名稱**。
   1. 從修飾元下拉式功能表中選取&#x200B;**是**&#x200B;的任一項，然後開始輸入角色的名稱，並在角色顯示在清單中時選取角色。 您可以輸入多個角色。

      >[!TIP]
      >
      >請勿使用&#x200B;**指派給**，因為此欄位僅參考問題擁有者，而非所有受指派人。

      問題清單會自動根據您的篩選條件進行篩選。
   1. （選擇性）按一下&#x200B;**另存新檔**，然後按&#x200B;**儲存**。

1. 選取您要修改指派的問題，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/qs-edit-icon.png)。

   **編輯問題**&#x200B;隨即顯示。 所選的專案數會顯示在頁面的左上角。

1. 按一下左側面板中的&#x200B;**工作**，然後按一下您要移除的工作負責人旁的&#x200B;**x**&#x200B;圖示。

   >[!TIP]
   >
   >只有已指派給所有選定問題的受指派者才會顯示在&#x200B;**工作分派**&#x200B;區域中。

   ![大量編輯問題中的指派區域](assets/assignments-area-on-bulk-edit-issues.png)

1. 開始輸入使用者、角色或團隊的名稱，以將受指派人新增到所有選取的問題。

   >[!TIP]
   >
   >您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
   >
   >* 將工作專案重新指派給作用中的資源。
   >* 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。

   新增的受指派人會新增至現有受指派人。 它們不會取代每個所選問題的現有問題。

1. （選擇性）按一下&#x200B;**指派給我**&#x200B;以指派所有問題給您自己。
1. 按一下「**儲存**」。


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->




