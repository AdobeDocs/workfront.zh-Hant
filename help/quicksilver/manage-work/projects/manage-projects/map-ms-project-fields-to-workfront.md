---
product-area: projects
navigation-topic: manage-projects
title: 將Microsoft專案欄位對應至Adobe Workfront專案
description: Adobe Workfront中的專案與Microsoft專案大多相容。 本文說明這兩個應用程式中最常見的專案欄位如何相互對應。
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# 將Microsoft專案欄位對應至Adobe Workfront專案

Adobe Workfront中的專案與Microsoft專案大多相容。 使用這兩個應用程式，您可以執行下列動作：

* 從Microsoft專案匯出專案，並將其匯入Workfront
* 從Workfront匯出專案，並將其匯入Microsoft專案。 

如需有關將專案從Microsoft專案匯入到Workfront的詳細資訊，請參閱[從Microsoft專案匯入專案](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)。

如需從Workfront匯出專案以匯入Microsoft專案的詳細資訊，請參閱[將專案匯出至Microsoft專案](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)。

執行這類資料匯入時，請務必瞭解資訊如何從一個應用程式轉譯為另一個應用程式。 大多數時候，您必須在完成匯入後，對專案進行一些手動修改。 

## 欄位對應概觀

>[!NOTE]
>
>計畫日期並非總是對應至兩個系統。 差異可透過Workfront和Microsoft專案之間的排程和系統偏好設定差異來解釋。 這些日期差異也會造成工作量、持續時間和完成百分比的差異。

| **Microsoft專案欄位** | **Workfront欄位** |
|---|---|
| 專案標題 | 專案名稱 |
| 開始和完成日期 | 計劃開始與完成日期 |
| 任務名稱 | 任務名稱 |
| 任務期間 | 任務計畫期間 |
| 任務工作 | 任務計畫時數 |
| 任務%完成 | 任務完成百分比（根據任務期間） |
| 任務工作%完成 | 任務完成百分比（根據任務的計畫時數） |
| 已排程的開始和完成 | 計劃開始與完成日期 |
| 實際開始與完成 | 實際開始與完成日期 |
| 資源名稱 | 任務指派 |
| 工作分派單位 | 指派分配百分比 |
| 任務備註 | 任務說明 |
| 前置任務 | 前置任務 |

## 未包括的資料概觀

有許多專案欄位不會匯入或匯出Workfront。

這些欄位包含但不限於下列專案：

* 檔案附件
* 自訂欄位（專案或任務層級）
* Workfront附註
* 問題
* 具有「開始/完成」前置任務關係之任務的負延遲（任務匯入時沒有延遲）
* 指派
* 任務限制

  >[!NOTE]
  >
  >由於限制無法在Microsoft專案和Workfront之間對應，請確定任務之間有前置任務關係。 否則，任務的計劃開始和計畫完成日期在匯入的專案中可能不準確。 
