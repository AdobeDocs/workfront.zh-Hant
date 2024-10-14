---
product-area: templates
navigation-topic: templates-navigation-topic
title: 從專案移除範本資訊
description: 您無法從專案移除範本。 您只能手動移除將範本附加至專案後新增至專案的資訊。 如需有關附加範本的資訊，請參閱將範本附加至專案。
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# 從專案移除範本資訊

您無法從專案移除範本。 您只能手動移除將範本附加至專案後新增至專案的資訊。 如需有關附加範本的資訊，請參閱[將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>新增：標準</p>
   <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理對任務的存取 </p> <p>Contribute或更高的專案存取權 </p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從專案移除範本資訊的選項

若要移除已新增至專案的範本資訊，您可以執行下列任一項作業：

* 在附加範本後，手動從專案中移除資訊。

  如需詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

* 刪除專案中新增了範本的任務。

  如需詳細資訊，請參閱本文中的[刪除從範本](#delete-tasks-created-from-a-template)建立的任務。

* 從Workfront刪除範本。 從Workfront中刪除範本並不會從專案中刪除從範本新增的任務。

  如需詳細資訊，請參閱[刪除專案範本](../../../manage-work/projects/create-and-manage-templates/delete-templates.md)。

## 刪除從範本建立的任務 {#delete-tasks-created-from-a-template}

1. 移至專案的&#x200B;**任務**&#x200B;區段。
1. 執行下列其中一項：

   * 建立工作清單的篩選器，僅顯示使用下列陳述式從範本建立的工作：

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     如需建立篩選的詳細資訊，請參閱[在Adobe Workfront中建立或編輯篩選](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

     當您套用篩選器時，清單中只會顯示與範本任務ID相關的任務。

   * 建立工作清單的檢視，以顯示資料欄中的&#x200B;**範本工作識別碼**&#x200B;或&#x200B;**範本工作名稱**&#x200B;欄位。

     當您套用檢視時，會使用範本建立包含「範本任務ID」或「範本任務名稱」欄中資訊的任務。

     如需建立檢視的相關資訊，請參閱[在Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

1. 選取步驟2中識別為使用範本建立的所有工作，然後按一下&#x200B;**刪除圖示****>是，刪除**。 如需詳細資訊，請參閱[刪除工作](../../../manage-work/tasks/manage-tasks/delete-tasks.md)。
