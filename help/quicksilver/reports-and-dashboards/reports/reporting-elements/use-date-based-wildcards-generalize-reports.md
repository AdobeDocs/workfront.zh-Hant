---
product-area: reporting
navigation-topic: reporting-elements
title: 使用日期型萬用字元來歸納報表
description: 建置特定報表元素時，您可以使用萬用字元（而非特定資訊）來歸納報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 使用日期型萬用字元來歸納報表

建置特定報表元素時，您可以使用萬用字元（而非特定資訊）來歸納報表。

例如，如果要建立一個報告，顯示具有特定計畫起始日期的任務，則可以使用篩選器中的日曆日期選擇器來選擇特定日期。 不過，如果您想要建立報表，以顯示自存取報表之日起特定時間範圍內具有計劃開始日期之工作，您可以使用萬用字元，指出當有人檢視報表時，其會顯示與其檢視報表時間相關的時間範圍資訊。

例如，過去一週、過去一年、未來兩週等。 這樣，您只需建置報表一次，但由於您在篩選器中使用萬用字元，因此每當有人讀取報表時，報表會產生不同的結果，因為報表會隨著使用者執行報表的當天而調整。

建置下列報表元素時，您可以使用日期型萬用字元：

* 篩選器
* 自訂提示
* 新增欄規則時的檢視

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的報表元素</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理報表權限以編輯報表中的報表元素</p> <p>管理檢視或篩選器的權限，以便編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立報表，才能新增萬用字元變數。

如需建立報表的詳細資訊，請參閱 [建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 操作步驟

若要在報表中插入日期型萬用字元：

1. 移至要插入日期型萬用字元的報表。
1. 按一下 **報表動作**，然後 **編輯**.

1. 按一下 **篩選器** 標籤。
1. 按一下 **新增篩選規則**.
1. 開始鍵入要篩選的欄位名稱。\
   您必須輸入參考日期的欄位。
1. 選擇 **等於** 的下拉式選單中。

   >[!TIP]
   >
   >您必須一律選取 **等於** 在Adobe Workfront中使用萬用字元時篩選變數。

1. 在 **開始鍵入名稱……** 框，鍵入： `$$TODAY` 如果您想要顯示報表執行當天發生之事項的相關資訊。

   或

   類型 `$$NOW` 如果您想要顯示與報表執行的相同日期和時間所發生之事件相關的資訊。

   此日期一律不同，因為它會隨著使用者實際檢視報表的日期而變更。 因此，報表中的資訊會因日而異。

1. （選用）如果您想要顯示報表執行日期後的時間範圍內發生的資訊，請輸入 `$$TODAY+1w` 顯示下週的資訊，或 `$$TODAY+2m` 以顯示未來兩個月的資訊。 您也可以指出季度、小時、天或年的時間範圍。
1. （選用）如果您想要顯示報表執行日期前某時間範圍內發生之項目的相關資訊，請輸入 `$$TODAY-1w` 顯示前一週的資訊，或 `$$TODAY-2m` 顯示前兩個月的資訊。 您也可以指出季度、小時、天或年的時間範圍。

   有關可以在基於日期的通配符中使用的屬性、限定符和運算子的完整清單，請參閱文章 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. 按一下 **儲存+關閉**.

## 其他資訊

另請參閱：

* [基本報表建立程式](https://one.workfront.com/s/basic-report-creation-program)
* [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
