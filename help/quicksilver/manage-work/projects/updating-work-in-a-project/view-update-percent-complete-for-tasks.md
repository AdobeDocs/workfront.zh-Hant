---
product-area: projects
navigation-topic: update-work-in-a-project
title: 檢視和更新任務的完成百分比
description: 您可以更新任務的完成百分比，以指出完成任務的進度。 更新問題的完成百分比類似於更新任務的完成百分比。 本文會介紹如何更新任務的完成百分比。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 檢視並更新任務的完成百分比

<!--Audited: 05/2025-->

您可以更新任務的完成百分比，以指出完成任務的進度。

更新問題的完成百分比類似於更新任務的完成百分比。 本文會介紹如何更新任務的完成百分比。

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
   <p>工作或更高</p>
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
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 您可以更新任務完成百分比的區域

您可以在下列任一區域中更新任務的完成百分比：

* **在任務清單中**：當顯示完成百分比欄時，您可以更新任務的完成百分比。

  如需內嵌編輯的詳細資訊，請參閱[在Adobe Workfront中內嵌編輯清單的專案](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)。

* **在里程碑檢視中**：在專案清單或專案報告上使用里程碑檢視時，您可以更新任務的完成百分比。

  >[!TIP]
  >
  >  您無法更新「里程碑」檢視中問題的完成百分比。


  如需詳細資訊，請參閱[使用里程碑檢視](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md)。

* **在任務標題中**：您可以更新任務標題中任務的完成百分比。

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **在任務的摘要面板中**：您可以在檢視下列區域中的任務時，更新摘要面板頂端的任務完成百分比：

   * 任務清單或報告
   * 時程表
   * 工作負載平衡器

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  如需詳細資訊，請參閱[摘要概觀](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **首頁**：您可以從「首頁」區域的「摘要」面板或「我的工作」Widget更新任務或問題的完成百分比。

  如需詳細資訊，請參閱[首頁快速入門](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md)。

## 更新任務完成百分比的考量事項

* 當您將任務標示為100%完成時，任務「狀態」會更新為「完成」。 問題的狀態更新為「已關閉」。
* 完成任務也會更新父系和專案的完成百分比。
* 父級任務和專案存在下列案例：
   * 當專案的「摘要完成模式」設定為「自動」且子任務未完成時，您無法將父系任務的完成百分比更新為100%。
   * 當專案的「摘要完成模式」設定為「手動」，且子任務完成或不完成時，您可以將父系任務或專案的完成百分比更新為100%。

  如需詳細資訊，請參閱[編輯專案](../manage-projects/edit-projects.md)。

## 更新任務的完成百分比

1. 前往您要更新任務完成百分比的任何區域。

   如需詳細資訊，請參閱本文章中[您可以更新任務](#areas-where-you-can-update-the-percent-complete-of-a-task)完成百分比的區域。

1. 找到您要更新其完成百分比的任務的&#x200B;**完成百分比**&#x200B;欄位。

   >[!TIP]
   >
   >完成百分比欄位一律顯示在摘要面板頂端。

1. 在&#x200B;**完成百分比**&#x200B;欄位內按一下，然後輸入介於0到100之間的數字

   或

   按一下並拖曳&#x200B;**完成百分比**&#x200B;藍色泡泡至必要的數字，以指出您完成了多少工作（可用時）。

   >[!NOTE]
   >
   >    * 當您在「完成百分比」泡泡內按一下時，無法輸入十進位數字。
   >    * 當您拖放「摘要」面板中的藍色泡泡時，「完成百分比」會以一點為單位更新。
   >
   >    * 當您拖放任務標題中的藍色泡泡時，完成百分比會以5點為單位更新。

1. 在鍵盤上按Enter鍵以儲存完成百分比。

   專案或任何父系任務的完成百分比也可能自動更新。

   任務或問題的狀態也會更新。

