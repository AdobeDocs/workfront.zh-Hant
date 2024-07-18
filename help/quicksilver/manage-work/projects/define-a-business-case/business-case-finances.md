---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 業務案例財務欄位概要
description: 「業務案例」子頁標包含專案的財務欄位。 為了讓某些財務欄位有值，必須完成業務案例的對應區域。
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 2%

---

# 業務案例財務欄位概要

「業務案例」子頁標包含專案的財務欄位。 為了讓某些財務欄位有值，必須完成業務案例的對應區域。  

業務案例中會顯示下列專案財務欄位：

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">欄位名稱</th> 
   <th scope="col">說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>已對齊 </td> 
   <td> <p>根據計分卡顯示專案的對齊方式。 高百分比值表示專案與組織的目的和目標高度一致。 <br>如需使用計分卡的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">建立計分卡</a>。</p> <p>此欄位會顯示在「業務案例摘要」區域中。 </p> </td> 
  </tr> 
  <tr> 
   <td>預算成本</td> 
   <td> <p>專案啟動時，與專案相關聯的預估總成本。</p> <p>專案的預算成本是透過下列公式計算：<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront使用資源規劃工具的預算時數來計算預算勞力成本。<br>如需有關計算預算成本的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">計算預算成本</a>。 </p> <p>此欄位會顯示在「業務案例摘要」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>預算費用成本</td> 
   <td> <p>專案上所有費用的預算成本。 </p> <p>計算公式如下：</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>如需有關計算費用的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理專案費用</a>。</p> <p>此欄位會顯示在「費用」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>預算勞力成本</td> 
   <td> <p>與指定完成專案工作的資源相關聯的成本。</p> <p>專案的預算勞力成本會透過下列公式計算：<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront使用資源規劃工具的預算時數來計算預算勞力成本。<br>如需有關計算預算勞力成本的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">瞭解專案的預算勞力成本和預算時數</a>。</p> <p>此欄位會顯示在業務案例的資源預算區域中。 </p> </td> 
  </tr> 
  <tr> 
   <td>費用計畫成本</td> 
   <td> <p>這與預算費用成本相同。 </p> <p>備註：費用計畫成本與專案的計畫成本不同。 費用計畫成本是以專案上的費用計畫金額計算，而計畫成本是以專案上的計畫時數計算。 </p> <p>此欄位會顯示在各項費用的「費用」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>淨值</td> 
   <td> <p>這是計算專案的收益並移除成本後，專案的預期總值。</p> <p>專案的「淨值」透過下列公式計算：<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>。 <br></p> <p>如需有關計算淨值的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">計算淨值</a>。<br></p> <p>此欄位會顯示在「業務案例摘要」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>規劃收益</td> 
   <td>此專案完成時，貴組織貨幣收益的手動預估。 可以是任何數量的貨幣，但您和您管理的每個專案都會有專屬的值。 計畫收益不能有負值。 此欄位會顯示在業務案例摘要區域中，並可在業務案例的專案資訊區域中編輯。 </td> 
  </tr> 
  <tr> 
   <td>潛在風險成本</td> 
   <td> <p>這是專案所有風險的潛在成本。 </p> <p>使用下列公式計算：</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>如需有關專案風險的詳細資訊，請參閱<a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">建立與編輯專案風險</a>。</p> <p>此欄位會顯示在「業務案例摘要」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>潛在風險</td> 
   <td> <p>在「業務案例摘要」中，這是所有風險（如果應該發生）的成本金額（根據其機率）。 例如，如果風險的潛在成本為$100，發生機率為10%，則潛在風險為$10。 「業務案例摘要」中的「潛在風險」是以下公式計算：</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> 針對所有風險。 </p> </td> 
  </tr> 
  <tr> 
   <td>風險降低成本</td> 
   <td> <p>針對您正在預估的風險之緩解計畫的成本，可能會發生在專案上。<br>如需有關專案風險的詳細資訊，請參閱<a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">建立並編輯專案風險</a>。</p> <p>此欄位會顯示在專案上所指定之各個風險的「風險」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>單一風險的潛在成本</td> 
   <td> <p>專案上定義的風險實際發生時的預估財務成本，無論其機率為何。 </p> <p>這是手動更新的欄位，會顯示在業務案例的風險區域中的每個風險。 </p> </td> 
  </tr> 
  <tr> 
   <td>風險總潛在成本</td> 
   <td> <p>這是專案上定義之所有風險實際發生時的預估財務成本總計。 </p> <p>計算公式如下：</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>它會在業務案例的風險區域標題旁邊顯示為貨幣編號。</p> </td> 
  </tr> 
 </tbody> 
</table>
