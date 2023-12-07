---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：顯示欄中兩個欄位之間的計算結果」
description: 您可以在欄中使用文字模式，以顯示兩個欄位之間的計算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 檢視：顯示欄中兩個欄位之間的計算結果

您可以在欄中使用文字模式，以顯示兩個欄位之間的計算。

例如，如果您想找出兩個日期之間經過的周天數，您可以使用文字模式語法和資料運算式來計算此差異。\
例如，您可以計算任務的「計畫完成日期」與「實際完成日期」之間的周間日差，並在欄中顯示結果。

您可以在此計算中使用任何其他兩個日期（實際開始日期、實際完工日期、預計開始日期、預計完工日期等）。\
如需有關計算資料運算式的詳細資訊，請參閱 [計算資料運算式的概觀](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 顯示欄中兩個欄位之間的計算結果

若要將此欄新增至工作檢視：

1. 前往工作清單。
1. 從 **檢視** 下拉式功能表，按一下 **新檢視**.

1. 按一下 **新增欄**，然後 **切換到文字模式**.

1. 暫留在文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：
   <pre>displayname=周間差異<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate}，{actualCompletionDate})<br>valueformat=HTML</pre>

1. （選擇性）若要彙總群組檢視中顯示的值，請遵循中所述的步驟 [分組：顯示分組中多個計算值的彙總結果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. 按一下 **儲存**，然後 **儲存檢視**.
