---
product-area: projects
navigation-topic: manage-projects
title: 將Microsoft專案欄位對應至Adobe Workfront專案
description: Adobe Workfront和Microsoft專案大多相容。 本文說明兩個應用程式中最常見的專案欄位如何彼此對應。
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# 將Microsoft專案欄位對應至Adobe Workfront專案

Adobe Workfront和Microsoft專案大多相容。 使用這兩個應用程式，您可以執行下列操作：

* 從Microsoft專案匯出專案並匯入Workfront
* 從Workfront匯出專案並匯入至Microsoft專案。 

如需有關將專案從Microsoft專案匯入Workfront的詳細資訊，請參閱 [從Microsoft專案匯入專案](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

如需從Workfront匯出專案以匯入Microsoft專案的詳細資訊，請參閱 [將專案匯出至Microsoft專案](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

執行此類資料導入時，必須了解資訊如何從一個應用程式轉換為另一個應用程式。 大部分情況下，您必須在完成匯入後對專案進行一些手動修改。 

## 欄位對應概觀

>[!NOTE]
>
>兩個系統之間的計畫日期不一定對應。 差異可透過排程和Workfront和Microsoft專案之間系統偏好設定的差異來處理。 這些日期差異也可能導致工作量、持續時間和完成百分比的差異。

| **Microsoft專案欄位** | **Workfront欄位** |
|---|---|
| 專案標題 | 專案名稱 |
| 開始和結束日期 | 計畫的開始和完成日期 |
| 任務名稱 | 任務名稱 |
| 任務持續時間 | 任務計畫期間 |
| 任務工作 | 任務計畫小時數 |
| 任務完成% | 任務完成%（根據任務的持續時間） |
| 任務完成% | 任務完成%（根據任務的計畫小時數） |
| 排程的開始和完成 | 計畫的開始和完成日期 |
| 實際開始和結束 | 實際開始和完成日期 |
| 資源名稱 | 任務分配 |
| 分配單位 | 分配分配百分比 |
| 任務說明 | 任務說明 |
| 前置任務 | 前置任務 |

## 未包含的資料概觀

有許多專案欄位未匯入或從Workfront匯出。

這些欄位包括但不限於下列項目：

* 文檔附件
* 自訂欄位（在專案或任務層級）
* Workfront附註
* 問題
* 具有「開始/完成」前置關係的任務出現負滯後（導入任務時沒有滯後）
* 指派
* 任務約束

   >[!NOTE]
   由於「限制」不會對應於Microsoft Project和Workfront，因此請確保任務之間存在前置關係。 否則，任務的計畫起始日期和計畫完成日期在導入的項目中可能不準確。 
