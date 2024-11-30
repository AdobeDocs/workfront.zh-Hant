---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 執行報告
description: 您可以執行任何您有權檢視的報表。
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---


# 執行報告

您可以執行任何您有權檢視的報表。

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
      <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視對報告、儀表板、行事曆的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視報表許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 執行報告

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 報表]**。

1. 從下列選項中選取：

   * **我的報告：**&#x200B;您已建立的報告。
   * **與我共用：**&#x200B;其他使用者與您共用的報告。
   * **所有報告：**&#x200B;系統中您可存取的所有報告。

1. 按一下您要執行的報表名稱。\
   或\
   如果報表是使用提示建立的，請從下拉式功能表中選取適當的資訊，然後按一下&#x200B;**[執行報表]**。\
   如需提示的詳細資訊，請參閱[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。\
   報表內容會在報表的右上角顯示時間戳記，包括從執行報表的使用者內容執行報表時的日期、時間和時區。

1. （選擇性）如果報表已在瀏覽器中顯示一段時間，請按一下&#x200B;**重新載入圖示** ![重新載入圖示](assets/unshimmed-report-refresh-icon.png)以重新整理報表中的結果。

1. （視條件而定）如果報告使用篩選器或提示，請按一下&#x200B;**顯示篩選器和提示**，以顯示您檢視之報告上使用的篩選器和提示清單。 如果報告僅包含篩選器或僅包含提示，則會改為顯示&#x200B;**顯示篩選器**&#x200B;或&#x200B;**顯示提示**。

   ![顯示篩選和提示](assets/unshimmed-show-filters-and-prompts.png)

   資訊會顯示在頁面左側的報表名稱下方。 對於提示，這是在執行報告時所做的提示選擇的資訊，如步驟3中所述。

1. 如果您使用自訂提示，則不會顯示。 只顯示系統提示。 自訂篩選器一律顯示。

## 檢視快取報告

如果報表在瀏覽器中顯示了一段時間，則可能會快取該報表。 執行下列任一動作時，可以強制重新載入快取報表：

* 編輯報告設定並儲存報告。
* 變更「檢視」、「群組」或「篩選」。
* 按一下&#x200B;**重新載入圖示** ![重新載入圖示](assets/unshimmed-report-refresh-icon.png)
此選項可在頁面右上角的「訊息」方塊中使用，以指出儲存報表的時間，或此選項可在放置報表的儀表板的右上角中使用。 如需有關重新載入儀表板的詳細資訊，請參閱[開始使用儀表板](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)一文中的「顯示儀表板」一節。

* 導覽至「摘要」、「矩陣」或「圖表」標籤，存取第一頁以外的任何報表頁面。
