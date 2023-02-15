---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽
description: 資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2973'
ht-degree: 0%

---

# 資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

對資源進行預算，以使其在項目上必須完成的工作是資源計畫員的主要功能。 您可以檢視資源的可用時間，並將其時間分配給指派資源的專案。

有關資源計畫員中預算資源的資訊，請參閱 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

本文介紹了在開始在資源計畫器中預算資源之前需要了解的一些重要概念。

## 預算資源概覽

使用資源計畫器編製資源預算時，請考慮以下事項：

* 您可以指定資源可用於完成項目工作的小時數、FTE或成本，從而為資源分配預算。 在預算資源的時間或成本時，資源的可用小時數、FTE或成本將按預算金額減少。 因此，在您要為其編製預算的項目後面的項目的可用小時數、FTE或成本金額會減少這些用戶和這些項目上的角色。

   >[!IMPORTANT]
   >
   >您可以將資源預算為15年。 如果為持續時間超過15年的項目預算資源，則預算資訊可能不準確。

* 您可以為資源在資源計畫器中顯示的任意時間範圍預算小時數、FTE或成本，而不受項目時間軸的影響。 例如，如果您想要指明資源可能在項目時間軸期間不可用（在該時間軸與計畫小時數關聯），但在其他時間可能可用，則可以通過為計畫小時數為零的時間範圍編製預算來執行此操作（如果計畫小時數可用）。 在執行此操作後，您可以手動更改項目的時間表，以匹配資源可用性。

   >[!NOTE]
   >
   >建議您先手動預算職務角色或用戶的小時數、FTE或成本。 只有在確定「計畫小時數」、「FTE」或「成本」的金額始終與「預算小時數」、「FTE」或「成本」相匹配時，您才能使用自動選項來為項目和資源預算時間。\
   >有關在資源計畫員中使用預算自動選項的資訊，請參閱文章中的「自動預算項目和職責」部分 [使用Adobe Workfront資源計畫器複查資源可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* 預算FTE或成本與預算小時相同，在預算小時中，Adobe Workfront會使用FTE和成本值，而不是您預算的資源的小時數。

   有關了解如何在資源計畫器中計算成本的詳細資訊，請參閱 [在資源計畫器中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* 在「資源計畫器」中為資源分配預算分配的方法如下：

   * 手動

      或

   * 自動，借由在 **依專案檢視** 和 **按角色查看** 檢視。
   如需詳細資訊，請參閱 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* 當用戶更改作業角色、從資源池中刪除、停用或刪除時，該角色的預算小時數不會更改，並且這些小時會被重新分配給該角色中的其餘用戶。 如果再沒有任何使用者與工作角色相關聯，該角色的「已預算小時數」將變為零。

如需專案和角色選項的詳細資訊，請參閱區段 [了解資源計畫員中的小時數、FTE和成本值](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) 這篇文章。

## 了解資源計畫員中的小時數、FTE和成本值 {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

在對資源進行預算以及在資源計畫器中更新預算小時數資訊之前，您必須熟悉以下概念

* **計畫小時數、FTE或成本**:需要根據任務和問題的定義完成的工作。
* **可用小時數、FTE或成本**:根據與用戶關聯的計畫，用戶或作業角色可用於工作的時間。

此資訊顯示在資源計畫器中，用於每個資源（用戶或角色）和每個項目。

如需專案中顯示項目和角色檢視項目相關資訊，請參閱文章 [資源計畫員導航概覽](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

有關了解如何在資源計畫器中計算成本的資訊，請參閱文章 [在資源計畫器中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>按成本編製預算與按小時數或FTE編製預算相同，但您必須了解Workfront如何計算資源計畫員的成本。
>
>有關如何在資源計畫器中計算成本的資訊，請參閱文章 [在資源計畫器中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

下表顯示了在應用項目或角色視圖時在資源計畫器中顯示的分配和可用性資訊。 您可以按小時、FTE或成本查看此資訊：

* [AVL（可用）欄](#the-avl-available-column)
* [「PLN（計畫）」列](#the-pln-planned-column)
* [BDG（預算）欄](#the-bdg-budgeted-column)
* [VAR（變數）欄](#the-var-variance-column)
* [NET列](#the-net-column)

### AVL（可用）欄 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td><strong>說明</strong> </td> 
  </tr> 
  <tr> 
   <td>專案 </td> 
   <td> <p>項目上所有用戶都可以根據其計畫在所選時間範圍內工作的小時數、FTE或成本總計。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>與此角色關聯的所有用戶均可根據其計畫和計畫工作的小時數、FTE或成本合計 <strong>FTE可用性百分比</strong> 針對該特定角色，針對所選時間範圍。 </p> <p>請考量下列事項： </p> 
    <ul> 
     <li>如果沒有用戶與作業角色相關聯，則作業角色的「可用小時數」值為零。 </li> 
     <li>如果用戶與主要作業角色相關聯，但 <strong>FTE可用性百分比</strong> 對於角色為0%，工作角色「可用小時數」值為零。</li> 
     <li>如果使用者與「其他角色」相關聯，且 <strong>FTE可用性百分比</strong> 對於角色為0%，「其他角色」不會列在「資源規劃器」中，用戶只會顯示在其「主要角色」下。</li> 
    </ul> <p>如需 <strong>FTE可用性百分比</strong> 如需工作角色，請參閱文章 <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</p> <p>有關如何在資源計畫員中計算任務職責可用性的詳細資訊，請參閱文章中的「計算資源計畫員中任務職責的可用小時數和FTE」部分 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">在資源計畫員中計算用戶和角色的小時數和FTE的概覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>根據用戶的計畫，在所選時間範圍內，用戶可以工作的小時數、FTE或成本。 此數字減去與以下項目相關聯的小時數：</p> 
    <ul> 
     <li>排程例外</li> 
     <li>用戶超時</li> 
     <li>為其他項目編列預算的時數。 </li> 
    </ul> <p>用戶的可用小時數、FTE或成本根據以下條件進行更改： </p> 
    <ul> 
     <li>如何根據系統級別的「資源管理首選項」計算其計畫和FTE。<br><p>有關計算用戶和作業角色可用性的詳細資訊，請參閱文章 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">在資源計畫員中計算用戶和角色的小時數和FTE的概覽</a>.</p>
     有關在Workfront中配置資源管理首選項的詳細資訊，請參見 <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置資源管理首選項</a></li> 
    </ul> 
    <ul> 
     <li>the <strong>項目計畫優先順序</strong>，則會在使用者已編入工作預算時執行。<br>有關項目計畫優先順序如何影響用戶可用小時數的詳細資訊，請參閱 <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">資源計畫員導航概覽 </a>. </li> 
    </ul> <p>如果計畫用戶停用，則停用日期後的可用小時數、FTE或成本為零。 <br>如需停用使用者的詳細資訊，請參閱文章 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### 「PLN（計畫）」列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td><strong>說明</strong> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td> <p>項目下列出的所有任務角色或用戶的計畫小時數、FTE或成本合計，包括 <strong>無角色</strong> 或 <strong>無用戶</strong> 節，顯示所選時間範圍和項目的「項目詳細資訊」頁簽中顯示的內容。 </p> <p><b>附註</b>

人工調整每日用戶分配可能會更改資源計畫員中的每週、每月或每季計畫小時數值。 您可以使用工作負載平衡器手動調整任務和問題的每日用戶分配。 如需詳細資訊，請參閱 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器中管理用戶分配</a>.</p> </td>
</tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>在所選時間範圍內，從分配給角色的所有任務中的計畫時數總計。 </p> <p>此 <strong>無角色</strong> 小節將顯示與未分配、分配給團隊(其小時數列於 <strong>無用戶</strong> 區段)，或指派給未與工作角色相關聯的使用者。 </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>在所選時間範圍內，從分配給某個特定角色的用戶的所有任務的計畫小時數。 </p> <p>此 <strong>無用戶</strong> 小節將顯示與未分配或分配給團隊的任務關聯的計畫小時數。 </p> </td> 
  </tr> 
 </tbody> 
</table>

檢視「計畫小時數」時，請考量下列事項：

* 雖然您在「項目」和「職責」視圖中看不到「資源計畫員」中有關任務分配的資訊，但「計畫小時數」金額來自項目中任務的「計畫小時數」。
* 計畫小時數在任務持續時間內的每天分配給它們的每個資源。 任務持續時間基於任務計劃開始和完成日期，並包括該時段內的每個日曆日。\
   Workfront在將「計畫時間」分發給使用者或專案時，會考量使用者或專案的排程。 在這種情況下，計畫小時數在任務持續時間內平均分配給每天，但不包括週末、休假天數和計畫例外。\
   例如，如果按周顯示資源計畫員，並且您的任務跨越項目的多個周，則每週計畫小時數取決於該周內多少天屬於任務持續時間的一部分。 在按月或季度顯示資源計畫器以及任務跨越多個月或季度時，這同樣適用。\
   此分配中不包括週末天數、排程例外和休假天數。
* 計算每個資源的「計畫小時數」時包括以下任務類別：

   * 分配給項目上資源池、作業角色或團隊中的用戶的任務\
      如果將任務指派給團隊，則其分配將顯示在 **無角色** 和 **無用戶** 區段。 您可以看到與團隊相關聯的計畫小時數，但無法預算小時數，因為沒有任何角色或用戶與任務相關聯。

   * 未分配的任務

* 資源計畫員中的計畫小時數不包含與以下項目關聯的計畫小時數：

   * 上層任務
   * 分配給沒有資源池的用戶的任務
   * 問題，當 **包括來自問題的小時數** 設定已停用。

* 如果任務持續時間為零，計畫小時數不會顯示在資源計畫器中。
* 未顯示與停用的使用者相關聯的計畫小時數。

### BDG（預算）欄 {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td><strong>說明</strong> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td> <p>人工輸入，用於估計選定時間範圍內項目預算的小時數、FTE或成本。 </p> <p>在「項目」視圖中，您為項目預算的小時數將分配給項目下列出的作業角色。 每個角色的「計畫小時數」決定如何將「預算小時數」分配給這些角色。 預算小時數分配給具有較高計畫小時數值的角色。 </p> <p>在「角色」視圖中，您為項目預算的小時數不會分配給項目上的角色或用戶。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>人工輸入，用於估計選定時間範圍內某個職責的預算小時數。 </p> <p>如果沒有任何用戶與職務角色相關聯，則無法估計職務角色的預算小時數。 </p> <p>在「角色」視圖中，您為角色預算的小時數將分配給該角色下列出的項目。 每個項目的「計畫小時數」量決定如何將「預算小時數」分配給項目。 預算小時數分配給計畫小時數值較高的項目。</p> <p>在「項目」視圖中，您為角色預算的小時數不會分配給與角色關聯的項目或用戶。 </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>人工輸入，用於估計所選時間範圍內用戶預算的小時數。 </p> <p> <p><b>注意</b>   您可以估計未分配給任務，但與項目上的資源池關聯的用戶的預算小時數，因為這些用戶也顯示在資源計畫器中。 但是，如果未將計畫小時數分配給任務，則其計畫小時數應為零。 </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

使用預算小時數時，請考量下列事項：

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* 只有在對項目具有「編輯」「資源管理」和「財務資料」的訪問權限和「管理財務」權限時，才能對資源進行預算。

   有關預算資源所需的訪問權限的資訊，請參閱文章 [獲得Adobe Workfront預算資源所需資源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* 預設情況下，資源計畫器中的預算小時數為所有資源和所有項目的預算小時數為零。
* 您可以手動估計用戶和角色的預算小時數，也可以使用項目或職務角色中的一個連結 **更多** 功能表，以根據「計畫小時數」來更新。\
   如需專案和角色選項的詳細資訊，請參閱 [資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽](#Budget) 這篇文章。

* 可以預算小時數、FTE或成本的最短時間是一週。 您不能預算一天的小時數、FTE或成本。
* 在任務的持續時間內，為分配給任務的每個資源，預算小時數平均分配給每天。 任務持續時間基於任務計劃開始和完成日期，並包括該時段內的每個日曆日。\
   Workfront在將預算小時數分發給使用者或專案時，會考量使用者或專案的排程。 在這種情況下，預算小時數在任務持續時間（不包括週末）內平均分配給每天，但包括超時和計畫例外。\
   例如，如果按周顯示資源規劃器，並且您的任務跨越了多周，則每週預算小時數取決於該周內多少天是任務持續時間的一部分。 此分送會排除週末天數。 在按月或季度顯示資源計畫器以及任務跨越多個月或季度時，這同樣適用。

* 您可以選擇「預算小時數」作為新報表的報表對象，以報告「預算小時數」。\
   如需可在Workfront中報告哪些物件的詳細資訊，請參閱文章中的「報告物件」一節 [了解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   有關建立「預算小時」報表的資訊，請參閱文章 [報告：預算小時數](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* 先前為之後已停用的使用者編列的小時數不會顯示。

### VAR（變數）欄 {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td><strong>說明</strong> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td> <p>「小時」、「FTE」或「成本差異」顯示項目是否有足夠的預算小時數來完成項目的所有計畫小時數。 </p> <p>項目小時數、FTE或成本差異使用以下公式計算：</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>「小時」、「FTE」或「成本差異」顯示職責是否有足夠的預算小時數、FTE或成本來完成分配給該職責的「計畫小時數」。 </p> <p>職責小時、FTE或成本差異使用以下公式計算：</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>小時數、FTE或成本差異顯示是否有足夠的預算小時數供用戶完成分配給它們的計畫小時數。 </p> <p>用戶小時數、FTE或成本差異使用以下公式計算：</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>當「小時數」、「FTE」或「成本差異」以紅色顯示時，您估計的預算小時數比需要完成的實際工作的「計畫小時數」要少。 在這種情況下，預算小時數可能不足以完成工作。

### NET列  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>顯示者</strong> </td> 
   <td><strong>說明</strong> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td> 
    <div> 
     <p>項目淨小時數、FTE或成本可能顯示以下其中一項： </p> 
     <ul> 
      <li> <p>項目的可用時間或成本與預算時間或成本之間的差：</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>啟用NET計算設定中的「使用計畫(PLN)」值時，項目的「可用時間」或「成本」與「計畫時間」或「成本」之間的差值： </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>筆尖</b></p>        
  <p>只有當您自訂「顯示選取的項目」區段中的檢視時，才會套用此選項。</p>
  <p>如需詳細資訊，請參閱 <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >使用Adobe Workfront資源計畫器複查資源可用性和分配</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> 
    <div> 
     <p>「淨小時數」、「FTE」或「成本」角色可能顯示以下任一項： </p> 
     <ul> 
      <li> <p>職責的可用時間或成本與預算時間或成本之間的差異：</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>啟用NET計算設定中的「使用計畫(PLN)」值時，職責的「可用時間」或「成本」與「計畫時間」或「成本」之間的差值：</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>筆尖</b> <span>

只有當您自訂「顯示選取的項目」區段中的檢視時，才會套用此選項。</span> </p> <p><span>如需詳細資訊，請參閱 </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront資源計畫器複查資源可用性和分配</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>使用者</td> 
   <td> 
    <div> 
     <p>用戶淨小時數、FTE或成本可能顯示以下任一項： </p> 
     <ul> 
      <li> <p>用戶的可用時間或成本與預算時間或成本之間的差異：</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>啟用NET計算設定中的「使用計畫(PLN)」值時，用戶的可用時間或成本與「計畫時間」或「成本」之間的差：</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>筆尖</b> <span>

只有當您自訂「顯示選取的項目」區段中的檢視時，才會套用此選項。</span> </p> <p><span>如需詳細資訊，請參閱 </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront資源計畫器複查資源可用性和分配</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**當「淨小時數」、「FTE」或「成本」顯示為紅色時，沒有足夠的可用時間或預算來覆蓋預算的時間或預算** 或與工作相關的計畫時間或成本。 在這種情況下，資源會過度分配。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
