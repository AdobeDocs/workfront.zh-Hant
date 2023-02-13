---
title: 建立或自訂問題嚴重性
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您的使用者可使用嚴重性來定義問題的嚴重程度。 您可以自訂Adobe Workfront中現有的五個預設嚴重性之一，或為使用者建立新的嚴重性。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# 建立或自訂問題嚴重性

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

您的使用者可使用嚴重性來定義問題的嚴重程度。 您可以自訂Adobe Workfront中現有的五個預設嚴重性之一，或為使用者建立新的嚴重性。

>[!NOTE]
>
>任務和項目不具有嚴重性。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 內建問題嚴重性

Workfront有5個內建的問題嚴重性：

* 輕微
* 導致混淆
* 有因應措施的錯誤
* 無因應措施的錯誤
* 致命錯誤

<p>您可以編輯下列這些嚴重性的項目：</p>

* 名稱
* 顏色

   如果按「問題嚴重性」對結果進行分組，則嚴重性的顏色將保留在圖表報告中。 如需圖表報表的資訊，請參閱 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 預設嚴重性

   如需預設嚴重性的詳細資訊，請參閱 [建立或編輯問題嚴重性](#create-or-edit-an-issue-severity) 這篇文章。
* 說明
* 嚴重性是否隱藏在Workfront中

   有關隱藏嚴重性的詳細資訊，請參閱 [建立或編輯問題嚴重性](#create-or-edit-an-issue-severity")

* 刪除嚴重性

   執行此操作時，必須選擇替換嚴重性。

## 建立或編輯問題嚴重性 {#create-or-edit-an-issue-severity}

身為Workfront管理員，您可以建立和編輯期刊嚴重性，以符合使用者的需求。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **專案偏好設定** > **嚴重性**.

1. 如果要建立新的嚴重性，請按一下 **添加新嚴重性**.
1. 為新嚴重性配置以下選項，或為現有嚴重性編輯它們：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">嚴重程度名稱</td> 
      <td>鍵入嚴重性的名稱</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要</td> 
      <td>增加或降低嚴重性級別(最初由Workfront指定)。
      <p>每個嚴重性的重要性編號必須是唯一的。 最高數量對應於最高級別的嚴重性。</p> <p>保存嚴重性後，無法編輯此編號。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">顏色</td> 
      <td> <p>選擇嚴重性的顏色。</p> 
      <p>按問題嚴重性對結果進行分組時，會在圖表報告中使用嚴重性的顏色。 如需圖表報表的資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">新增圖表至報表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設嚴重程度</td> 
      <td>選取您希望Workfront自動選取所有新建立的問題的嚴重性。</p>
      <p>美化是Workfront中問題的預設嚴重性。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>鍵入嚴重性的說明以解釋其功能。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱藏</td> 
      <td> 隱藏不再需要的嚴重性。 
      <p>隱藏的嚴重性不會顯示在Workfront的任何位置，因此使用者無法針對其問題選擇它。</p> 
      <p><b>重要</b>:建議您隱藏這些嚴重性，而不要刪除您不想再使用的嚴重性。 這樣，您就可以保留已以嚴重性完成的對象上的所有歷史資料，同時防止將來使用嚴重性。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）依您想要的順序拖放，以變更嚴重性的清單順序。

   這會變更問題的顯示順序。 不會變更 **重要性** 數字。

1. 按一下&#x200B;**儲存**。

如需如何在處理問題時使用嚴重性的詳細資訊，請參閱 [更新問題嚴重性](../../../manage-work/issues/issue-information/update-issue-severity.md).
