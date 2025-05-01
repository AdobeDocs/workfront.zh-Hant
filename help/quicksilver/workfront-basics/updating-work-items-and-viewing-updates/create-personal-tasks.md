---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 建立個人任務
description: 個人任務是指您傳送給使用者、自己或您在「首頁」區域中為自己建立的待辦事項的臨時工作請求。 Workfront會儲存隨選工作請求以及將專案作為個人任務來執行。
author: Lisa
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: a1081b7ce0877b08f9546ab57cfac3f2a580ea76
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# 建立個人任務

<!--Audited: 10/2024-->

個人任務是指您傳送給使用者或自己傳送或新增的臨時工作請求。

Adobe Workfront會儲存臨時工作請求，以及將專案當做個人任務在Wprfront自動為每個使用者建立的使用者個人專案上。

以下是使用者個人專案的特徵：

* Workfront中的所有使用者都有名為「&lt;使用者全名>的任務」的個人專案。 例如，「John Smith的任務」。
* 每個使用者的個人專案不會顯示在搜尋中，且會隱藏。
* 無法刪除個人專案，即使使用者已停用。
* The Status of a personal project is always Current. Personal projects cannot be completed or canceled.
* 所有個人任務都儲存在使用者的個人專案中。
* 如有需要，您可以將個人任務移至另一個專案。

您可以透過下列方式建立個人工作：

* 在您的首頁區域中建立待辦事項

  For information, see [Create work items and projects from the Home area](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Create and send a personal work request to another user from the user profile page
* Create and send a personal work request to yourself from your user profile page

This article describes how you can create a personal work request for a user or for yourself from the user profile page.

Regardless how you add a personal task, you can find them in the same areas of Workfront. For more information, see the section [Locate personal task](#locate-personal-tasks) in this article.

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> 
   <p>新增：標準傳送要求給其他使用者。 所有使用者都可以為自己建立工作請求。</p> 
   <p>目前：計畫傳送要求給其他使用者。 所有使用者都可以為自己建立工作請求。</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>編輯使用者的存取權以為其建立工作請求。 檢視存取權以建立自己的個人工作請求。 </p>
   </td> 
  </tr>

</tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 建立個人工作請求

1. 移至您使用者的設定檔頁面，或移至您有權檢視的其他使用者的設定檔頁面。

   >[!TIP]
   >
   >當某些使用者設定您的存取層級時，您的Workfront管理員可能會阻止您檢視這些使用者。

1. 按一下標題中使用者名稱右側的&#x200B;**更多功能表** ![](assets/more-menu.png)。
1. Click **Send work request**.
The **Send user a work request** box displays.

   ![](assets/personal-task-box.png)
1. 更新下列資訊：

   * **Task Name**: This is the name of the ad hoc work request or the personal task.
   * **Description**: Add a description for the task.
   * **Assign to**: The name of the user that you selected displays by default. You can add more users or teams.
   * **到期日**：這是您想要完成此工作的日期。 依預設，這是今天的日期。 您無法選取過去的日期
   * **Time**: This is the time by which you&#39;d like this task to be completed. By default, this is the current time.

1. Click **Send Request** to save the work request.

   The work request is saved as a personal task in Workfront and it is added to the user&#39;s To-dos widget in their Home area. 如果您將工作請求傳送給自己，它會顯示在您首頁的待辦事項Widget中。


## 尋找個人工作

您可以在下列區域找到個人工作：

* 傳送個人請求之使用者的「首頁」區域中的待辦事項Widget。

  如需詳細資訊，請參閱[從首頁區域建立工作專案和專案](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 個人工作報告或清單。 You can build and apply a personal task filter to a task report or list to display only personal tasks and exclude project tasks.

  For information, see [Filter: personal tasks](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).
