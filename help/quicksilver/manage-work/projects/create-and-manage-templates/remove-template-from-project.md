---
product-area: templates
navigation-topic: templates-navigation-topic
title: 從項目中刪除模板資訊
description: 無法從項目中刪除模板。 您只能手動移除將範本附加至專案後，新增至專案的資訊。 有關附加模板的資訊，請參閱將模板附加到項目。
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 從項目中刪除模板資訊

無法從項目中刪除模板。 您只能手動移除將範本附加至專案後，新增至專案的資訊。 有關附加模板的資訊，請參閱 [將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理對任務的訪問 </p> <p>貢獻或更高權限存取專案 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從項目中刪除模板資訊的選項

若要移除已新增至專案的範本資訊，您可以執行下列其中一項操作：

* 附加範本後，手動從專案移除資訊。

   如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

* 刪除專案中隨範本新增的任務。

   如需詳細資訊，請參閱 [刪除從模板建立的任務](#delete-tasks-created-from-a-template) 一節。

* 從Workfront刪除範本。 從Workfront刪除範本不會刪除專案中從範本新增的工作。

   如需詳細資訊，請參閱 [刪除專案範本](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## 刪除從模板建立的任務 {#delete-tasks-created-from-a-template}

1. 前往 **工作** 區段。
1. 執行下列任一項作業：

   * 為任務清單建立篩選器，以僅顯示使用以下語句從模板建立的任務：

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      如需建立篩選器的相關資訊，請參閱 [在Adobe Workfront中建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      應用篩選器時，清單中只顯示與「模板任務ID」關聯的任務。

   * 建立任務清單的視圖以顯示 **模板任務ID** 或 **模板任務名稱** 欄中的欄位。

      應用視圖時，使用模板建立了包含「模板任務ID」或「模板任務名稱」列中資訊的任務。

      如需建立檢視的相關資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 選取步驟2中識別的所有從範本建立的任務，然後按一下 **「刪除」圖示****>是，刪除它**。 如需詳細資訊，請參閱 [刪除任務](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
