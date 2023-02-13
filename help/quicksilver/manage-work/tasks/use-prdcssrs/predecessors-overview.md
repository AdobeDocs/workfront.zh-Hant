---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 任務前置任務概述
description: 前置任務是另一個任務（稱為後繼任務或從屬任務）所依賴的任務。 Adobe Workfront支援五種舊版相依性。
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# 任務前置任務概述

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

前置任務是另一個任務（稱為後繼任務或從屬任務）所依賴的任務。 Adobe Workfront支援五種舊版相依性。 若要了解前置項的相依性，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## 前置任務概述

了解前身功能對於了解專案的時間軸非常重要。

任務之間的前置關係既存在於單個項目中，也存在於多個項目中。

在多項目依賴的情況下，可以建立跨項目前置任務。

無論前置任務和後繼任務屬於同一項目還是屬於兩個不同的項目，依賴項和時間表都以相同的方式計算。

若是前置作業，專案時間軸會受到下列項目影響：

* 前置相依性
* 延遲值和類型\
   如需相依性和延遲的詳細資訊，請參閱 [任務清單中的前置值示例](#examples-of-predecessor-values-in-a-task-list).

例如，如果任務A是完成 — 開始關係中任務B的前置任務，且任務B的任務約束為「盡快」，則Workfront會在任務A的計畫完成日期之後立即為任務B分配計畫起始日期，而不管前置任務是否被強制。

要了解前身關係，您必須了解：

* **相依性類型：** 前置項由各種依賴項類型連結。 如需相依性類型的詳細資訊，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **執行前身：** 實施前置任務時，在前置任務完成之前，後置任務無法啟動。 後續任務在前置任務完成後立即顯示為開始。

   在前置作業完成之前，Workfront不會將其標示為「進行中」或「完成」。 但Workfront則允許在工作上報告數小時。\
   有關強制執行前置任務的詳細資訊，請參閱 [強制前置作業](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **滯後：** 您可以在相依性中建立滯後，這會造成必須在前置任務完成之後以及後繼任務開始之前發生的延遲。 滯後影響項目的時間表。

   若要了解延遲類型，請參閱 [延遲類型概觀](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## 建立前置關係

若要建立前置文章，請參閱下列任一文章：

* 要使用任務的「前置任務」頁簽建立前置任務，請參閱 [使用前置任務區域建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* 要在任務清單中建立前置任務，請參閱 [在任務清單上建立前置關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* 要通過連結任務建立前置任務關係，請參閱 [通過連結任務建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* 要建立跨項目前置任務，請參閱 [建立跨專案的前置項目](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## 查找任務的前置任務 {#locate-the-predecessors-of-a-task}

要查找任務的前置任務，請執行以下操作之一：

* 前往您正在處理的專案，並執行下列動作：

   1. 查找要為其查找前置任務的任務，然後按一下該任務。
   1. 按一下 **前置任務** 中。 您可能需要按一下 **顯示更多**，然後 **前置任務**.
   1. 前身所在的專案名稱會顯示在 **專案** 欄。

      中的數字 **#** 列顯示前置任務編號。 例如，「6」表示專案中的第六個任務。

      ![任務的前置任務部分](assets/predecessors-area-with-task-header.png)

* 前往您正在處理的專案，並執行下列動作：

   1. 按一下 **工作** 標籤。
   1. 選擇 **標準檢視** 在任務清單的頂部。
   1. 此 **前置任務** 列顯示前置任務編號。

      對於跨項目前置項，前置項列顯示前置項所屬項目的引用編號和任務編號，用冒號分隔。

      前置任務標籤為完成時，前置任務表徵圖將變為綠色。 這表示相依任務已準備就緒可供使用。

      將滑鼠指標暫留在此值上，可取得前置項目、日期的詳細資訊。

      ![前置任務詳細資訊](assets/predecessor-details-in-task-list.png)

## 任務清單中的前置值示例 {#examples-of-predecessor-values-in-a-task-list}

在任務清單中查看前置任務時，您可能會看到以下任一類型的前置任務及其各自的「相依類型」和「滯後」金額：

* **1fs -** 前置任務編號為1。 相依性類型為「完成開始」。 在項目時間軸中，此任務被安排在任務1完成後立即開始。 儘管如此，它仍可標示為進行中或完成。
* **1 -** 前置任務編號為1。 這等同於 **1fs**，因為 **fs** 是Workfront中的預設前置關係。

* **1fse -** 前置任務編號為1。 依賴項類型為「完成開始」(Finish-Start-Enforced)。 在項目時間軸中，此任務在任務1完成後立即顯示為開始。 Workfront不允許在任務1完成之前將其標示為「進行中」或「完成」。 但Workfront則允許在工作上報告數小時。
* **1fs+3d -** 前置任務編號為1。 相依性類型為「完成 — 開始」，延遲時間為3天。 在項目時間表中，此任務在任務1完成後的3個工作日內顯示為開始。
* **1fs-3d -** 前置任務編號為1。 相依性類型為「完成 — 開始」，延遲時間為3天。 在項目時間表中，此任務顯示為在前一個任務完成前3個工作日開始。
* **1fs+3de**  — 前置任務編號為1。 相依性類型為「完成 — 開始 — 強制」，延遲時間為3天。 在項目時間表中，此任務在任務1完成後的3個工作日內顯示為開始。 Workfront不允許在任務1完成之前將其標籤為「進行中」或「完成」。 但Workfront則允許在工作上報告數小時。

   >[!NOTE]
   >
   >強制值(**e**)，而非前身。

* **4515:2** 前置任務編號為2。  — 這是「完成至開始」，與項目中的前置項沒有強制的依賴關係，並帶有引用編號 **4515**;前置任務編號為 **2**.

## 查看前置資訊

您可以在Workfront的下列區域中檢視前置資訊。 這包括跨專案前置作業的相關資訊：

* 在任務級別，在前置任務部分。

   如需在前置項區段中檢視前置項資訊的相關資訊，請參閱區段 [查找任務的前置任務](#locate-the-predecessors-of-a-task) 這篇文章。

* 在甘特圖中。

   有關在甘特圖中顯示前置作業的資訊，請參見 [配置資訊在甘特圖上的顯示方式](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* 在任務清單中。

   要在任務清單中查看有關任務前置任務的資訊，可以執行以下操作之一：

   * 在任務清單中應用內置的標準視圖。

      有關在「標準」視圖中查看前置資訊的資訊，請參閱 [查找任務的前置任務](#locate-the-predecessors-of-a-task) 這篇文章。

   * 建立任務視圖或報告，並將前置項列添加到該視圖。

      有關使用前置資訊為任務建立自定義視圖的詳細資訊，請參見 [查看：前置詳細資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* 訪問任務時在任務標題中。

   ![](assets/qs-predecessor-info-in-task-header-350x141.png)
