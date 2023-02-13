---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''報表或清單：顯示與對象關聯的用戶'
description: 您可以顯示與報表或清單中的物件相關聯的使用者、工作角色和團隊，以及在篩選器中參考這些物件。 不能按與對象關聯的用戶、作業角色或團隊進行分組。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 2%

---

# 報表或清單：顯示與對象關聯的用戶

您可以顯示與報表或清單中的物件相關聯的使用者、工作角色和團隊，以及在篩選器中參考這些物件。 不能按與對象關聯的用戶、作業角色或團隊進行分組。

您可以依與下列物件相關聯的使用者、工作角色或團隊來顯示或篩選：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">物件</td> 
   <td>關聯的用戶或作業角色</td> 
  </tr> 
  <tr> 
   <td role="rowheader">專案</td> 
   <td> <p>您可以在專案報表中顯示所有使用者及其在專案中履行的工作角色。 您無法依使用者或其在專案報表中的相關工作角色進行篩選。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">任務</td> 
   <td>您可以依指派給任務報表中任務的所有使用者、工作角色和團隊來顯示和篩選。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">問題</td> 
   <td>您可以依指派給問題報表中的所有使用者、工作角色和團隊來顯示和篩選問題。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">專案組合</td> 
   <td>您可以在專案報表中顯示所有使用者及其在專案中履行的工作角色，並依Portfolio分組報表。 您無法依使用者或其在專案報表中的相關工作角色進行篩選。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">計劃</td> 
   <td>您可以在項目報告中顯示所有用戶及其在項目上履行的職務角色，並按方案對報告進行分組。 您無法依使用者或其在專案報表中的相關工作角色進行篩選。</td> 
  </tr> 
 </tbody> 
</table>

## 顯示與專案相關聯的所有使用者和工作角色

您可以在專案清單或報表的檢視中顯示專案中與關聯的所有使用者。 這包括列在專案「人員」區段中的所有使用者。 您也可以在專案報表中檢視指派給專案上的工作或問題時，與之關聯的角色。

![](assets/project-with-user-and-role-information-report-350x100.png)

如需有關建立專案報表以顯示專案上所有使用者及其角色的資訊，請參閱 [查看：具有作業角色的項目用戶清單](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

您無法在專案篩選器中篩選與專案相關聯的使用者或工作角色。

## 顯示指派給任務的所有用戶、作業角色或團隊

通過將「分配」欄位添加到視圖，您可以在任務清單或報告的視圖中顯示分配給任務的所有用戶、角色或團隊。

![](assets/assignments-field-task-view-350x124.png)

您可以參考任務篩選器中的以下欄位，依指派給任務的使用者、作業角色或團隊進行篩選：

* 指派使用者
* 指派角色
* 團隊

![](assets/assignment-users-roles-task-filter-350x334.png)

## 顯示指派給問題的所有使用者、工作角色或團隊

您可以在問題清單或報表的檢視中，將「工作總攬」欄位新增至檢視，以顯示指派給問題的所有使用者、角色或團隊。

您可以參照問題篩選器中的下列欄位，依指派給問題的使用者、工作角色或團隊進行篩選：

* 指派使用者
* 指派角色
* 團隊

## 顯示與產品組合關聯的所有用戶和作業角色

您可以在專案報表中顯示與產品組合相關聯的所有使用者和角色，然後依Portfolio將報表分組。

如需有關建立專案報表以顯示專案上所有使用者及其角色的資訊，請參閱 [查看：具有作業角色的項目用戶清單](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

您無法篩選產品組合或專案篩選器中與專案相關聯的使用者或工作角色。

## 顯示與程式關聯的所有用戶和作業角色

您可以在項目報告中顯示與某個程式關聯的所有用戶和角色，然後按程式對該報告進行分組。

如需有關建立專案報表以顯示專案上所有使用者及其角色的資訊，請參閱 [查看：具有作業角色的項目用戶清單](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

您無法篩選方案或專案篩選器中與專案相關聯的使用者或工作角色。
