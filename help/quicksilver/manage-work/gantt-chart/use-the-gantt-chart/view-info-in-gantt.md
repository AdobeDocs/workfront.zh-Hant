---
navigation-topic: use-the-gantt-chart
title: 檢視[!UICONTROL 甘特圖]中的資訊
description: 任務清單甘特圖和專案清單甘特圖會顯示有關專案和任務的資訊。
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# 檢視[!UICONTROL 甘特圖]中的資訊

任務清單[!UICONTROL 甘特圖]和專案清單[!UICONTROL 甘特圖]顯示有關專案和任務的資訊。

## 存取需求

您必須具備下列專案才能依照本文所述步驟操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權概述*</td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL檢視]或更高的專案和任務存取權</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否已在您的存取層級中設定其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[！UICONTROL檢視]或更高的專案存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 找到[!UICONTROL 甘特圖]

您可以從Workfront內的多個區域找到工作清單甘特圖和專案清單[!UICONTROL 甘特圖]。 如需詳細資訊，請參閱[開始使用[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)。

## 檢視[!UICONTROL 重要路徑]上的工作

在專案清單[!UICONTROL 甘特圖]中，不在[!UICONTROL 關鍵路徑]上的任務會顯示為淺藍色水平線。 位於專案[!UICONTROL 關鍵路徑]上的任務會顯示為紅色水平線。

如需[!UICONTROL 關鍵路徑]上任務的詳細資訊，請參閱[專案概述[!UICONTROL 關鍵路徑]](../../../manage-work/tasks/manage-tasks/critical-path.md)。

## 檢視專案清單[!UICONTROL 甘特圖]中的任務資訊

您可以直接從「專案清單」檢視專案的工作資訊。 任務會列在每個專案的名稱下。

>[!NOTE]
>
>您無法從專案清單[!UICONTROL 甘特圖]編輯任務。

您可以直接從下列區域的專案清單中檢視專案的工作資訊：

* 在[!UICONTROL 專案]區域中
* 在Portfolio內
* 在計畫內

若要從專案清單檢視專案中的任務：

1. 前往上述其中一個區域。

   例如，從[!UICONTROL 主功能表]，按一下&#x200B;**[!UICONTROL 專案]**。

   專案清單隨即顯示。

1. 按一下畫面右上角的&#x200B;**[!UICONTROL 甘特圖]**&#x200B;圖示![](assets/gantt-icon-nwe.png)。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. 按一下&#x200B;**[!UICONTROL 顯示工作清單]**&#x200B;圖示。

1. 在左側的專案清單中，按一下專案名稱旁邊的下拉箭頭，以顯示該專案下的任何任務。\
   這會在[!UICONTROL 甘特圖]上顯示任務資訊。\
   ![Show_task_list_enabled_project_expanded.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. （選擇性）按一下右上角的&#x200B;**[!UICONTROL 列印]**&#x200B;圖示以匯出[!UICONTROL 甘特圖]。

   >[!NOTE]
   >
   >專案清單[!UICONTROL 甘特圖]僅匯出專案。 未包含任務資訊。

## 變更資訊顯示在[!UICONTROL 甘特圖]中的時段

您可以調整[!UICONTROL 甘特圖]上顯示的時間段來顯示精細層級的資訊，或者您可以快速瀏覽至日、周、月、季或年檢視：

* [在精細層次變更時段](#change-the-time-period-on-a-granular-level)
* [依日、周、月、季或年檢視資訊](#view-information-by-day-week-month-quarter-or-year)

### 在精細層次變更時段 {#change-the-time-period-on-a-granular-level}

1. 將游標暫留在[!UICONTROL 甘特圖]的時間表上，然後從左到右拖曳縮放指示器，以展開或收縮時間表。\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### 依日、周、月、季或年檢視資訊 {#view-information-by-day-week-month-quarter-or-year}

1. 在[!UICONTROL 甘特圖]中，按一下時間範圍下拉式功能表。

   ![](assets/timeline-options.png)

1. 從下列可用選項中選取時間範圍：

   * **[!UICONTROL 適合全部]**：此選項會顯示整個專案的時間線。
   * **[!UICONTROL 所有專案]**：此選項僅在專案清單甘特圖中可用。
   * **[!UICONTROL 年]**
   * **[!UICONTROL 季]**
   * **[!UICONTROL 個月]**
   * **[!UICONTROL 周]**
   * **[!UICONTROL 天]**

1. （選擇性）選取更細微的時間範圍，例如[!UICONTROL 周]或[!UICONTROL 天]，然後按一下並拖曳[!UICONTROL 甘特圖]底部的水準卷軸，在專案的時間線上從左到右移動。\
   [!UICONTROL 甘特圖]的時間表快照集隨即顯示，以顯示整個專案。

   >[!TIP]
   >
   >時間軸快照只有在您按一下水準卷軸之後才會顯示。

   ![stretchy_gantt_minimap_with_outline__1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. （可選）按一下時間線快照內的任何位置，以瀏覽至專案生命週期中的特定點。\
   或\
   拖曳快照檢視器的控制代碼，以選取特定的時間線範圍，將其顯示在主要[!UICONTROL 甘特圖]中。

## 使用篩選器、檢視和群組

[!UICONTROL 甘特圖]是目前顯示在工作清單中的資訊的視覺化表示法。 您可以將篩選器、檢視和群組套用至[!UICONTROL 甘特圖]中列出的物件。

>[!CAUTION]
>
>當您選取[!UICONTROL 手動]儲存[!UICONTROL 時間表計畫]以儲存對您工作清單的變更時，無法套用篩選器、檢視和群組。 如需有關儲存清單中工作變更的資訊，請參閱[在清單中編輯工作](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)。

您套用至清單的篩選器和群組會反映在專案清單和工作清單[!UICONTROL 甘特圖]上，也會在匯出甘特圖時納入：

* 篩選器\
   您可以套用篩選器至清單，以控制[!UICONTROL 甘特圖]中顯示的資訊。\
   如需套用篩選的詳細資訊，請參閱[篩選總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

* 群組\
   您套用至清單的群組會反映在[!UICONTROL 甘特圖]上。\
   如需套用群組的相關資訊，請參閱Adobe Workfront中的[群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

檢視未反映在[!UICONTROL 甘特圖]上。 不過，當您匯出[!UICONTROL 甘特圖] (如[將[!UICONTROL 甘特圖]匯出至PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)中所述)時，除了[!UICONTROL 甘特圖]之外，也會匯出工作清單，並將目前的檢視套用至清單。

## 設定顯示選項

您可以選擇在兩個[!UICONTROL 甘特圖]中顯示的資訊型別。 如需詳細資訊，請參閱[設定資訊在[!UICONTROL 甘特圖]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上的顯示方式。
