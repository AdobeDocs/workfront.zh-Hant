---
content-type: overview;how-to-procedural
product-area: projects
keywords: 分析，量度，專案，任務，受指派人，完成，狀態，過期，近期
navigation-topic: manage-projects
title: 專案量度概觀
description: 專案量度可讓您以視覺效果呈現專案中發生的事件，讓您快速評估專案的需求和狀態。 瞭解如何解讀專案左側面板中的量度區域。
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: 78b4724ca8d5df15ed76e9e882179e3cb127282c
workflow-type: tm+mt
source-wordcount: '1163'
ht-degree: 0%

---

# 專案量度概觀

專案量度以圖表格式提供您專案執行方式的一般檢視。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront授權*</td> 
   <td> <p>新增：淺色或更高 </p>
   <p>目前：檢閱或以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

若要從專案的左側面板存取量度區域，您必須：

* 在版面配置範本的專案區域中啟用左側面板選項量度。

  若要瞭解Workfront管理員或群組管理員如何使用配置範本來自訂左側面板，請參閱[使用配置範本來自訂左側面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)。

## 專案量度區域概觀

專案量度可讓您以視覺效果呈現專案中發生的事件，讓您快速評估專案的需求和狀態。

![](assets/project-metrics-full-screen-350x238.png)

在量度區域中，您可以檢視專案的整體健康情況，以及：

* 工作進行中或停止的位置
* 誰擁有指派給他們的未完成工作專案
* 逾期或接近計畫完成日期的任務或問題詳細資訊

您也可以深入研究每個圖表，以更密切地檢視特定類別中的任務或問題。

若要深入瞭解檢視這些工作或問題，請參閱[檢視量度詳細資料](#view-metrics-details)。

<!--this was deprecated: 
>[!TIP]
>
>To see metrics at a higher level for a group of projects within a program, portfolio, etc., navigate to the Enhanced analytics area.  
>To learn more about Enhanced analytics, see [Enhanced analytics overview](../../../enhanced-analytics/enhanced-analytics-overview.md).-->

## 專案KPI

關鍵績效指標(KPI)會顯示在量度區域的頂端。

![](assets/project-metrics-kpis-350x52.png)

這些KPI可劃分為下列類別：

| 已完成的任務 | **已完成的工作**&#x200B;顯示處於完成狀態的任務數目。 此數字也包含具有自訂狀態（等同於完成）的任務。 |
|---|---|
| 未完成的任務 | **未完成任務**&#x200B;顯示未處於「完成」或「已關閉」狀態，或等同於「完成」狀態的任務數。 |
| 超期任務 | **逾期任務**&#x200B;顯示超過計畫完成日期且未處於「完成」或「已關閉」狀態，或等同於「完成」或「已關閉」狀態的任務數。 |
| 任務總數 | **任務總數**&#x200B;顯示專案中的任務總數。 |

>[!TIP]
>
>若要顯示特定重要績效指標的工作專案清單，請按一下該重要績效指標。 在該清單中，您可以按一下特定工作專案以在新的索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱[檢視量度詳細資料](#view-metrics-details)。

## 任務或問題長條圖

在專案KPI下方顯示的長條圖中，您可以檢視專案中工作專案的狀態或優先順序。 預設會選取工作檢視。

在此圖表中選取狀態時，您可以檢視專案中所有任務或問題的狀態。 每個狀態都會分組到圖表中的長條圖中。 所有預設系統狀態和自訂狀態都會顯示在此圖表中。

![](assets/project-metrics-task-issue-by-status-350x120.png)

在此圖表中選取優先順序時，您可以檢視專案中任務或問題的所有優先順序。

![](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>若要顯示具有特定狀態或優先順序的工作專案清單，請按一下圖表中的長條圖。 在該清單中，您可以按一下特定工作專案以在新的索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱[檢視量度詳細資料](#view-metrics-details)。

## 環形圖

位於專案KPI下方的環形圖可讓您檢視專案中已完成工作專案與未完成工作專案的比率。

![](assets/tasks-issues-by-complete-status-350x250.png)

在圖表上方的下拉式功能表中，可以選取：

| 所有任務 | 選取&#x200B;**任務**&#x200B;會顯示專案中的任務總數，以及已完成和未完成任務之間的比率。 |
|---|---|
| 所有問題 | 選取&#x200B;**個問題**&#x200B;會顯示專案中的問題總數，以及已完成和未完成問題之間的比率。 |

>[!TIP]
>
>若要顯示已完成或未完成的工作專案清單，請按一下環形圖中的該區段。 在該清單中，您可以按一下特定工作專案以在新的索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱[檢視量度詳細資料](#view-metrics-details)。

## 被指定者長條圖

受指派人長條圖顯示指派給專案中每個人的任務數量。 此數字會因您從下拉式功能表中選取的類別而異。

![](assets/tasks-issues-by-assignee-350x104.png)

您可以選擇檢視下列類別中專案的作業指派：

| 完成 | 選取&#x200B;**完成**&#x200B;會顯示指派給每位使用者已完成的工作數量。 |
|---|---|
| 未完成 | 選取&#x200B;**未完成**&#x200B;會顯示指派給每個使用者但尚未完成的任務數目。 |
| 近期 | 選取「**近期**」會顯示指派給每個使用者但尚未達到計劃開始日期的任務數。 |
| 已逾期 | 選取&#x200B;**過期**&#x200B;會顯示指派給每個使用者的已超過計畫完成日期但尚未完成的任務數。 |

>[!TIP]
>
>若要顯示所選類別中指派給特定使用者的工作專案清單，請按一下圖表中使用者名稱旁的橫條。 在該清單中，您可以按一下特定工作專案以在新的索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱[檢視量度詳細資料](#view-metrics-details)。

## 檢視量度詳細資料 {#view-metrics-details}

您可以與「量度」區域中的圖表互動，以檢檢視表的不同方面，或更密切地檢檢視表內的任務和問題。

1. 前往您要檢視其量度的專案。
1. 在左側面板中，按一下&#x200B;**度量**。\
   依照預設，「測量結果」區域中的圖表會顯示工作的資訊。\
   ![](assets/metrics-section-350x298.png)

1. （視條件而定）如果圖表上顯示下拉箭頭，請按一下圖表上的&#x200B;**下拉箭頭**&#x200B;圖示![](assets/dropdown-arrow.png)，然後從選單中選取您想要的選項。\
   如需每個圖表功能表中選項的相關資訊，請參閱上方的相關區段。

1. （可選）若要更密切地檢視頁面上任何量度的任務或問題，請執行下列動作：

   1. 按一下您要檢視詳細資訊的元素，例如指派給特定使用者的任務、高優先順序的問題或所有逾期任務。

      任務或問題清單隨即顯示。

      ![](assets/completed-tasks-dialog-350x75.png)

   1. 使用清單底部的箭頭來找出您要檢視的任務或問題。

      或

      選取特定數字，以在特定頁面上顯示任務或問題。

      ![](assets/pagination-300x152.png)

   1. 選取一個任務或問題以檢視更多詳細資料。

      任務或問題會在新標籤中開啟。

1. （選擇性）若要將專案度量儀表板匯出至.png檔案，請按一下&#x200B;**匯出**&#x200B;圖示![](assets/export.png)，然後從下拉式選單中選取&#x200B;**匯出為PNG**。

   >[!TIP]
   >
   >匯出圖示板時，匯出的檔案僅包含目前顯示在檢視區中的內容。 若要在匯出的檔案中加入某些專案，您可能需要在頁面上上下捲動，或調整瀏覽器的縮放設定。
