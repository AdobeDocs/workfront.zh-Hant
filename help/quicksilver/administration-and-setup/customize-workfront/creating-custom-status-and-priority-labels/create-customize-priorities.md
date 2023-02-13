---
title: 建立和自訂優先順序
description: 您可以在Workfront的「設定」區域中控制專案、工作和問題的優先順序。 優先順序會重視您在Adobe Workfront中的專案、工作或問題。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# 建立和自訂優先順序

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

您可以在Workfront的「設定」區域中控制專案、工作和問題的優先順序。 優先順序會重視您在Adobe Workfront中的專案、工作或問題。

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

## 自訂現有優先順序

身為Workfront管理員，您可以對Workfront中提供的預設優先順序進行下列修改：

* 更名優先順序。
* 重新排序優先順序。

   如需如何重新排序優先順序的詳細資訊，請參閱 [為項目任務或問題建立優先順序](#create-a-priority-for-a-project-task-or-issue).

* 變更預設優先順序。

   如需變更預設優先順序功能的詳細資訊，請參閱 [為項目任務或問題建立優先順序](#create-a-priority-for-a-project-task-or-issue).

* 編輯優先順序的說明。
* 為每個優先順序設定一個顏色。

   將結果分組為 **優先順序**.

   如需圖表報表的詳細資訊，請參閱 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 刪除優先順序。

   刪除現有優先順序時，必須選擇替換優先順序。

* 隱藏優先順序。

   如需隱藏優先順序功能的詳細資訊，請參閱 [為項目任務或問題建立優先順序](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >每個物件的Workfront帳戶中必須至少有一個優先順序。

預設情況下，為每個對象類型（項目、任務和問題）提供的優先順序相同：

* 無
* 低
* 標準
* 高
* 緊急

## 為項目任務或問題建立優先順序 {#create-a-priority-for-a-project-task-or-issue}

除了Workfront中提供的預設優先順序外，您也可以新增自己的優先順序以反映組織的需求。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **專案偏好設定** > **優先順序**.

1. 按一下要建立優先順序的對象類型(**專案**, **任務**，或 **問題**)。
1. 按一下 **新增優先順序**.
1. 指定新優先順序的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">優先順序名稱</td> 
      <td>輸入優先順序的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要</td> 
      <td> <p>新增優先順序時，預設會為其指派數字。 編輯此號碼（如果它不符合您的需要）。</p> <p>此 <strong>重要性</strong> 每個優先順序的編號對於所選對象必須是唯一的。<br>優先順序的數量反映了項目、任務或問題的重要性：最高數目對應於最高優先順序。</p> <p><b>注意</b>:保存優先順序後，無法編輯「重要性」編號。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">顏色</td> 
      <td> <p>選擇優先順序的顏色。</p> <p>優先順序的顏色用於圖表報告和敏捷團隊設定。 如需圖表報表的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">新增圖表至報表</a>.</p> <p>如需敏捷團隊設定的詳細資訊，請參閱中的。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設優先順序</td> 
      <td> <p>選取選項按鈕，以決定此優先順序是否為預設優先順序。</p> <p>如果將優先順序指定為 <strong>預設優先順序</strong>，系統會針對Workfront中的所有專案、工作或問題自動挑選摘要。 <strong>正常</strong> 是Workfront中所有物件的預設優先順序。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>為優先順序新增說明以說明其功能。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱藏</td> 
      <td> <p>如果要隱藏優先順序，請選擇此框。</p><p>選取 <b>隱藏</b> 選項中，優先順序不會顯示在Workfront的任何位置，且使用者無法針對其專案、工作和問題選擇優先順序。</p> 
      <p><b>重要</b>:建議您隱藏不想再使用的優先順序，而不要刪除。 通過隱藏它們，您仍然可以保留所有以此優先順序完成的對象的歷史資料，同時防止人們將來選擇此優先順序。 </p>
      <p>您可以視需要選擇將優先順序拖曳至所需順序，以變更優先順序的清單順序。 這會變更專案、工作和問題的顯示順序。 這不會變更 <b>重要性</b> 數字。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

有關將優先順序應用於項目、任務和問題的說明，請參閱以下文章：

* [了解並更新專案優先順序](../../../manage-work/projects/planning-a-project/project-priority.md)
* [更新任務優先順序](../../../manage-work/tasks/task-information/task-priority.md)
* [更新問題優先順序](../../../manage-work/issues/issue-information/update-issue-priority.md)
