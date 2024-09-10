---
title: 建立或自訂問題嚴重程度
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您的使用者可使用嚴重程度來定義問題的嚴重程度。 您可以自訂Adobe Workfront中現有的五種預設嚴重程度，或為使用者建立新的嚴重程度。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 5%

---

# 建立或自訂問題嚴重程度

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

您的使用者可使用嚴重程度來定義問題的嚴重程度。 您可以自訂Adobe Workfront中現有的五種預設嚴重程度，或為使用者建立新的嚴重程度。

>[!NOTE]
>
>任務和專案沒有嚴重性。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
     <p>新增：標準</p>
     <p>或</p>
     <p>目前：計畫</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 內建問題嚴重程度

Workfront有五個內建問題嚴重性：

* 輕微
* 導致混淆
* 有因應措施的錯誤
* 無因應措施的錯誤
* 致命錯誤

<p>您可以針對這些嚴重程度編輯下列專案：</p>

* 姓名
* 顏色

  如果您依問題嚴重程度將結果分組，嚴重程度的顏色會保留在圖表報告中。 如需圖表報表的資訊，請參閱[新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 預設嚴重程度

  如需預設嚴重程度的詳細資訊，請參閱本文中的[建立或編輯問題嚴重程度](#create-or-edit-an-issue-severity)。
* 說明
* Workfront中是否隱藏嚴重程度

  如需隱藏嚴重程度的詳細資訊，請參閱[建立或編輯問題嚴重程度](#create-or-edit-an-issue-severity")

* 刪除嚴重程度

  執行此操作時，必須選取替代嚴重程度。

## 建立或編輯問題嚴重程度 {#create-or-edit-an-issue-severity}

身為Workfront管理員，您可以根據使用者的需求建立和編輯問題嚴重程度。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**專案偏好設定** > **嚴重程度**。

1. 如果您正在建立新的嚴重程度，請按一下&#x200B;**新增嚴重程度**。
1. 針對新嚴重性設定下列選項，或編輯現有嚴重性的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">嚴重程度名稱</td> 
      <td>輸入嚴重程度的名稱</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要</td> 
      <td>提高或降低嚴重性的嚴重性等級，最初由Workfront指派。
      <p>每個嚴重程度的重要性數字必須是唯一的。 最高數字對應於嚴重性的最高層級。</p> <p>儲存嚴重程度後，就無法編輯此數字。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">顏色</td> 
      <td> <p>選擇嚴重程度的顏色。</p> 
      <p>當您依問題嚴重程度將結果分組時，會在圖表報告中使用嚴重程度的顏色。 如需圖表報表的資訊，請參閱<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">新增圖表至報表</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設嚴重程度</td> 
      <td>選取您希望Workfront自動選取所有新建立問題的嚴重程度。</p>
      <p>在Workfront中，裝飾是問題的預設嚴重性。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入嚴重程度的說明以說明其功能。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱藏</td> 
      <td> 隱藏不再需要的嚴重程度。 
      <p>隱藏的嚴重程度不會在Workfront的任何位置顯示，因此使用者無法針對其問題選擇它。</p> 
      <p><b>重要</b>：建議您隱藏嚴重程度，不要刪除不想再使用的嚴重程度。 如此一來，您就可以保留物件上所有已使用嚴重度完成的歷史資料，同時防止人們日後使用嚴重度。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）以您想要的順序拖放嚴重性，以變更其清單順序。

   這會變更問題顯示的順序。 它不會變更&#x200B;**重要性**&#x200B;數字。

1. 按一下「**儲存**」。

如需處理問題時如何使用嚴重程度的詳細資訊，請參閱[更新問題嚴重程度](../../../manage-work/issues/issue-information/update-issue-severity.md)。
