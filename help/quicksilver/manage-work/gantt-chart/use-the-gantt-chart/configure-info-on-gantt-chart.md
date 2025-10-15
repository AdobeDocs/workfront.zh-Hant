---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: 設定資訊在[!UICONTROL 甘特圖]上的顯示方式
description: 您可以設定哪些資訊會顯示在工作清單甘特圖和專案清單甘特圖中。
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# 設定資訊在[!UICONTROL 甘特圖]上的顯示方式

<!-- Audited: 5/2025 -->

您可以設定哪些資訊會同時顯示在工作清單甘特圖和專案清單甘特圖中。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> 
   <p>[!UICONTROL Light]或更高<p>
   <p>[!UICONTROL Review]或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[!UICONTROL 檢視]或更高的專案和任務存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[!UICONTROL 檢視]或更高的專案和任務存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Light<p>
   <p>Or</p>
   <p>Current: Review</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 瞭解顯示選項

下表詳細說明[!UICONTROL 甘特圖]的顯示選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">實際日期</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL 實際開始日期]和[!UICONTROL 實際完成日期]會以三角形圖示顯示。 如果[!UICONTROL 實際完成日期]為Null，則只會顯示[!UICONTROL 實際開始日期]。</p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">專案總覽[!UICONTROL 實際完成日期] </a>和<a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">專案總覽[!UICONTROL 實際開始日期] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 指定任務]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>顯示任務受指派人。 將滑鼠停留在受指派人名稱旁的「詳細資訊」連結上，可檢視有關他們的詳細資訊，包括其配置給任務的百分比。</p> <p>將[!UICONTROL 甘特圖]匯出至PDF時，[!UICONTROL 甘特圖]上不會顯示受指派人。 將[!UICONTROL 甘特圖]匯出至PDF時，受指派人只會顯示在工作清單中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 基準線]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>代表包含在初始專案計畫中的專案關鍵資料片段的專案快照。 可以在專案的時間表中使用基準線。 當您啟用在[!UICONTROL 甘特圖]中顯示基準線時，請選取您要顯示的基準線。 您一次只能在[!UICONTROL 甘特圖]上檢視一個基準線，而且會以灰色長條顯示。</p> <p>如需基準線的詳細資訊，請參閱<a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">建立專案基準線</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 認可日期]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>受指派人承諾完成工作的日期，會在[!UICONTROL 甘特圖]中以標籤顯示。 </p> <p>如需認可日期的詳細資訊，請參閱<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL 認可日期]概觀</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL %完成]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  任務的完成百分比會顯示在任務明細中。<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 關鍵路徑]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>可能會影響專案時間表的工作會視為關鍵路徑的一部分，並明確地以紅色標示。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]菱形</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>與里程碑相關聯的工作之後會顯示菱形圖示。 將滑鼠指標暫留在里程碑上，即可檢視里程碑的名稱和日期。 [!DNL Workfront]管理員決定每個里程碑菱形的顏色。</p> <p>如需里程碑的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">建立里程碑路徑</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]行</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>與里程碑相關聯的任務後面會顯示一條直線。 將滑鼠指標暫留在里程碑上，即可檢視里程碑的名稱和日期。 [!DNL Workfront]管理員決定每個里程碑線的色彩。</p> <p> 如需里程碑的詳細資訊，請參閱  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">建立里程碑路徑</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 前置任務]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="前置任務_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>顯示兩個任務之間前置任務關係的任務行。 若要反白顯示個別的前置任務行，請將滑鼠游標停留在前置任務行上。 按一下以反白顯示。 您一次只能反白一個前置任務行。</p> <p>任何具有跨越甘特圖上多個頁面的前置任務關係的任務，或具有跨專案前置任務的任何任務，其旁邊都會顯示[!UICONTROL 前置任務]圖示。</p> <p>按一下[!UICONTROL 前置任務]圖示可檢視所有前置任務和後續任務及其詳細資訊，例如任務名稱、前置任務關係型別和關鍵日期。</p> <p>注意：專案清單中的[!UICONTROL 甘特圖]會顯示跨專案前置任務的相關資訊。 如需有關如何在不同專案之間建立前置任務關係的詳細資訊，請參閱<a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">建立跨專案前置任務</a></p> <p>如需前置任務的詳細資訊，請參閱<a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">強制執行前置任務</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 進度狀態]</td> 
   <td> <p>[!UICONTROL 開啟時間] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__10月_2017.png"></p> <p>[!UICONTROL 落後]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind__10月_2017.png"></p> <p>[!UICONTROL 有風險]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>延遲        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>指定任務目前進度的狀態。 </p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務[!UICONTROL 進度狀態]總覽</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預計日期</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>根據目前已完成的工作加上剩餘工作，標示預計開始和完成日期的預計預計時間表。 </p> <p>如需預計完成日期的詳細資訊，請參閱<a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">專案、任務和問題的預計完成日期總覽</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定顯示選項

1. 移至&#x200B;**工作清單甘特圖**&#x200B;或&#x200B;**專案清單甘特圖**。\
   如需甘特圖所在位置的詳細資訊，請參閱[開始使用[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)。

1. （選用）選取&#x200B;**切換至預計日期**&#x200B;設定，以依據任務的預計日期顯示任務。 依預設，任務會依其計畫日期顯示。
1. 按一下&#x200B;**選項**&#x200B;圖示。 **選項**&#x200B;對話方塊開啟。\
   ![選項.png](assets/options-350x129.png)

1. 選取您要顯示在[!UICONTROL 甘特圖]中的組態選項。

   >[!NOTE]
   >
   > 專案清單[!UICONTROL 甘特圖]中並非所有組態選項都可用。

1. 按一下甘特圖中的任何位置，以關閉&#x200B;**選項**&#x200B;對話方塊。
