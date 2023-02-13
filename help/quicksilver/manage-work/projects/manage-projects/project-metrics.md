---
content-type: overview;how-to-procedural
product-area: projects
keywords: analytics,metrics，專案，enhanced,tasks,assignee,complete,status，逾期，近期
navigation-topic: manage-projects
title: 專案量度概觀
description: 專案量度可讓您以視覺化方式呈現專案中發生的狀況，讓您快速評估專案的需求和狀態。 了解如何解譯專案左側面板的「量度」區域。
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 0%

---

# 專案量度概觀

專案量度可讓您以圖表格式查看專案的執行情形。

## 存取需求

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront授權*</td> 
   <td> <p>審核或更高版本 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>檢視專案的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取專案的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予專案的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的權限</p> <p> 如需專案權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

若要從專案左側面板存取「量度」區域，您必須：

* 在「配置範本」的「專案」區域中啟用「左側面板」選項「量度」。

   若要了解Workfront管理員或群組管理員如何使用版面範本來自訂左側面板，請參閱 [使用版面範本自訂左側面板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## 專案量度區域概觀

專案量度可讓您以視覺化方式呈現專案中發生的狀況，讓您快速評估專案的需求和狀態。

![](assets/project-metrics-full-screen-350x238.png)

在「量度」區域中，您可以看到專案的整體運作狀況，以及：

* 工作處於活動狀態或停止狀態
* 分配了未結工作項的人員
* 任務或問題的詳細資訊，這些任務或問題已過期或接近計畫完成日期

您也可以深入檢視每個圖表，以更密切地查看特定類別中的任務或問題。

若要進一步了解如何查看這些工作或問題，請參閱 [檢視量度詳細資訊](#view-metrics-details).

>[!TIP]
>
>若要查看方案、產品組合等中一組專案的較高層級量度，請導覽至「增強分析」區域。\
>若要進一步了解增強分析，請參閱 [增強的分析概觀](../../../enhanced-analytics/enhanced-analytics-overview.md).

## 專案KPI

關鍵績效指標(KPI)會顯示在「量度」區域的頂端。

![](assets/project-metrics-kpis-350x52.png)

這些KPI可劃分為下列類別：

| 已完成的任務 | **已完成的任務** 顯示處於「完成」狀態的任務數。 此數字還包括具有與完成相當的自訂狀態的任務。 |
|---|---|
| 未完成任務 | **未完成任務** 顯示未處於「完成」或「已關閉」狀態或與「完成」相等的狀態的任務數。 |
| 逾期任務 | **逾期任務** 顯示超過計畫完成日期且未處於「完成」或「已關閉」狀態或與「完成」或「已關閉」相等的狀態的任務數。 |
| 任務總計 | **任務總計** 顯示項目中的任務總數。 |

>[!TIP]
>
>要顯示特定KPI的工作項清單，請按一下該KPI。 在該清單中，您可以按一下特定工作項目，以在新索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱 [檢視量度詳細資訊](#view-metrics-details).

## 任務或問題條形圖

在項目KPI下方顯示的條形圖中，您可以查看項目中工作項的狀態或優先順序。 預設情況下，將選擇任務視圖。

在此圖表中選擇狀態時，您可以查看項目中任務或問題的所有狀態。 每個狀態都會分組成圖表中的長條圖。 此圖表會顯示所有預設系統狀態和自訂狀態。

![](assets/project-metrics-task-issue-by-status-350x120.png)

在此圖表中選擇優先順序時，可以查看項目中任務或問題的所有優先順序。

![](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>要顯示具有特定狀態或優先順序的工作項清單，請按一下圖表中的條。 在該清單中，您可以按一下特定工作項目，以在新索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱 [檢視量度詳細資訊](#view-metrics-details).

## 環圈圖

位於項目KPI下方的環圈圖允許您查看項目中已完成工作項與未完成工作項的比例。

![](assets/tasks-issues-by-complete-status-350x250.png)

在圖表上方的下拉式功能表中，您可以選取：

| 所有任務 | 選取 **任務** 顯示項目中的任務總數，以及已完成任務和未完成任務之間的比率。 |
|---|---|
| 所有問題 | 選取 **問題** 顯示專案中的問題總數，以及已完成和未完成問題之間的比率。 |

>[!TIP]
>
>要顯示已完成或未完成的工作項清單，請按一下環圈圖中的該節。 在該清單中，您可以按一下特定工作項目，以在新索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱 [檢視量度詳細資訊](#view-metrics-details).

## 受託人長條圖

受託人長條圖顯示分配給項目中每個人員的任務數。 此數字會依您從下拉式功能表中選取的類別而異。

![](assets/tasks-issues-by-assignee-350x104.png)

您可以選擇查看以下類別中項目的任務分配：

| 已完成 | 選取 **完成** 顯示已分配給每個用戶的任務數。 |
|---|---|
| 未完成 | 選取 **不完整** 顯示分配給每個用戶的任務數，這些任務尚未完成。 |
| 近期 | 選取 **即將推出** 顯示分配給每個用戶但尚未達到計劃開始日期的任務數。 |
| 已逾期 | 選取 **逾期** 顯示分配給每個用戶的任務數，這些任務已超過計畫完成日期，但尚未完成。 |

>[!TIP]
>
>要顯示指定給特定用戶的選定類別中的工作項目清單，請按一下圖表中用戶名稱旁邊的欄。 在該清單中，您可以按一下特定工作項目，以在新索引標籤中檢視更多詳細資訊。\
>![](assets/completed-tasks-dialog-350x75.png)\
>如需詳細資訊，請參閱 [檢視量度詳細資訊](#view-metrics-details).

## 檢視量度詳細資訊 {#view-metrics-details}

您可以與「度量」區域中的圖表互動，以查看圖表的不同方面，或更密切地查看圖表中的任務和問題。

1. 前往您要查看量度的專案。
1. 在左側面板中，按一下 **顯示更多** 顯示更多區，然後按一下 **量度**.\
   預設情況下，「度量」區域中的圖表顯示任務的資訊。\
   ![](assets/metrics-section-350x298.png)

1. （條件性）如果圖表上顯示下拉箭頭，請按一下 **下拉箭頭** 圖示 ![](assets/dropdown-arrow.png) 在圖表上，從功能表中選取您要的選項。\
   如需每個圖表功能表中顯示之選項的相關資訊，請參閱上方的相關區段。

1. （選用）若要更仔細地查看頁面上任何量度的工作或問題，請執行下列動作：

   1. 按一下要查看詳細資訊的元素，如指派給特定用戶的任務、高優先順序的問題或所有逾期任務。

      任務或問題清單隨即顯示。

      ![](assets/completed-tasks-dialog-350x75.png)

   1. 使用清單底部的箭頭，找出您要查看的任務或問題。

      或

      選擇特定編號以顯示特定頁面上的任務或問題。

      ![](assets/pagination-300x152.png)

   1. 選擇任務或問題以查看更多詳細資訊。

      任務或問題會在新索引標籤中開啟。

1. （選用）若要將專案量度控制面板匯出為.png檔案，請按一下 **匯出** 圖示 ![](assets/export.png)，然後選取 **匯出為PNG** 從下拉式功能表。

   >[!TIP]
   >
   >匯出控制面板時，匯出的檔案只會包含檢視區中目前顯示的內容。 若要在匯出的檔案中加入某些項目，您可能需要在頁面上向上或向下捲動，或調整瀏覽器的縮放設定。
