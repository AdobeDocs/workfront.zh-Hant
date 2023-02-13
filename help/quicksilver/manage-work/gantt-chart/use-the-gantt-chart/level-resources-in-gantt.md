---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: 層級資源  [!UICONTROL 甘特圖]
description: 有關如何在甘特圖中對資源進行分級的資訊。
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# 層級資源 [!UICONTROL 甘特圖]

在專案上調整資源有兩個用途：

* 自動調整受分配者的超分配時間。
* 為項目自動建立實際任務計畫。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>[!UICONTROL編輯]對項目的訪問</p> <p><b>附註</b>

如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>對項目的[!UICONTROL管理]訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 資源均衡概述

如果將同一資源分配給兩個不同的任務，則可以使用資源均衡來調整任務的時間軸，使這些任務不會同時發生。

在項目上調平資源時，請考慮以下事項：

* 資源調平僅適用於一個項目，因此 [!DNL Adobe Workfront] 不會一次在多個專案間層級資源。
* 若 **[!UICONTROL 工作驅動]** 被選為 **[!UICONTROL 持續時間類型]**, [!DNL Workfront] 不會層級資源。
* 當多個用戶被分配到同一任務時，調平將被取消。
* 類型的條件 **[!UICONTROL 任務約束]** 將優先於資源平衡。 例如，若 **[!UICONTROL 固定日期]** 被選為 [!UICONTROL 任務約束]，資源調平不會變更任務日期。
* 前置關係優先於資源均衡。
* **[!UICONTROL 資源均衡]** 需要設定為 **[!UICONTROL 手動]** 為了調整 [!UICONTROL 甘特圖]. 如果您對專案擁有「管理」權限，則可以調整專案上的此設定並選取「 」，讓系統自動層級資源 **[!UICONTROL 自動]** 而非 **[!UICONTROL 手動]** 在 **[!UICONTROL 編輯專案]** 框。

   ![](assets/resource-leveling-mode-350x177.png)

* 作為項目所有者或任務受託人，您可以為任務引入調平延遲，以指明任務可能需要額外時間的可能性很大。 有關向任務添加調平延遲的資訊，請參閱 [更新任務調平延遲](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## 在 [!UICONTROL 甘特圖]

您可以使用任務清單 [!UICONTROL 甘特圖] 來級別資源。

1. 前往您要層級的專案。
1. 在 **[!UICONTROL 工作]** ，按一下 **[!UICONTROL 甘特圖]** 表徵圖。

   所有變更都會在 **[!UICONTROL 自動儲存]** 選項。 預設會啟用。

1. （選用）按一下 **[!UICONTROL 計畫] 模式** 圖示並選取 **[!UICONTROL 手動儲存Standard]** 或 **[!UICONTROL 時間表規劃]** 以手動儲存變更。

   >[!TIP]
   >
   >您無法在  [!UICONTROL 甘特圖] 當 [!UICONTROL 自動儲存] 選項。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 按一下 **[!UICONTROL 層級資源]** 下拉式功能表。

   ![Level_resources.png](assets/level-resouces.png)

1. 選取下列其中一個選項：

   * **[!UICONTROL 立即級別]**:將資源調平應用於選定任務。
   * **[!UICONTROL 清除平整]**:從所選任務中刪除所有資源均衡。

   >[!NOTE]
   >
   >如果資源被分配給同一時間範圍內發生的多個任務，則可能會過度分配資源。

1. （選用和條件式）如果您已停用自動儲存選項，請按一下 **[!UICONTROL 還原]** 或&#x200B;**[!UICONTROL 取消復原]** 表徵圖。

   >[!TIP]
   >
   >您可以使用下列鍵盤快速鍵來還原或重做對 [!UICONTROL 甘特圖]:
   >
   >* [!DNL Mac]:使用 [!UICONTROL Command + Z] 還原和 [!UICONTROL Command + Shift + Z] 重做。
   >* 窗口：使用 [!UICONTROL Ctrl + Z] 還原和 [!UICONTROL Ctrl + Y] 重做。



1. 按一下 **[!UICONTROL 儲存]** 在 [!UICONTROL 甘特圖].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p> <p> <img src="assets/qs-task-edit-icon-highlighted-350x154.png" style="width: 350;height: 154;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
