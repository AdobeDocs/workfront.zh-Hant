---
product-area: reporting
navigation-topic: reporting-elements
title: 使用日期型萬用字元來一般化報表
description: 您可以在建立特定報表元素時，使用萬用字元而非特定資訊來泛化報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 1%

---

# 使用日期型萬用字元來一般化報表

<!-- Audited: 11/2024 -->

您可以在建立特定報表元素時，使用萬用字元而非特定資訊來泛化報表。

例如，如果您想要建立顯示具有特定計劃開始日期之任務的報表，則可以使用篩選器中的行事曆日期選擇器來選取特定日期。 但是，如果您想要建立一份報告，顯示自存取報告日期起特定時間範圍內具有計劃開始日期的任務，則可以使用萬用字元來指示當有人檢視報告時，它顯示與檢視報告之時相關的時間範圍資訊。

例如在過去的一週、在過去的一年、接下來的兩週等。 這樣的話，報表只需建立一次，但由於您在篩選器中使用萬用字元，因此每當有人讀取報表時，就會產生不同的結果，因為這會隨著他們執行報表的日期而改變。

建置下列報表元素時，您可以使用日期型萬用字元：

* 篩選器
* 自訂提示
* 為欄新增規則時的檢視

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>計劃</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的報告元素</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權，以編輯報表中的報表元素</p> <p>管理檢視或篩選的許可權以編輯它們</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先建立報表，才能在其中新增萬用字元變數。

如需建立報告的詳細資訊，請參閱[建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 操作步驟

若要在報表中插入以日期為基礎的萬用字元：

1. 移至您要插入日期型萬用字元的報表。
1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**編輯**。
1. 按一下&#x200B;**篩選器**&#x200B;索引標籤。
1. 按一下&#x200B;**新增篩選規則**。
1. 開始輸入您要作為篩選依據的欄位名稱。\
   您必須輸入參考日期的欄位。
1. 在篩選變數的下拉式選單中選取&#x200B;**等於**。

   >[!TIP]
   >
   >在Adobe Workfront中使用萬用字元時，您必須一律選取&#x200B;**等於**&#x200B;篩選器變數。

1. 按一下&#x200B;**設定相對日期**&#x200B;切換按鈕，然後在顯示的文字方塊中輸入： `$$TODAY` （如果您想要顯示報表執行當天發生的資訊）。

   或

   如果要顯示與報告執行日期和時間同時發生的某些事情的相關資訊，請輸入`$$NOW`。

   此日期一律不同，因為它會隨著使用者實際檢視報表的日期而變更。 所以報告中的資訊每天都不同。

1. （選擇性）如果要顯示報表執行日期之後某個時間範圍內發生的資訊，請輸入`$$TODAY+1w`以顯示下一週的資訊，或輸入`$$TODAY+2m`以顯示未來兩個月內的資訊。 您也可以指出季度、小時、天或年的時間範圍。
1. （選擇性）如果您想要顯示在執行報告日期之前的時間範圍內所發生事件的相關資訊，請輸入`$$TODAY-1w`以顯示前一週的資訊，或輸入`$$TODAY-2m`以顯示前兩個月的資訊。 您也可以指出季度、小時、天或年的時間範圍。

   如需您可以在日期型萬用字元中使用的屬性、限定詞和運運算元的完整清單，請參閱文章[萬用字元篩選變數概觀](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

1. 按一下「**儲存並關閉**」。

## 其他資訊

另請參閱：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [萬用字元篩選器變數總覽](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
