---
title: Adobe Workfront Planning物件限制總覽
description: Adobe Workfront Planning限制您可在執行個體中建立的物件數目。 物件限制已生效，可改善產品效能並增強您對Workfront規劃的體驗。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 1%

---

<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Adobe Workfront Planning物件限制總覽

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}


Adobe Workfront Planning限制您可在執行個體中建立的物件數目。 物件限制已生效，可改善產品效能並增強您對Workfront規劃的體驗。

下表顯示您可以在Workfront Planning中建立多少物件的限制。 當我們進入下一個開發階段時，限制可能會有所變更。

| Adobe Workfront計畫物件 | 限制 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 一個Workfront例項的工作區數 | 無限制* |
| 一個工作區的區段數 | 50 |
| 一個工作區的記錄型別數 | 1,000 （這包括來自所有區段的記錄型別，以及在使用工作區範本時建立的記錄型別） |
| 一種記錄型別的記錄數 | 25,000 |
| 一個工作區的記錄數 | 25,000適用於計畫為<br>的客戶500,000適用於計畫為Planning Plus的客戶 |
| Workfront Planning單一例項的總記錄數 | 500,000 （針對計畫計畫為<br>200,000）的客戶（針對計畫為Planning Plus的客戶） |
| 一種記錄型別或分類法的欄位數 | 500 |
| 單行文字欄位的字元數 | 1,000個字元 |
| 段落欄位的字元數 | 10,000字元 |
| 一種記錄型別的段落欄位數 | 20個段落欄位 |
| 您可以在記錄型別表格中貼上的檔案大小 | 1MB |
| 您可以透過記錄型別表格的API匯入的檔案大小 | 1.5毫巴 |
| 提出API要求的速率 | 每分鐘200個請求 |
| 單一使用者可為一個記錄型別建立的檢視次數 | 100 |
| CSV的Excel檔案大小，您可以匯入以建立記錄型別 | 5MB |
| <span class="preview">您可以匯入CSV或Excel檔案以建立記錄型別的列數</span> | 10,000 |
| <span class="preview">您可以匯入CSV或Excel檔案以建立記錄型別的欄數</span> | 500 |

*我們建議您不要有太多工作區，因為這些工作區可能會變得難以管理，而且您的工作流程可能太分散。

如需Workfront Planning定價與封裝的相關資訊，請參閱[Adobe Workfront定價與封裝](https://business.adobe.com/products/workfront/pricing.html)。

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->
