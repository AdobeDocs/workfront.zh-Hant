---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：顯示列中兩個欄位之間的計算結果'
description: 可以在列中使用文本模式來顯示兩個欄位之間的計算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 視圖：顯示列中兩個欄位之間的計算結果

可以在列中使用文本模式來顯示兩個欄位之間的計算。

例如，如果要瞭解兩個日期之間經過的周天數，可以使用文本模式語法和資料表達式來計算此差異。\
例如，您可以計算任務的計畫完成日期和實際完成日期之間的周天差，並在列中顯示結果。

您可以在此計算中使用任何其它兩個日期（實際起始、實際完成、預計起始和預計完成等）。\
有關計算資料表達式的詳細資訊，請參見 [計算的資料表達式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 顯示列中兩個欄位之間的計算結果

要將此列添加到任務視圖：

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖**。

1. 按一下 **添加列**，則 **切換到文本模式**。

1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：
   <pre>displayname=周天差異<br>textmode=true<br>valueexpression=Weekdaydiff({planedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. （可選）要聚合在分組中視圖中顯示的值，請按照中所述的步驟操作 [分組：顯示分組中聚合多個計算值的結果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md)。
1. 按一下 **保存**，則 **保存視圖**。
