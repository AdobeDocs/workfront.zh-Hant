---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 前置任務概觀
description: 前置任務是另一個任務（稱為後置任務或相依任務）所依賴的任務。 Adobe Workfront支援五種型別的前置任務相依性。
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# 前置任務概觀

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

前置任務是另一個任務（稱為後置任務或相依任務）所依賴的任務。 Adobe Workfront支援五種型別的前置任務相依性。 若要瞭解前置任務相依性，請參閱 [作業相依性型別的概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## 前置任務概觀

瞭解前置任務功能對於瞭解專案中的時間表非常重要。

任務前置任務關係存在於單一專案中的任務之間以及不同專案中的任務之間。

在多專案相依性的情況下，您可以在來自兩個不同專案的任務之間建立跨專案前置任務。

不論前置任務和後續任務屬於同一專案還是屬於兩個不同的專案，每個專案的相依性和時間表的計算方式都相同。

關於前置任務，專案時間表受下列影響：

* 前置任務相依性
* 延遲值與型別\
  如需相依性和延遲的詳細資訊，請參閱 [任務清單中的前置任務值範例](#examples-of-predecessor-values-in-a-task-list).

  例如，如果任務A是完成 — 開始關係中任務B的前置任務，而任務B具有儘快的任務限制，則Workfront會在任務A的計畫完成日期之後立即指派任務B的計劃開始日期，無論前置任務是否已強制執行。

若要瞭解前置任務關係，您必須瞭解：

* **相依性型別：** 前置任務由各種相依性型別連結。 如需相依性型別的詳細資訊，請參閱 [作業相依性型別的概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **強制前置任務：** 強制實施前置任務時，前置任務完成之前後置任務絕對不能開始。 後續任務會在前置任務完成後立即顯示為「開始」。

  當前置任務未完成（或已開始）且未強制執行時，後續任務可以開始，但專案時間表仍受前置任務和後續任務日期的影響。

  如果有強制的前置任務，Workfront不允許在前置任務完成之前，將後續任務標示為「進行中」或「完成」。

  但是，Workfront允許針對任務報告時數。\
  如需強制前置任務的詳細資訊，請參閱 [強制執行前置任務](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **延遲：** 您可以在相依性中建立延遲，這會造成前置任務完成後以及後續任務開始之前必須發生的延遲。 延遲會影響專案的時間表。

  若要瞭解延遲型別，請參閱 [延遲型別概觀](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## 建立前置任務關係

若要建立前置任務，請參閱下列任一文章：

* 若要使用任務的「前置任務」標籤來建立前置任務，請參閱 [使用前置任務區域建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* 若要在任務清單中建立前置任務，請參閱 [在任務清單上建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* 若要透過鏈結任務來建立前置任務關係，請參閱 [透過鏈結任務建立前置任務關係](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* 若要建立跨專案前置任務，請參閱 [建立跨專案前置任務](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## 找出任務的前置任務 {#locate-the-predecessors-of-a-task}

若要尋找任務的前置任務，請執行下列任一項作業：

* 前往您正在處理的專案，然後執行下列動作：

   1. 尋找您要尋找前置任務的工作，然後按一下該工作。
   1. 按一下 **前置任務** 在左側面板中。 您可能需要按一下 **顯示更多**，然後 **前置任務**.
   1. 前置任務所在的專案名稱會顯示在 **專案** 欄。

      中的數字 **#** 欄顯示前置任務任務編號。 例如，「6」表示專案中的第六個任務。

      ![任務的前置任務區域](assets/predecessors-area-with-task-header.png)

* 前往您正在處理的專案，然後執行下列動作：

   1. 按一下 **任務** 標籤。
   1. 選擇 **標準檢視** 位於工作清單頂端。
   1. 此 **前置任務** 欄顯示前置任務任務編號。

      對於跨專案前置任務，「前置任務」欄會顯示前置任務所屬專案的參考編號，以及以冒號分隔的任務編號。

      前置任務被標示為完成時，前置任務圖示會變成綠色。 這表示相依任務已準備好工作。

      將滑鼠指標暫留在此值上，即可取得前置任務、專案和日期的詳細資訊。

      ![前置任務詳細資訊](assets/predecessor-details-in-task-list.png)

## 任務清單中的前置任務值範例 {#examples-of-predecessor-values-in-a-task-list}

當您在任務清單中檢視前置任務時，您可能會看到下列任何型別的前置任務及其各自的「相依性型別」和「延遲」金額：

* **1fs -** 前置任務編號為1。 相依性型別為「完成 — 開始」。 在專案時間表中，此任務排程為任務1完成後立即開始。 儘管如此，仍可將其標籤為「進行中」或「完成」。
* **1 -** 前置任務編號為1。 這與 **1fs**，因為 **fs** 是Workfront中的預設前置任務關係。

* **1fse -** 前置任務編號為1。 相依性型別是Finish-Start-Enforced。 在專案時間表中，此任務會在任務1完成後立即開始顯示。 在任務1完成之前，Workfront不允許將其標籤為進行中或完成。 但是，Workfront允許針對任務報告時數。
* **1fs+3d -** 前置任務編號為1。 相依性型別為「完成 — 開始」，延遲時間為3天。 在專案時間軸中，此任務會在任務1完成後3個工作日開始顯示。
* **1fs-3d -** 前置任務編號為1。 相依性型別為「完成 — 開始」，延遲時間為3天。 在專案時間表中，此任務會顯示為前置任務完成前3個工作天的開始。
* **1fs+3de**  — 前置任務編號為1。 相依性型別為「完成 — 開始 — 強制」，延遲時間為3天。 在專案時間軸中，此任務會在任務1完成後3個工作日開始顯示。 在任務1完成之前，Workfront不允許將其標籤為進行中或完成。 但是，Workfront允許針對任務報告時數。

  >[!NOTE]
  >
  >您必須新增強制值(**è**)，而不是前置任務。

* **4515:2** 前置任務編號為2。  — 這是專案中前置任務的「完成開始」、非強制相依性及參考編號 **4515**.

## 檢視前置任務資訊

您可以在Workfront的下列區域中檢視前置任務資訊。 此包含跨專案前置任務的相關資訊：

* 在任務層級的「前置任務」區段。

  如需在「前置任務」區段中檢視前置任務資訊的詳細資訊，請參閱區段 [找出任務的前置任務](#locate-the-predecessors-of-a-task) 本文章內容。

* 在甘特圖中。

  如需有關在甘特圖中顯示前置任務的資訊，請參閱 [設定資訊在甘特圖上的顯示方式](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* 在任務清單中。

  若要在任務清單中檢視您任務的前置任務相關資訊，您可以執行下列任一項作業：

   * 在工作清單中套用內建的標準檢視。

     如需有關在「標準」檢視中檢視前置任務資訊的資訊，請參閱區段 [找出任務的前置任務](#locate-the-predecessors-of-a-task) 本文章內容。

   * 建立任務檢視或報告，並將「前置任務」欄新增到該檢視。

     如需有關建立具有前置任務資訊之任務的自訂檢視的詳細資訊，請參閱 [檢視：前置任務詳細資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* 在存取任務時位於任務標題中。

  ![](assets/qs-predecessor-info-in-task-header-350x141.png)
