---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 1發行活動
description: 本頁說明2018.2 Beta 1版預覽環境中最近可用的所有變更。 2018年3月22日在預覽環境中提供此功能。 它將於2018年6月在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# 2018.2 Beta 1發行活動

本頁說明2018.2 Beta 1版預覽環境中最近可用的所有變更。 2018年3月22日在預覽環境中提供此功能。 它將於2018年6月在生產環境中提供。

>[!IMPORTANT]
>
>本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.2年度所有變更的清單，請參閱 [2018.2版本活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

2018.2 Beta 1版包含下列增強功能：

* [修改甘特圖中的任務日期](#modify-task-dates-in-the-gantt-chart)
* [從更新索引標籤存取專案甘特圖](#access-the-project-gantt-chart-from-the-updates-tab) （暫時移除）

* [檔案清單上檔案的各種連結重新引入](#various-links-re-introduced-to-documents-on-the-document-list)
* [資源規劃工具中的使用者檢視改善](#user-view-improvements-in-the-resource-planner)
* [新專案清單體驗](#new-project-list-experience)
* [更新索引標籤的新外觀](#new-look-for-updates-tab)
* [行動裝置改良](#mobile-improvements)

## 修改甘特圖中的任務日期 {#modify-task-dates-in-the-gantt-chart}

您現在可以拖曳任務泡泡以變更甘特圖中的規劃開始與規劃完成日期。 透過這項變更，您可以將假設情況套用至專案，而不會影響時間表。

在此變更之前，您只能在工作清單或工作層次中變更工作日期。

如需詳細資訊，請參閱 [更新工作清單甘特圖中的資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## 從更新索引標籤存取專案甘特圖 {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>此功能已暫時從預覽環境中移除。

您現在可以從更新索引標籤存取新專案甘特圖。 當使用者以影響專案時間表的方式變更任務的認可日期時，您可以在專案甘特圖中檢視影響。

在此變更之前，專案時間表連結會開啟舊版甘特圖。

如需詳細資訊，請參閱 [認可日期總覽](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

如需詳細資訊，請參閱 [Portfolio最佳化工具概觀](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## 檔案清單上檔案的各種連結重新引入 {#various-links-re-introduced-to-documents-on-the-document-list}

在18.1版中，從檔案清單的檔案中移除了各種連結，並移至介面的其他區域（有些是檔名稱旁的按鈕，有些是按鈕上的下拉式選單中的）。 在此版本中，將在檔名稱下方重新引入以下連結，現在可在檔案清單中的個別檔案中使用：

* 產生校訂（尚未產生校訂時可用）
* 未完成的校訂（產生校訂時可用）
* 檔案詳細資訊（尚未產生校訂時可用）
* 校訂詳細資訊（產生校訂時可用）
* 列印摘要

在檔案清單中，以下動作不會重新匯入為檔案上的連結：

* 共用（仍可作為功能表中的按鈕）
* 出庫/入庫（仍可在功能表的「更多」下拉式功能表中找到）

如需詳細資訊，請參閱下列章節：

*  
*  在 

## 資源規劃工具中的使用者檢視改善 {#user-view-improvements-in-the-resource-planner}

資源規劃工具的使用者檢視現在包含下列改進：

* 「使用者檢視」現在為預設檢視，取代了「專案檢視」。
* 改善篩選條件，可從整個資料庫擷取資訊，而非僅擷取畫面上的資訊。
* 全熒幕模式。
* 現在效能更快、效率更高。

   * 您可以顯示的使用者、專案、角色及任務數的新限制。
   * 延遲載入，可加快使用者載入速度。

下列功能已在資源規劃工具中暫時停用：

* 使用「使用者檢視」時，從資源規劃工具匯出資料。

在這些改進之前，您報告資源規劃工具載入緩慢，並且您注意到顯示的資料中出現不一致。 透過這些改善功能，這些應該現已淘汰。

如需有關資源規劃工具區域的詳細資訊，請參閱 [資源規劃工具導覽概觀](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## 新專案清單體驗 {#new-project-list-experience}

檢視專案清單時，現在提供新體驗。 此體驗包括提升效能，以及更順暢且更快速的清單導覽。 此新體驗只更新了Workfront專案區域中專案索引標籤中的清單。

大多數情況下，變更會以清單的速度和效率進行。 此外還引進了下列可見變更：

* 清單預設會顯示最多2,000個專案。

  在此增強功能之前，清單顯示100個專案。

* 依預設，群組會摺疊。

  在此變更之前，依預設會展開群組。

* 選取列的區域已展開至整列。

下列功能已在指定的專案清單中暫時停用：

* 調整欄大小（此功能已在2018.2 Beta 5版本中重新引入）
* 欄重新排序
* 狀態圖示欄位顯示為空白（此功能已在2018.2 Beta 5版本中重新引入）
* 無法存取甘特圖（2018.2 Beta 3版本已重新引入此功能）。

如需有關在清單中工作的詳細資訊，請參閱 [開始使用Adobe Workfront中的清單](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## 更新索引標籤的新外觀 {#new-look-for-updates-tab}

>[!NOTE]
>
>對於某些使用者，新的更新索引標籤可能不會顯示在預覽環境中。 我們的開發團隊目前正在疑難排解問題，並致力於儘快解決問題。

「更新」標籤的外觀與操作方式已變更，使其更符合介面的其他區域。 此變更適用於專案、任務、問題和檔案。

下表顯示對「更新」標籤所做的更新：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務</strong> </p> </th> 
   <th> <p><strong>上一個使用者動作</strong> </p> </th> 
   <th> <p><strong>新增使用者動作</strong> </p> </th> 
   <th> <p><strong>如需詳細資訊，請參閱……</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>在時程表上記錄時間</p> </td> 
   <td> <p>按一下記錄時間連結</p> </td> 
   <td> <p>按一下記錄時間按鈕</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">記錄時間</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>在[更新]索引標籤上篩選出系統更新</p> </td> 
   <td> <p>按一下篩選器系統更新連結</p> </td> 
   <td> <p>停用「顯示活動記錄」切換</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>在更新標籤上檢視系統更新</p> </td> 
   <td> <p>按一下「顯示所有更新」</p> </td> 
   <td> <p>啟用「顯示活動記錄」切換</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>在更新或評論上標籤其他使用者</p> </td> 
   <td> <p>按一下「將其他人包含在此更新上」圖示</p> </td> 
   <td> <p>在通知欄位中新增使用者和團隊</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>僅允許貴公司內的使用者檢視物件</p> </td> 
   <td> <p>按一下鎖定圖示</p> </td> 
   <td> <p>啟用「我的公司私人」切換按鈕</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">標籤其他人的更新</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>允許公司外部的使用者檢視物件</p> </td> 
   <td> <p>按一下鎖定圖示</p> </td> 
   <td> <p>停用「私人擁有我的公司」切換按鈕</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">標籤其他人的更新</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>新增回覆或更新至評論或更新</p> </td> 
   <td> <p>按一下評論按鈕</p> </td> 
   <td> <p>按一下回覆或更新按鈕</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任務狀態</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新任務和問題的條件</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">將更新新增至檔案</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 行動裝置改良 {#mobile-improvements}

行動應用程式包含下列增強功能：

* 您在其他行動應用程式中共用的連結，現在會在Workfront行動應用程式中開啟。

  如需共用連結的詳細資訊，請參閱。

  此更新本週有時會發佈到iOS，Android更新應該會在之後不久發佈。

* 我們已更新iOS平台的支援需求，以支援iPhone X。

  如需支援的行動裝置和作業系統的詳細資訊，請參閱。
