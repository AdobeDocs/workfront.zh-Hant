---
content-type: reference
product-area: projects
navigation-topic: financials
title: 計算預算成本
description: 使用利用率報告計算預算成本跟蹤項目進度」
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# 計算預算成本

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

項目的預算成本是指在計畫項目時與項目關聯的總成本。

## 項目預算成本概覽

您不能手動更改項目的預算成本。 Adobe Workfront使用下列公式計算預算成本：

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* 此 **資源計畫員預算人工成本** 在上述計算中，是與項目中的任務角色關聯的成本。

   您可以在「業務案例」或「資源計畫員」的「資源預算」區域中跟蹤項目的預算人工成本。

   >[!TIP]
   >
   >  在「業務案例」中，項目的預算人工成本在報表和清單中顯示為資源計畫員預算人工成本。

   有關預算人工成本的資訊，請參閱文章 [了解項目的預算人工成本和預算工時](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* 此 **預算費用** 在上述計算中，與項目支出關聯的計畫成本，這些費用在「業務案例」的「支出」區域或項目的「支出」標籤中計算。\
   有關項目費用的詳細資訊，請參閱文章 [管理項目費用](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* 此 **固定成本** 在上述計算中，與項目成本關聯的固定金額，如項目「詳細資訊」部分的「財務」區域中所定義。\
   有關項目的「財務」子頁簽的詳細資訊，請參閱文章 [管理項目財務區域中的資訊](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront會使用專案的貨幣計算所有成本資訊。 如果在「資源計畫員」中為資源指定「預算小時數」，則禁用更改項目幣種的選項。
>
>如需變更專案貨幣的詳細資訊，請參閱文章 [更改項目幣種](../../../manage-work/projects/project-finances/change-project-currency.md).

## 查找項目的預算成本

「業務案例」或「資源計畫員」的「資源預算」區域中反映的「預算成本」將以下名稱顯示在Workfront的以下區域：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>預算成本顯示名稱</strong></td> 
     <td><strong>Workfront地區</strong></td> 
    </tr> 
    <tr> 
     <td>預算成本</td> 
     <td> <p>業務案例摘要</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>成本</td> 
     <td> <p>Portfolio優化程式</p> <p>提示：所有項目預算成本值的合計為組合的預算成本。</p> </td> 
    </tr> 
    <tr> 
     <td>專案預算成本</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>專案報表</p> <p>項目（財務資料）報告</p> <p>任務報告</p> <p>問題報告</p> <p>預算小時報表</p> <p>如需建立報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
