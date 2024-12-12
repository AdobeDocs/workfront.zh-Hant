---
content-type: reference
product-area: projects
navigation-topic: financials
title: 計算預算成本
description: 使用使用情況報告計算預算成本追蹤專案進度」
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
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

專案的預算成本是當您計畫專案時，與專案相關聯的總估計成本。

## 專案中的預算成本概要

您無法手動變更專案的預算成本。 Adobe Workfront使用下列公式計算預算成本：

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* 上述計算中的&#x200B;**資源規劃工具預算勞力成本**&#x200B;是與專案中工作角色相關的成本。

  您可以在業務案例或資源規劃工具的資源預算區域中追蹤專案的預算勞力成本。

  >[!TIP]
  >
  >  業務案例中專案的預算勞力成本在報表和清單中顯示為「資源規劃工具預算勞力成本」。

  如需有關預算勞力成本的資訊，請參閱文章[瞭解專案的預算勞力成本和預算時數](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)。

* 以上計算中的&#x200B;**預算費用成本**&#x200B;是與專案費用相關的計畫成本，因為這些費用是在業務案例的費用區域或專案的費用標籤中計算的。\
  如需有關專案費用的詳細資訊，請參閱文章[管理專案費用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

* 以上計算中的&#x200B;**固定成本**&#x200B;是與專案成本相關的固定金額，如專案詳細資訊區段的「財務」區域中所定義。\
  如需有關專案[財務]子標籤的詳細資訊，請參閱文章[專案財務區域](../../../manage-work/projects/project-finances/manage-project-finance-area.md)中的管理資訊。

>[!NOTE]
>
>Workfront會使用專案的貨幣來計算所有成本資訊。 如果您在資源規劃工具中指定資源的預算時數，則會停用變更專案幣別的選項。
>
>如需有關變更專案貨幣的詳細資訊，請參閱文章[變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 找出專案的預算成本

反映在業務案例或資源規劃工具的資源預算區域中的預算成本，顯示在Workfront的以下區域中，其名稱如下：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>預算成本顯示名稱</strong></td> 
     <td><strong>Workfront區域</strong></td> 
    </tr> 
    <tr> 
     <td>預算成本</td> 
     <td> <p>業務案例摘要</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>成本</td> 
     <td> <p>Portfolio最佳化工具</p> <p>提示：所有專案預算成本值的總計是投資組合的預算成本。</p> </td> 
    </tr> 
    <tr> 
     <td>專案預算成本</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>專案報告</p> <p>專案（財務資料）報表</p> <p>任務報告</p> <p>問題報告</p> <p>已編列預算時數報告</p> <p>如需有關建立報告的詳細資訊，請參閱文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報告</a>。</p> </td> 
    </tr> 
   </tbody> 
  </table>
