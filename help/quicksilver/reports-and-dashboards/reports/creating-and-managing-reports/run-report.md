---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 執行報表
description: 您可以執行任何您有權存取「檢視」的報表。
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---


# 執行報表

您可以執行任何您有權存取「檢視」的報表。

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視對報表、控制面板、日曆的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視報表的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 執行報表

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.

1. 從下列選項中選取：

   * **我的報告：** 您已建立的報表。
   * **與我共用：** 其他使用者已與您共用的報表。
   * **所有報表：** 系統中您有權存取的所有報表。

1. 按一下您要執行之報表的名稱。\
   或\
   如果報告是使用提示建立的，請從下拉菜單中選擇相應的資訊，然後按一下 **執行報表**.\
   有關提示的詳細資訊，請參閱 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   報表內容會在報表的右上角顯示時間戳記，包含從執行報表的使用者上下文執行報表時的日期、時間和時區。

1. （選用）按一下 **重新載入圖示** ![](assets/qs-report-refresh-icon.png) 若要在瀏覽器中顯示報表一段時間後，重新整理報表中的結果。

1. （條件性）如果報表使用篩選器或提示，請按一下 **顯示篩選器和提示** 顯示您正在檢視之報表上使用的篩選器和提示清單。 如果報表僅包含篩選器或僅包含提示， **顯示篩選器** 或 **顯示提示** 的URL。

   ![顯示篩選器和提示](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   資訊會顯示在頁面左側的報表名稱下方。 對於提示，這是有關運行報告時所做的提示選擇的資訊，如步驟4所述。

1. 如果使用「自定義提示」，則不顯示這些提示。 只顯示系統提示。 自訂篩選器一律會顯示。

## 檢視快取報表

如果報表已在您的瀏覽器中顯示一段時間，則可能會快取它。 執行下列任一動作時，可以強制重新載入快取報表：

* 編輯報表設定並儲存報表。
* 變更檢視、群組或篩選。
* 按一下 **重新載入圖示**
此選項位於訊息方塊內頁面的右上角，指出儲存報表的時間，或位於報表所在控制面板的右上角。 有關重新載入控制面板的詳細資訊，請參閱文章中的「顯示控制面板」一節 [控制面板快速入門](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* 導覽至「摘要」、「矩陣」或「圖表」標籤，以存取報表中第一頁以外的任何頁面。
