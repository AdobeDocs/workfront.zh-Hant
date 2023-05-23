---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看和分組：顯示項目實際工期按分組中的平均值聚合'
description: 您可以在項目報告中添加以下列，以將實際持續時間聚合顯示為分組中的平均值。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 查看和分組：顯示按分組中的平均值聚合的項目實際持續時間

您可以在項目報告中添加以下列，以將實際持續時間聚合顯示為分組中的平均值。

![project_with_aggregate_actual_duration_in_grouping_view_png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## 顯示按分組中的平均值聚合的項目實際持續時間

要將此列添加到項目視圖：

1. （建議）要獲得最佳結果並查看實際工期的合計平均值，必須將分組添加到項目清單或報表中。\
   有關建立分組的詳細資訊，請參閱文章 [Adobe Workfront分組概覽](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

1. 轉到現有項目視圖。
1. 展開「視圖」(View)下拉菜單，然後選擇 **自定義視圖**。
1. 按一下 **添加列**。
1. 按一下 **切換到文本模式**。
1. 滑鼠懸停在 **在此列中顯示** ，然後按一下 **按一下可編輯文本**。

1. 刪除「文本模式」框中的所有文本，並用以下代碼替換它：

   <pre>聚合器.displayformat=複合 <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=項目實際工期 <br>durationunitifield=durationUnit.value <br>linkedname=project <br>namekey=實際持續時間 <br>namekeyargkey=實際工期 <br>querysort=actualDurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M:D <br>viewalias=實際持續時間</pre>

1. 按一下 **保存視圖**。
