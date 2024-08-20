---
title: Adobe Workfront Planning物件限制總覽
description: Adobe Workfront Planning限制您可在執行個體中建立的物件數目。 物件限制已生效，可改善產品效能並增強您對Workfront規劃的體驗。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: a2062658110792689c0a15dd1c616c58ebf7e07a
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Adobe Workfront Planning物件限制總覽

Adobe Workfront Planning限制您可在執行個體中建立的物件數目。 物件限制已生效，可改善產品效能並增強您對Workfront規劃的體驗。

下表顯示您可以在Workfront Planning中建立多少物件的限制。 當我們進入下一個開發階段時，限制可能會有所變更。

| Adobe Workfront計畫物件 | 限制 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 一個Workfront例項的工作區數 | 1,000 |
| 一個工作區的區段數 | 50 |
| 一個工作區的記錄型別數 | 1,000 （這包括來自所有區段的記錄型別，以及在使用工作區範本時建立的記錄型別） |
| 一種記錄型別的記錄數 | 50,000 |
| 一種記錄型別或分類法的欄位數 | 500 |
| 文字欄位的字元數 | 1,000個字元 |
| 您可以在記錄型別表格中貼上的檔案大小 | 1MB |
| 您可以透過記錄型別表格的API匯入的檔案大小 | 1.5毫巴 |
| 提出API要求的速率 | 每分鐘200個請求 |
| 您可以匯入的Excel檔案CSV大小* | 5MB |
| 單一使用者可為一個記錄型別建立的檢視次數 | 100 |

<!--add to the table above: Maximum number of views created by one use 100 -->

>[!IMPORTANT]
>
>*此功能已暫時停用，將於稍後提供。

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import** | 5MB |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.
**This functionality has been temporarily disabled and it will be available at a later date.
-->