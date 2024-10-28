---
content-type: reference
product-area: reporting;projects
keywords: 計算，彙總，進階，檢視
navigation-topic: custom-view-filter-and-grouping-samples
title: 「分組：顯示分組中多個計算值的彙總結果」
description: 您可以使用欄中的文字模式，在報表或清單檢視中的兩個欄位之間顯示計算。 每一行會顯示報表或清單中每個物件的計算。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 分組：顯示分組中多個計算值的彙總結果

<!--Audited: 10/2024-->

您可以使用欄中的文字模式，在報表或清單檢視中的兩個欄位之間顯示計算。 每一行會顯示報表或清單中每個物件的計算。

例如，您可以在任務報告中針對每個任務，在名為「工作平衡」的第三欄中顯示實際時數與計畫時數之間的差異。 如需有關計算資料運算式的詳細資訊，請參閱[計算資料運算式概觀](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

您可以將計算新增至包含計算值的欄的`aggregator`行，以在群組的相同欄中顯示多個計算檢視專案的彙總值。 例如，您可以彙總（顯示總計）報告分組或「工作平衡」欄清單中所有任務的「工作平衡」時數金額。 本文會介紹如何執行此動作。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 顯示群組內多個計算值的彙總結果

1. 前往工作報告，按一下&#x200B;**報告動作** > **編輯**。
1. 在&#x200B;**群組**&#x200B;索引標籤中，按一下&#x200B;**新增群組**，並開始在&#x200B;**群組依據**&#x200B;欄位中輸入&#x200B;**專案名稱**，然後在其顯示在清單中時選取&#x200B;**專案>名稱**。

1. 在&#x200B;**欄（檢視）**&#x200B;索引標籤中，按一下&#x200B;**新增欄**，然後在&#x200B;**顯示在此欄**&#x200B;欄位中開始輸入&#x200B;**計畫時數**，然後在它顯示在清單中時選取它。

   >[!TIP]
   >
   >在文字模式中編輯資訊之前，請一律開始使用「標準」介面新增儘可能多的資訊。 新增最接近或包含最多您嘗試計算之資訊量的欄位。

1. 在&#x200B;**依**&#x200B;摘要此欄位中，選取&#x200B;**總和**。
1. 在您新增的欄中按一下&#x200B;**切換到文字模式**，然後按一下&#x200B;**編輯文字模式**。
1. 以下列文字模式範例取代方塊中的文字：

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >若要取得群組中的彙總值，以顯示計畫時數與實際時數欄位之間的彙總差異，請在`aggregator.valuefield`行中輸入相同的方程式。 用於計畫時數欄的`aggregator.displayformat`會將分鐘轉換為時數。 由於計畫時數欄位已用作預留位置，因此不需要調整此行。
   >
   >
   >`aggregator.displayformat`行的`minutesAsHoursString`定義表示不需要像在`valueexpression`上做的那樣，將每個欄位除以60以取得結果。 在此`aggregator.valuefield=workRequired`中變成： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`。
1. 按一下&#x200B;**完成**。
1. 按一下&#x200B;**儲存+關閉**。
