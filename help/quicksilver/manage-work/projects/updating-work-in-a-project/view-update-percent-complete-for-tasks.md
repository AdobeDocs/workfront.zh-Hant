---
product-area: projects
navigation-topic: update-work-in-a-project
title: 檢視並更新任務的完成百分比
description: 您可以更新任務的完成百分比，以指出完成任務的進度。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ee957e319941fe5eabb9144eed184372e5402197
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 檢視並更新任務的完成百分比

<!--Audited:01/2024-->

您可以更新任務的完成百分比，以指出完成任務的進度。

## 存取需求

您必須具有下列存取權才能手動更新任務：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新授權： Standard</p> 
   或
   <p>目前授權：工作或以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 您可以更新任務完成百分比的區域

您可以在下列任一區域中更新任務的完成百分比：

* **在工作清單中**：當顯示「完成百分比」欄時，您可以更新任務的完成百分比。\
  如需內嵌編輯的詳細資訊，請參閱 [在Adobe Workfront中內嵌編輯清單中的專案](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **在里程碑檢視中**：在專案清單或專案報告上使用里程碑檢視時，您可以更新任務的完成百分比。 如需詳細資訊，請參閱 [使用里程碑檢視](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **在任務標題中**：您可以在任務標題中更新任務的完成百分比。 如需詳細資訊，請參閱 [編輯任務](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **在任務的摘要面板中**：在下列區域中檢視任務時，您可以更新摘要面板頂端的任務完成百分比：

   * 任務清單或報告
   * 時程表
   * 工作負載平衡器

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  如需詳細資訊，請參閱 [摘要概觀](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)


## 更新任務完成百分比的考量事項

* 當您將任務標示為100%完成時，任務「狀態」會更新為「完成」。
* 父系任務存在下列情況：
   * 當專案的「摘要完成模式」設定為「自動」且子任務未完成時，您無法將父系任務的完成百分比更新為100%。
   * 當專案的「摘要完成模式」設定為「手動」，且子作業已完成或不完成時，您可以將父系作業的完成百分比更新為100%。

  如需詳細資訊，請參閱 [編輯專案](../manage-projects/edit-projects.md).

## 更新任務的完成百分比

1. 前往Workfront中的下列任一區域：

   * 工作清單
   * 專案清單和應用里程碑檢視
   * 任務，透過存取任務頁面
1. 找到 **完成百分比** 您要更新其完成百分比之任務的欄位。
1. 按一下完成百分比欄位，然後輸入介於0到100之間的數字

   或

   按一下並拖曳 **完成百分比** 列至必要的數字，以指出您已完成多少工作（若有可用的話）。

   >[!NOTE]
   >
   >當您指出所有的工作都已完成時，工作的狀態也會更新為「完成」。


1. 在鍵盤上按Enter鍵以儲存完成百分比。

專案的完成百分比也會自動更新。

