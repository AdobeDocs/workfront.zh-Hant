---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 業務案例財務欄位概覽
description: 「業務案例」子標籤包含項目的財務欄位。 為了使某些財務欄位具有值，必須完成「業務案例」的相應區域。
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# 業務案例財務欄位概覽

「業務案例」子標籤包含項目的財務欄位。 為了使某些財務欄位具有值，必須完成「業務案例」的相應區域。  

「業務案例」中顯示以下項目財務欄位：

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
   <td> <p>根據計分卡顯示專案的對齊方式。 高百分比值表示項目與本組織的宗旨和目標完全一致。 <br>如需使用計分卡的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">建立計分卡</a>.</p> <p>此欄位顯示在「業務案例摘要」區域中。 </p> </td> 
  </tr> 
  <tr> 
   <td>預算成本</td> 
   <td> <p>在項目啟動時與項目關聯的估計總成本。</p> <p>項目的預算成本按以下公式計算：<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront使用資源計畫員的預算小時數來計算預算人工成本。<br>有關計算預算成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">計算預算成本</a>. </p> <p>此欄位顯示在「業務案例摘要」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>預算費用成本</td> 
   <td> <p>項目所有費用的預算費用。 </p> <p>此計算公式如下：</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>有關計算費用的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理項目費用 </a>.</p> <p>此欄位顯示在「費用」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>預算勞力成本</td> 
   <td> <p>與分配給完成項目工作的資源相關聯的成本。</p> <p>項目的預算人工成本按以下公式計算：<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>Workfront使用資源計畫員的預算小時數來計算預算人工成本。<br>有關計算預算人工成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解項目的預算人工成本和預算工時</a>.</p> <p>此欄位顯示在「業務案例」的「資源預算」區域中。 </p> </td> 
  </tr> 
  <tr> 
   <td>費用計畫成本</td> 
   <td> <p>這與預算費用成本相同。 </p> <p>注意：費用計畫成本與項目的計畫成本不同。 「費用計畫成本」是按項目費用的「計畫金額」計算，而「計畫成本」是按項目的「計畫小時數」計算。 </p> <p>此欄位顯示在「費用」區域中，用於每項費用。</p> </td> 
  </tr> 
  <tr> 
   <td>淨值</td> 
   <td> <p>這是計算項目收益並去除成本後的項目總預期價值。</p> <p>項目的淨值按以下公式計算：<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>。 <br></p> <p>如需計算淨值的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">計算淨值</a>.<br></p> <p>此欄位顯示在「業務案例摘要」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>計畫收益</td> 
   <td>此項目完成時對貴組織的貨幣利益進行手動估計。 它可以是任何金額的貨幣，並且是您和您管理的每個項目專屬的貨幣。 計畫福利不能為負值。 此欄位顯示在「業務案例摘要」區域中，並可在「業務案例」的「項目資訊」區域中編輯。 </td> 
  </tr> 
  <tr> 
   <td>潛在風險成本</td> 
   <td> <p>這是項目上所有風險的潛在成本。 </p> <p>這會使用下列公式計算：</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>有關項目風險的詳細資訊，請參閱 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">建立和編輯項目風險</a>.</p> <p>此欄位顯示在「業務案例摘要」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>潛在風險</td> 
   <td> <p>在「業務案例摘要」中，這是所有風險（如果應發生）的成本金額，根據其發生概率。 例如，如果「風險」的潛在成本為$100，「發生的可能性」為10%，則「潛在風險」為$10。 「業務案例摘要」中的潛在風險按以下公式計算：</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> 所有風險。 </p> </td> 
  </tr> 
  <tr> 
   <td>風險降低成本</td> 
   <td> <p>針對您估計的風險的緩解計畫的成本可能發生在項目上。<br>有關項目風險的詳細資訊，請參閱 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">建立和編輯項目風險</a>.</p> <p>此欄位顯示在項目上指定的每個風險的「風險」區域中。</p> </td> 
  </tr> 
  <tr> 
   <td>一個風險的潛在成本</td> 
   <td> <p>在項目上確定的風險實際發生時的估計財務成本，不論其可能性如何。 </p> <p>這是一個手動更新的欄位，顯示在「業務案例」的「風險」區域中的每個風險。 </p> </td> 
  </tr> 
  <tr> 
   <td>風險總潛在成本</td> 
   <td> <p>這是項目實際發生時所界定的所有風險的估計財務費用總額。 </p> <p>此計算公式如下：</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>它顯示為「業務案例」「風險」區域標題旁的貨幣編號。</p> </td> 
  </tr> 
 </tbody> 
</table>
