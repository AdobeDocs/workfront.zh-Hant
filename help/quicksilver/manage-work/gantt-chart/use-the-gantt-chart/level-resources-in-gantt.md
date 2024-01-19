---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: 平準資源  [!UICONTROL 甘特圖]
description: 有關如何在甘特圖中層次資源的資訊。
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# 平準資源 [!UICONTROL 甘特圖]

平準專案的資源有兩個用途：

* 若要自動調整受指派者的時間過度配置。
* 自動為專案建立逼真的任務排程。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL Edit]專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[！UICONTROL Manage]專案的存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 資源平準概要

如果將相同的資源指派給兩個不同的任務，則可以使用資源平準來調整任務的時間表，使它們不會同時發生。

平準專案上的資源時，請考量下列事項：

* 資源平準僅適用於一個專案，因此 [!DNL Adobe Workfront] 不會一次將資源平準至多個專案。
* 如果 **[!UICONTROL 投入比導向]** 已選取為 **[!UICONTROL 期間型別]**， [!DNL Workfront] 不會平準資源。
* 將多位使用者指派給同一個任務時，將會取消平準。
* 此型別的條件 **[!UICONTROL 任務限制]** 優先於資源平準。 例如，如果 **[!UICONTROL 固定日期]** 已選取作為 [!UICONTROL 任務限制]，資源平準將不會變更任務日期。
* 前置任務關係將優先於資源平準。
* **[!UICONTROL 資源平準]** 需要設定為 **[!UICONTROL 手動]** 用於專案，以調整平準 [!UICONTROL 甘特圖]. 如果您擁有專案的管理許可權，您可以調整專案的這項設定並選取「 」，讓系統自動調整資源 **[!UICONTROL 自動]** 而非 **[!UICONTROL 手動]** 在 **[!UICONTROL 編輯專案]** 方塊。

  ![](assets/resource-leveling-mode-350x177.png)

* 作為專案所有者或任務受指派人，您可以為任務引入平準延遲，以表示任務極有可能需要額外的時間。 如需有關將平準延遲新增至任務的資訊，請參閱 [更新任務平準延遲](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## 在中套用資源平準 [!UICONTROL 甘特圖]

您可以使用工作清單 [!UICONTROL 甘特圖] 以平準您的資源。

1. 移至您要平準的專案。
1. 在 **[!UICONTROL 任務]** 區域，按一下 **[!UICONTROL 甘特圖]** 圖示。

   所有變更會在 **[!UICONTROL 自動儲存]** 選項已啟用。 預設為啟用。

1. （可選）按一下 **[!UICONTROL 計畫] 模式** 圖示並選取 **[!UICONTROL 手動儲存標準]** 或 **[!UICONTROL 時間表規劃]** 以手動儲存變更。

   >[!TIP]
   >
   >您無法在中調配資源  [!UICONTROL 甘特圖] 當 [!UICONTROL 自動儲存] 選項已啟用。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 按一下 **[!UICONTROL 平準資源]** 下拉式功能表。

   ![Level_resources.png](assets/level-resouces.png)

1. 選取下列其中一個選項：

   * **[!UICONTROL 立即平準]**：將資源平準套用至選取的任務。
   * **[!UICONTROL 清除平準]**：從選取的任務移除所有資源平準。

   >[!NOTE]
   >
   >如果將資源指派給在相同時間範圍內發生的多個任務，則資源可能會過度配置。

1. （選擇性和條件性）如果您已停用「自動儲存」選項，請按一下 **[!UICONTROL 還原]** 或&#x200B;**[!UICONTROL 取消復原]** 圖示。

   >[!TIP]
   >
   >您可以使用下列鍵盤快速鍵來復原或重做對 [!UICONTROL 甘特圖]：
   >
   >* [!DNL Mac]：使用 [!UICONTROL Command + Z] 還原和 [!UICONTROL Command + Shift + Z] 以取消復原。
   >* Windows：使用 [!UICONTROL Ctrl + Z] 還原和 [!UICONTROL Ctrl + Y] 以取消復原。


1. 按一下 **[!UICONTROL 儲存]** 位於的右上角 [!UICONTROL 甘特圖].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
