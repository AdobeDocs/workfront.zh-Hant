---
title: 建立及自訂優先順序
description: 您可以在Workfront的「設定」區域中控制專案、任務和問題的優先順序。 優先順序可強調您在Adobe Workfront中的專案、任務或問題。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 5c80dca8a9f7dd5a693db9bf22738602da8b521b
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 2%

---

# 建立和自訂優先順序

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

您可以在Workfront的「設定」區域中控制專案、任務和問題的優先順序。 優先順序可強調您在Adobe Workfront中的專案、任務或問題。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自訂現有的優先順序

身為Workfront管理員，您可以對Workfront中提供的預設優先順序進行下列修改：

* 重新命名優先順序。
* 重新排列優先順序。

  如需有關如何重新排序優先順序的詳細資訊，請參閱[建立專案、任務或問題的優先順序](#create-a-priority-for-a-project-task-or-issue)。

* 變更預設優先順序。

  如需有關變更預設優先順序功能的詳細資訊，請參閱[為專案、任務或問題建立優先順序](#create-a-priority-for-a-project-task-or-issue)。

* 編輯優先順序的說明。
* 設定每個優先順序的顏色。

  當您按&#x200B;**優先順序**&#x200B;將結果分組時，優先順序的顏色會用於圖表報告中。

  如需圖表報表的詳細資訊，請參閱[新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 刪除優先順序。

  當您刪除現有的優先順序時，必須選取替代優先順序。

* 隱藏優先順序。

  如需隱藏優先順序功能的詳細資訊，請參閱[為專案、任務或問題建立優先順序](#create-a-priority-for-a-project-task-or-issue)。

  >[!NOTE]
  >
  >在Workfront帳戶中，每個物件必須至少有一個優先順序。

預設為每個物件型別（專案、任務和問題）提供的優先順序相同：

* 無
* 低
* 正常
* 高
* 緊急

## 建立專案、任務或問題的優先順序 {#create-a-priority-for-a-project-task-or-issue}

除了Workfront提供的預設優先順序之外，您還可以新增自己的優先順序以反映組織的需求。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**專案偏好設定** > **優先順序**。

1. 按一下您要為（**專案**、**任務**&#x200B;或&#x200B;**問題**）建立優先順序的物件型別標籤。
1. 按一下表格底部的&#x200B;**新列**。
1. 為優先順序設定下列選項：

   * **優先順序名稱**：輸入優先順序的名稱。
   * **重要性**：新增優先順序時，預設會指派一個數字。 如果不符合您的需求，請編輯此數字。

     每個優先順序的重要性數字必須是唯一的。 優先順序的數目反映了專案、任務或問題的重要性：最高的數目對應到最高的優先順序。

     儲存優先順序後就無法編輯此數字。

   * **色彩**：選擇優先順序的色彩。

     優先順序的顏色用於圖表報告和敏捷團隊設定。 如需圖表報表的資訊，請參閱[新增圖表至報表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。 有關敏捷團隊設定的資訊，請參閱[建立敏捷團隊](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)。

   * **預設優先順序**：選取您希望Workfront自動套用至所有新建立專案、任務或問題的優先順序。

     **一般**&#x200B;是Workfront中所有物件的預設優先順序。

     您不能將隱藏的優先順序設為預設值。

     預設優先順序以圖示![預設優先順序圖示](assets/default-icon.png)表示。 若要選擇新的預設值，請執行下列任一項作業：

      * 選取優先順序名稱旁的核取方塊，並在熒幕底部的動作列中選取&#x200B;**設定為預設**。
      * 將滑鼠停留在優先順序名稱上，然後按一下出現的&#x200B;**更多**&#x200B;功能表。 然後，選取&#x200B;**設定預設值**。

        新的預設優先順序會以圖示標示。

   * **描述**：輸入優先順序的描述，以說明其功能。
   * **隱藏選擇**：選取&#x200B;**是**&#x200B;以隱藏不再需要的優先順序。

     隱藏的優先順序在Workfront中的任何位置都不會顯示，因此使用者無法為其專案、任務或問題選擇它。

     >[!IMPORTANT]
     >
     >建議您隱藏優先順序，不要刪除您不想再使用的優先順序。 如此一來，您就可以保留物件上所有已使用優先順序完成的歷史資料，同時防止人們日後使用優先順序。

1. （選擇性）依您想要的順序拖放優先順序，以變更優先順序的清單順序。

   這會變更專案、任務或問題的顯示順序。 它不會變更&#x200B;**重要性**&#x200B;數字。

1. 按一下「**儲存**」。

如需將優先順序套用至專案、任務和問題的指示，請參閱下列文章：

* [瞭解並更新專案優先順序](../../../manage-work/projects/planning-a-project/project-priority.md)
* [更新任務優先順序](../../../manage-work/tasks/task-information/task-priority.md)
* [更新問題優先順序](../../../manage-work/issues/issue-information/update-issue-priority.md)
