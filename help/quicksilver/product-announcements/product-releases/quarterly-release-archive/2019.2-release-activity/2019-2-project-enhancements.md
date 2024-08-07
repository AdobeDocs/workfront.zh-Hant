---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2專案增強功能
description: 本頁說明2019.2版本隨附的所有專案增強功能。 此功能計畫在2019年5月20日當週的生產環境中可用。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# 2019.2專案增強功能

本頁說明2019.2版本隨附的所有專案增強功能。 此功能計畫在2019年5月20日當週的生產環境中可用。

如需2019.2年度所有變更的清單，請參閱[2019.2年度發行活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md)。

## 自訂狀態時更快找到群組

「設定」區域中「狀態」標籤上的下拉式功能表現在是預先輸入功能表。 這可讓您快速搜尋和尋找系統中的任何群組，讓您更輕鬆地自訂狀態。

以前，下拉式選單顯示的群組數量有限。 如果您想要的群組未顯示，您必須導覽至「設定>群組」 ，並尋找特定群組以自訂群組的狀態。

如需詳細資訊，請參閱[建立或編輯狀態](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

## 將預設自訂Forms和核准流程附加至任務

您現在可以設定預設自訂表單和核准流程，以便在您將任務新增到專案時附加到任務。 您可以在專案層級進行預設設定。

如需有關在專案層級為任務設定預設自訂表單和核准流程的資訊，請參閱[編輯專案](../../../../manage-work/projects/manage-projects/edit-projects.md)文章中的「任務」一節。

## 在工作清單中以粗體顯示父系工作的整列

在工作清單中，包含父系工作的列會以粗體顯示。 當清單按「工作細目」結構或按「任務編號」遞增順序排序時，此變更會顯示。

## 反轉工作清單上的變更

工作清單上的新「自動儲存」按鈕可讓您選取是否要自動儲存所做的變更，或是否要先檢視變更的儲存效果。 此設定會同時套用至工作清單和甘特圖。

在此增強功能之前，所有變更一律會自動儲存。

如需有關編輯工作清單中工作的資訊，請參閱[編輯工作](../../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

如需有關編輯甘特圖中的工作的資訊，請參閱工作清單甘特圖中的[更新資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)。

## 新清單中的新欄寬預設值

現在，Workfront會根據每欄的值格式資訊，自動調整欄寬。 例如，顯示數字的欄比顯示「說明」欄位的欄寬。

在此改善之前，除非另有指定，否則新專案和工作檢視中的欄寬設定為100畫素。

如需欄寬的相關資訊，請參閱[修改欄寬和順序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

## 停用未使用的物件

>[!NOTE]
>
>此功能在2019.2預覽時間範圍內直接發佈到生產環境。

如果您有不再使用的物件，您現在可以停用它們以從清單中隱藏它們，以防止使用者將它們與其他物件產生關聯。

現在，當您編輯下列任何物件時，可以指出它們是否應該作用中。 設定為「作用中」的物件會出現在下拉式選單和預先輸入欄位中，並可附加到其他物件。 未設定為「作用中」的物件在下拉式選單和要附加至其他物件的預先輸入欄位中不可見。

* 核准程序
* 公司
* 自訂表單
* 里程碑路徑
* 專案組合
* 計劃
* 範本

您停用目前使用之任何專案仍會如常運作，且不會移除或封鎖。

>[!IMPORTANT]
>
>透過Workfront API建立這些物件時，「isActive」引數的預設值為true。 這是所有物件的新欄位，您無法在API 11版之前編輯。 此欄位先前在Portfolio中確實存在，但預設值為false；從API版本11開始，它會變更為預設值true。

## 在檢視表中顯示已排程工作(BCWS)與已執行工作(BCWP)的預算成本

您現在可以在專案與任務檢視中顯示「已排程工作的預算成本(BCWS)」與「已執行工作的預算成本(BCWP)」。

雖然這些專案績效量度以前用於Workfront的財務計算，但在此增強功能之前，無法在系統中看到。

如需有關計算BCWS的資訊，請參閱[計算排定工作的預算成本(BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md)。

如需有關計算BCWP的資訊，請參閱[計算已執行工作的預算成本(BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md)。

