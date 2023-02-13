---
product-area: projects
navigation-topic: use-the-gantt-chart
title: 更新任務清單甘特圖中的資訊
description: 任務清單甘特圖顯示項目或模板上任務的詳細資訊。
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 1%

---

# 更新任務清單中的資訊 [!UICONTROL 甘特圖]

任務清單 [!UICONTROL 甘特圖] 顯示項目或模板上任務的詳細資訊。

在模板中，任務清單 [!UICONTROL 甘特圖] 會反映在任務層模板的任務清單中所做的更新。 您無法編輯 [!UICONTROL 甘特圖] 與範本相關聯。

在項目中，您可以直接更新任務清單中的任務資訊 [!UICONTROL 甘特圖].

本文介紹了可以直接在「任務清單」中執行的以下操作 [!UICONTROL 甘特圖]:

* 修改任務持續時間
* 建立或刪除前置關係
* 更改任務開始和結束日期
* 更新完成百分比
* 級別項目資源

## 存取需求

您必須具備下列條件，才能遵循本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>[!UICONTROL編輯]對項目和任務的訪問</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>[!UICONTROL管理]對項目和任務的訪問 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 修改任務持續時間

1. 前往您要修改的專案。
1. 按一下 **[!UICONTROL 工作]** 中。

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. 按一下 **[!UICONTROL 甘特圖]** 表徵圖。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   所有變更都會在 **[!UICONTROL 自動儲存]** 選項。 預設會啟用。

1. （選用）按一下 **[!UICONTROL 計畫模式]** 圖示並選取 **[!UICONTROL 手動儲存Standard]** 或 **[!UICONTROL 時間表規劃]** 以手動儲存變更。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 將滑鼠指標暫留在任務的時間軸上，並將時間線指標拖曳至不同的日期。
1. 當您達到任務的正確新完成日期時，請刪除指示器。
1. （選用和條件式）如果您已選取手動儲存變更，請按一下 **[!UICONTROL 還原]** 或&#x200B;**[!UICONTROL 取消復原]** 表徵圖。

   >[!TIP]
   >
   >您可以使用以下鍵盤快捷鍵來撤消或重做甘特圖上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 還原和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]:使用 [!UICONTROL Ctrl + Z] 還原和 [!UICONTROL Ctrl + Y] 重做。


1. 按一下 **[!UICONTROL 儲存]** 在 [!UICONTROL 甘特圖].

## 建立或刪除前置關係

1. 前往您要修改的專案。
1. 在 **[!UICONTROL 工作]** ，按一下 **[!UICONTROL 甘特圖]** 表徵圖。

   此 **[!UICONTROL 自動儲存]** 選項，則所有變更都會自動儲存。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. （選用）按一下 **[!UICONTROL 計畫模式]** 圖示並選取 **[!UICONTROL 手動儲存Standard]** 或 **[!UICONTROL 時間表規劃]** 以手動儲存變更。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 要建立前置關係，請按一下任務的起始點，並將其拖動到任務的終點。
1. 要刪除前置關係，請按一下連接兩個任務的前置行以選擇它，然後按鍵 **[!UICONTROL 刪除]** 鍵盤上。\
   ![Delete_precisont.png](assets/delete-predecessor-350x152.png)

1. （選用和條件性）如果您選取手動儲存變更，請按一下 **[!UICONTROL 還原]** 或&#x200B;**[!UICONTROL 取消復原]** 表徵圖。

   >[!TIP]
   >
   >您可以使用以下鍵盤快捷鍵來撤消或重做甘特圖上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 還原和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]: [!UICONTROL 使用Ctrl + Z] 還原和 [!UICONTROL Ctrl + Y] 重做。


1. 按一下&#x200B;**[!UICONTROL 儲存]**。

## 更改任務開始和結束日期

1. 前往您要修改的專案。
1. 在 **[!UICONTROL 工作]** ，按一下 **[!UICONTROL 甘特圖]** 表徵圖。

   所有變更都會在 **[!UICONTROL 自動儲存]** 選項。 預設會啟用。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. （選用）按一下 **[!UICONTROL 計畫模式]** 圖示並選取 **[!UICONTROL 手動儲存Standard]** 或 **[!UICONTROL 時間表規劃]** 以手動儲存變更。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 將滑鼠指標暫留在工作中心，並找出多向箭頭。
1. 按一下「 」，然後將任務拖曳至所需日期。

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. 如果以影響任務約束的方式更改任務日期，請按一下 **[!UICONTROL 接受]** 確認任務約束更改。

   >[!NOTE]
   >
   >如果任務具有以下約束之一，則系統會更新 [!UICONTROL 任務約束] to [!UICONTROL 開始之前] 若從 [!UICONTROL 開始日期] 或 [!UICONTROL 完成時間不晚於] 如果已排程專案，則 [!UICONTROL 完成日期]:
   >
   >   
   >   
   >   * [!UICONTROL 盡可能早]
   >   * [!UICONTROL 盡可能遲]
   >   * [!UICONTROL 最早可用時間]
   >   * [!UICONTROL 最晚可用時間]

   >   
   >   
   >在某些情況下，前置關係可能會阻止任務較早開始，並且不允許任務移動。

1. （選用和條件式）如果您已選取手動儲存變更，請按一下 **[!UICONTROL 還原]** 或&#x200B;**[!UICONTROL 取消復原]** 表徵圖。

   >[!TIP]
   >
   >您可以使用下列鍵盤快速鍵來還原或重做對 [!UICONTROL 甘特圖]:
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 還原和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]:使用 [!UICONTROL Ctrl + Z] 還原和 [!UICONTROL Ctrl + Y] 重做。


1. 按一下&#x200B;**[!UICONTROL 儲存]**。

## 更新完成百分比

1. 前往您要修改的專案。
1. 在 **[!UICONTROL 工作]** ，按一下 **[!UICONTROL 甘特圖]** 表徵圖。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   所有變更都會在 **[!UICONTROL 自動儲存]** 選項。 預設會啟用。

1. （選用）按一下 **[!UICONTROL 計畫模式]** 圖示並選取 **[!UICONTROL 手動儲存Standard]** 或 **[!UICONTROL 時間表規劃]** 以手動儲存變更。
1. 按兩下任務內的百分比編號，然後輸入編號。

   >[!IMPORTANT]
   >
   >您必須 [!UICONTROL 完成%] 在 [!UICONTROL 選項] 對話方塊，以更新完成百分比。 若要這麼做，請按一下 **[!UICONTROL 選項]** 圖示並選取 **[!UICONTROL 完成%]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >

1. （選用和條件性）如果您選取手動儲存變更，請按一下 **[!UICONTROL 還原]** 或&#x200B;**[!UICONTROL 取消復原]** 表徵圖。

   >[!TIP]
   >
   >您可以使用下列鍵盤快速鍵來還原或重做對 [!UICONTROL 甘特圖]:
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 還原和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]:使用 [!UICONTROL Ctrl + Z] 還原和 [!UICONTROL Ctrl + Y] 重做。


1. 按一下 **[!UICONTROL 儲存]** 在 [!UICONTROL 甘特圖].

## 級別項目資源

您可以使用任務清單 [!UICONTROL 甘特圖] 來級別資源。

如需有關 [!UICONTROL 甘特圖]，請參閱 [層級資源 [!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
