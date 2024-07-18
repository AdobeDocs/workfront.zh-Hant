---
title: 建立和自訂優先順序
description: 您可以在Workfront的「設定」區域中控制專案、任務和問題的優先順序。 優先順序可強調您在Adobe Workfront中的專案、任務或問題。
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

您可以在Workfront的「設定」區域中控制專案、任務和問題的優先順序。 優先順序可強調您在Adobe Workfront中的專案、任務或問題。

## 存取需求

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂現有的優先順序

身為Workfront管理員，您可以對Workfront中提供的預設優先順序進行下列修改：

* 重新命名優先順序。
* 重新排列優先順序。

  如需有關如何重新排序優先順序的詳細資訊，請參閱[建立專案任務或問題的優先順序](#create-a-priority-for-a-project-task-or-issue)。

* 變更預設優先順序。

  如需有關變更預設優先順序功能的詳細資訊，請參閱[建立專案任務或問題的優先順序](#create-a-priority-for-a-project-task-or-issue)。

* 編輯優先順序的說明。
* 設定每個優先順序的顏色。

  當您按&#x200B;**優先順序**&#x200B;將結果分組時，優先順序的顏色會用於圖表報告中。

  如需圖表報表的詳細資訊，請參閱[新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 刪除優先順序。

  當您刪除現有的優先順序時，必須選取替代優先順序。

* 隱藏優先順序。

  如需隱藏優先順序功能的詳細資訊，請參閱[為專案任務或問題建立優先順序](#create-a-priority-for-a-project-task-or-issue)。

  >[!NOTE]
  >
  >在Workfront帳戶中，每個物件必須至少有一個優先順序。

預設為每個物件型別（專案、任務和問題）提供的優先順序相同：

* 無
* 低
* 標準
* 高
* 緊急

## 建立專案任務或問題的優先順序 {#create-a-priority-for-a-project-task-or-issue}

除了Workfront提供的預設優先順序之外，您還可以新增自己的優先順序以反映組織的需求。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**專案偏好設定** > **優先順序**。

1. 按一下您要為（**專案**、**任務**&#x200B;或&#x200B;**問題**）建立優先順序的物件型別標籤。
1. 按一下&#x200B;**新增優先順序**。
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
      <td> <p>新增優先順序時，預設會指定一個數字。 如果不符合您的需求，請編輯此數字。</p> <p>每個優先順序的<strong>重要性</strong>數字對您選取的物件而言必須是唯一的。<br>優先順序的數目反映了專案、任務或問題的重要性：最高的數目會對應到最高的優先順序。</p> <p><b>注意</b>：儲存優先順序後，您無法編輯重要性號碼。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">顏色</td> 
      <td> <p>選擇優先順序的顏色。</p> <p>優先順序的顏色用於圖表報告和敏捷團隊設定。 如需圖表報表的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">新增圖表至報表</a>。</p> <p>如需敏捷團隊設定的詳細資訊，請參閱中的。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設優先順序</td> 
      <td> <p>選取選項按鈕，決定這是否應為預設優先順序。</p> <p>如果優先順序指定為<strong>預設優先順序</strong>，則會自動為Workfront中的所有專案、任務或問題挑選它。 <strong>一般</strong>是Workfront中所有物件的預設優先順序。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>新增優先順序的說明以說明其功能。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱藏</td> 
      <td> <p>如果要隱藏優先順序，請選取此方塊。</p><p>當您選取<b>隱藏</b>選項時，優先順序不會在Workfront中的任何地方顯示，使用者無法為其專案、任務和問題選擇它。</p> 
      <p><b>重要</b>：建議您隱藏不想再使用的優先順序，不要刪除優先順序。 透過隱藏它們，您仍會保留所有已使用此優先順序完成的物件的歷史資料，同時防止人們日後選擇此優先順序。 </p>
      <p>您可以視需要選擇拖放優先順序，以變更其清單順序。 這會變更專案、任務和問題的顯示順序。 這不會變更<b>重要性</b>數字。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。

如需將優先順序套用至專案、任務和問題的指示，請參閱下列文章：

* [瞭解並更新專案優先順序](../../../manage-work/projects/planning-a-project/project-priority.md)
* [更新任務優先順序](../../../manage-work/tasks/task-information/task-priority.md)
* [更新問題優先順序](../../../manage-work/issues/issue-information/update-issue-priority.md)
