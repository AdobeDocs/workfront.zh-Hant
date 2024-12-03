---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 資源規劃工具之專案與角色檢視表中的時數、約當全職人數及成本資訊概要
description: 資源規劃工具之專案與角色檢視中的時數、約當全職人數及成本資訊概要
author: Lisa
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: c9e77e11fafbf224639289977783e95ccb45a9e2
workflow-type: tm+mt
source-wordcount: '3086'
ht-degree: 0%

---

# 資源規劃工具之專案與角色檢視中的時數、約當全職人數及成本資訊概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

資源規劃工具的主要功能是為資源編列預算，以供其在專案上完成的工作。 您可以檢視資源的可用時間，並將其時間分配給指派給它們的專案。

如需資源規劃工具中預算資源的相關資訊，請參閱資源規劃工具中使用專案與角色檢視的[預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

本文說明在資源規劃工具中開始為資源編列預算之前需要瞭解的一些關鍵概念。

## 預算資源概觀

使用資源規劃工具編列資源預算時，請考量下列事項：

* 您可以指定資源可用於完成專案工作的「時數」、「約當全職人數」或「成本」金額，以預算資源配置。 當您為資源編列時間或成本預算時，資源的可用時數、約當全職人數或成本會減少預算金額。 因此，您正在編列預算之專案之後之專案的可用時數、約當全職人數或成本金額，會針對這些專案中的使用者與角色而減少。

  >[!IMPORTANT]
  >
  >您可以為資源編列為期15年的預算。 如果您為持續期間超過15年的專案編列資源預算，預算資訊可能不準確。

* 您可以在「資源規劃工具」中顯示的任何時間範圍內，為資源預算「小時」、「約當全職人數」或「成本」，不受專案時間表的影響。 例如，如果您想要指出您的資源在專案的時間表期間可能無法使用（這些資源與計畫時數相關聯），但它們可能在另一個時間可供使用，您可以透過為計畫時數為零的時間範圍編列預算來執行此操作，前提是這些資源可供使用。 您可在執行此操作後，手動變更專案的時間表以符合您的資源可用性。

  >[!NOTE]
  >
  >建議您先手動為工作角色或使用者編列時數、約當全職人數或成本的預算。 只有在您確定計畫時數、約當全職人數或成本之金額一律符合您的預算時數、約當全職人數或成本時，您才可以使用自動選項來預算專案與資源的時間。\
  >如需有關在資源規劃工具中使用自動預算選項的相關資訊，請參閱文章[使用Adobe Workfront資源規劃工具](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md)檢閱資源可用性與配置中的「自動預算專案與角色」一節。

* 編列預算FTE或成本與編列預算時數相同，其中Adobe Workfront會使用FTE和成本值，而非您編列預算之資源的時數。

  如需瞭解如何在資源規劃工具中計算成本的詳細資訊，請參閱[在資源規劃工具中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

* 資源規劃工具中資源的預算配置可透過下列方式完成：

   * 手動

     或

   * 使用&#x200B;**依專案檢視**&#x200B;和&#x200B;**依角色檢視**&#x200B;檢視中的專案和角色選項，自動執行。

  如需詳細資訊，請參閱資源規劃工具中使用專案和角色檢視的[預算資源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

* 當使用者變更工作角色，被刪除、停用或從資源集區中移除時，為角色預算的時數未變更並且它們被重新分配給角色中的其餘使用者。 如果沒有任何使用者再與工作角色相關聯，該角色的預算時數將變為零。

如需有關專案和角色選項的詳細資訊，請參閱本文章[瞭解資源規劃工具](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner)中的時數、約當全職人數和成本值。

## 瞭解資源規劃工具中的時數、約當全職人數和成本值 {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

在將資源編列預算以及更新資源規劃工具中的預算時數資訊之前，您必須熟悉下列概念

* **計畫時數、FTE或成本**：需要完成的工作（如任務和問題上的定義）。
* **可用時數、FTE或成本**：根據與使用者關聯的排程，使用者或工作角色可用的工作時間。

此資訊會顯示在每個資源（使用者或角色）和每個專案的資源規劃工具中。

有關專案的專案和角色檢視中顯示的資訊，請參閱文章[資源規劃工具導覽概觀](../../resource-mgmt/resource-planning/resource-planner-navigation.md)。

如需瞭解如何在資源規劃工具中計算成本的資訊，請參閱文章[在資源規劃工具中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

>[!NOTE]
>
>按成本編列預算與按小時或約當全職人數編列預算相同，但您必須瞭解Workfront如何計算資源規劃工具的成本。
>
>如需有關如何在資源規劃工具中計算成本的資訊，請參閱文章[在資源規劃工具中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

下表顯示套用「專案」或「角色」檢視時，「資源規劃工具」中顯示的配置與可用性資訊。 您可以按小時、約當全職人數或成本檢視此資訊：

* [AVL （可用）資料行](#the-avl-available-column)
* [計畫（計畫）資料行](#the-pln-planned-column)
* [預算(BDG)資料行](#the-bdg-budgeted-column)
* [VAR （變數）資料行](#the-var-variance-column)
* [NET欄](#the-net-column)

### AVL （可用）欄 {#the-avl-available-column}

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
   <td> <p>專案上所有使用者在選取的時間範圍內根據其排程可工作的小時、約當全職人數或成本總計。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>在選取的時間範圍內，與此角色相關的所有使用者可根據其排程和他們在該特定角色的<strong>FTE可用性百分比</strong>工作的時數、FTE或成本總計。 </p> <p>請考量下列事項： </p> 
    <ul> 
     <li>如果沒有使用者與工作角色相關聯，則工作角色的「可用時數」值為零。 </li> 
     <li>如果使用者與主要工作角色相關聯，但角色的FTE可用性<strong>百分比</strong>為0%，則工作角色可用時數值為零。</li> 
     <li>如果使用者與其他角色相關聯，且角色的FTE可用性<strong>百分比</strong>為0%，則其他角色不會列在資源規劃工具中，使用者只會顯示在其主要角色下。</li> 
    </ul> <p>如需有關工作角色的<strong> FTE可用性百分比</strong>的詳細資訊，請參閱文章<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者設定檔</a>。</p> <p>如需有關如何在資源規劃工具中計算工作角色可用性的詳細資訊，請參閱文章<a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">計算資源規劃工具中使用者和角色的時數和FTE的概觀</a>中的「計算資源規劃工具中工作角色的可用時數和FTE」一節。</p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>在所選的時間範圍內，使用者根據其排程可工作的小時、FTE或成本。 此數字減去與以下專案相關的時數：</p> 
    <ul> 
     <li>排程例外</li> 
     <li>使用者的休假</li> 
     <li>為其他專案編列的時數。 </li> 
    </ul> <p>使用者的可用時數、FTE或成本會根據下列專案變更： </p> 
    <ul> 
     <li>如何根據系統層級的Resource Management Preferences計算其排程和FTE。<br><p>如需有關計算使用者和工作角色可用性的詳細資訊，請參閱文章<a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">計算資源規劃工具</a>中使用者和角色的時數和FTE的概觀。</p>
     如需有關在Workfront中設定資源管理偏好設定的詳細資訊，請參閱<a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理偏好設定</a></li> 
    </ul> 
    <ul> 
     <li><strong>專案計畫優先順序</strong> （如果使用者已編列工作預算）。<br>如需有關專案計畫優先順序如何影響使用者可用時數的詳細資訊，請參閱<a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">資源規劃工具導覽概觀</a>。 </li> 
    </ul> <p>如果使用者已排定停用，則停用日期後幾天的可用時數、FTE或成本為零。 <br>如需停用使用者的詳細資訊，請參閱文章<a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>



### 計畫（計畫）欄 {#the-pln-planned-column}

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
   <td> <p>專案下列出的所有工作角色或使用者的計畫時數、FTE或成本總計，包括所選時間範圍內的<strong>無角色</strong>或<strong>無使用者</strong>區段，並顯示在專案的[專案詳細資料]索引標籤中。 </p> <p><b>附註</b>

手動調整每日使用者配置可能會變更資源規劃工具中的每週、每月或每季計畫時數值。 您可以使用工作負載平衡器手動調整任務和問題的每日使用者分配。 如需詳細資訊，請參閱<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器</a>中管理使用者配置。</p> </td>
</tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>在選取的時間範圍內，從指派給角色的所有任務中計畫的時數總計。 </p> <p><strong>無角色</strong>區段將顯示與任務相關的計畫時數，這些任務可能是未指派、已指派給團隊（其時數列在<strong>無使用者</strong>區段中），或是已指派給未與工作角色相關聯的使用者。 </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>在選取的時間範圍內，從指派給特定角色中使用者的所有任務中計畫的時數。 </p> <p><strong>沒有使用者</strong>區段將顯示與未指派或指派給團隊的任務相關的計畫時數。 </p> </td> 
  </tr> 
 </tbody> 
</table>

檢視計畫時數時，請考慮下列事項：

* 雖然您在「專案」和「角色」檢視的「資源規劃工具」中看不到任務配置的相關資訊，但計畫時數的金額來自於專案中任務的計畫時數。
* 對於指派給任務的每個資源，計畫時數會平均分配給任務持續時間內的每一天。 「工期」是以任務的「計劃開始日期」和「完成日期」為基礎，並包含該時段內的每個行事曆日。\
  當向使用者或專案分配計畫時數時，Workfront會考慮使用者或專案的排程。 在此情況下，計畫時數會平均分配到工作期間內的每一天，週末除外、休假天數和排程例外。\
  例如，如果您按周顯示「資源規劃工具」，而您有專案上跨越多個周的任務，則每週的計畫時數取決於該周內的多少天屬於任務「工期」。 當按月或季度顯示資源規劃工具，以及任務跨越多個月或季度時，其作用類似。\
  週末天數、排程例外和休假天數會從此分佈中排除。
* 計算每個資源的計畫時數時，會包含下列任務類別：

   * 指派給資源集區、工作角色或專案團隊中使用者的任務\
     如果任務已指派給團隊，則其配置將顯示在&#x200B;**無角色**&#x200B;和&#x200B;**無使用者**&#x200B;區段下。 您可以檢視與團隊關聯的計畫時數，但無法預算時數，因為沒有任何角色或使用者與任務相關聯。

   * 未指派任務

* 資源規劃工具中的計畫時數不包含與下列專案關聯的計畫時數：

   * 父系任務
   * 指派給無資源集區之使用者的任務
   * 問題，當&#x200B;**包含來自問題的時數**&#x200B;設定停用時。

* 如果任務期間為零，則計畫時數不會顯示在資源規劃工具。
* 未顯示與已停用使用者相關的計畫時數。

### 預算(BDG)欄 {#the-bdg-budgeted-column}

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
   <td> <p>手動輸入以估計在選取的時間範圍內，您為專案編列預算的時數、約當全職人數或成本。 </p> <p>在「專案」檢視中，您為專案編列預算的時數會分配給專案下列出的職務角色。 每個角色的計畫時數金額決定如何將預算時數分配給角色。 預算時數會分配給具有較高計畫時數值的角色。 </p> <p>在「角色」檢視中，您為專案預算的時數不會分配給專案上的角色或使用者。 </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>手動輸入以估計您為某個角色在選定時間範圍內編列預算的時數。 </p> <p>如果沒有與工作角色相關聯的使用者，則您無法估計工作角色的預算時數。 </p> <p>在「角色」檢視中，您為角色編列預算的時數會分配至該角色下列出的專案。 每個專案的計畫時數金額會決定如何將預算時數分配給專案。 預算時數會分配給具有較高計畫時數值的專案。</p> <p>在「專案」檢視中，您為角色編列預算的時數不會分配至專案或與角色相關聯的使用者。 </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>手動輸入，用於估計在選取的時間範圍內，為使用者預算的時數。 </p> <p> <p><b>附註</b>   您可以為未指派給任務，但與專案上的資源集區相關聯的使用者估計預算時數，因為這些使用者也會出現在資源規劃工具中。 但是，如果它們未指派給任務，則其計畫時數應為零。 </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

使用預算時數時，請考慮下列事項：

* 只有當您對專案具有「資源管理」和「財務資料」的「編輯」存取權和「管理財務」許可權時，才能為資源編列預算。

  如需有關預算資源所需存取權的資訊，請參閱文章[在Adobe Workfront中預算資源所需的存取權](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)。

* 依預設，資源規劃工具中的預算時數，對於所有資源和所有專案都是零。
* 您可以手動估計使用者和角色的預算時數，或者您可以使用專案或工作角色&#x200B;**更多**&#x200B;選單中的其中一個連結，根據計畫時數來更新它們。\
  如需有關專案和角色選項的詳細資訊，請參閱本文中資源規劃工具](#Budget)的專案和角色檢視中的[時數概觀、約當全職人數和成本資訊一節。

* 您可以為預算小時、FTE或成本的最小期間是一週。 您無法編列一天的時數、約當全職人數或成本的預算。
* 預算時數會平均分配給任務期間內的每一天，適用於指派給他們的每個資源。 「工期」是以任務的「計劃開始日期」和「完成日期」為基礎，並包含該時段內的每個行事曆日。

  將預算時數分配給使用者或專案時，Workfront會考慮使用者或專案的排程。 在這種情況下，預算時數會平均分配到工作期間內的每一天，週末除外，但包括休假和排程例外狀況。

  例如，如果按周顯示「資源規劃工具」，而您的任務跨越數週，則每週的預算時數取決於該周內的天數是任務「工期」的一部分。 週末會從此分佈中排除。 當按月或季度顯示資源規劃工具，以及任務跨越多個月或季度時，其作用類似。

* 您可以選取預算時數作為新報告的報告物件，來報告預算時數。

  如需您可以在Workfront中報告哪些物件的相關資訊，請參閱[瞭解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一文中的「報告物件」一節。

  如需有關建立預算時數報表的資訊，請參閱文章[報表：預算時數](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md)。

* 先前為稍後停用的使用者編列的時數不會顯示。

  請注意，專案的預算勞力成本仍包含已在資源規劃工具中停用的使用者的預算時數。

  例如：如果角色指派給兩個使用者，且已新增預算時數（每個使用者20小時，總計40小時），然後手動設定該角色的總計，則停用資源規劃工具中的其中一個使用者會導致在計算中不再考慮其時數（將總時數降至20小時）。 但是，專案預算會正確保留手動設定的角色總計，因此停用的使用者小時仍會包含在計算中（保持在40小時）。

### VAR （變數）欄 {#the-var-variance-column}

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
   <td> <p>時數、FTE或成本差異會顯示您是否有足夠的專案預算時數來完成專案的所有計畫時數。 </p> <p>專案小時、約當全職人數或成本差異的計算公式如下：</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>時數、FTE或成本差異會顯示您是否有足夠的預算時數、FTE或成本供角色完成指派給它的計畫時數。 </p> <p>角色時數、約當全職人數或成本差異的計算公式如下：</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td> <p>時數、FTE或成本差異會顯示您是否有足夠的預算時數可供使用者完成指派給他們的計畫時數。 </p> <p>「使用者時數」、「約當全職人數」或「成本差異」的計算公式如下：</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>當時數、FTE或成本差異以紅色顯示時，您預估的預算時數少於需要完成之實際工作的計畫時數。 在此情況下，預算時數可能不足以完成工作。

### NET欄  {#the-net-column}

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
     <p>專案的「淨時數」、「約當全職人數」或「成本」會顯示下列其中一項： </p> 
     <ul> 
      <li> <p>可用的時間或成本與專案的預算時間或成本之間的差異：</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>啟用NET計算設定中的「使用計畫(PLN)」值時，專案的可用時間或成本與計畫時間或成本之間的差異： </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>秘訣</b></p>        
  <p>只有當您自訂「顯示選取的專案」區段中的檢視時，才會套用此選項。</p>
  <p>如需詳細資訊，請參閱<a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >使用Adobe Workfront資源規劃工具</a>檢閱資源可用性和配置 </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> 
    <div> 
     <p>「淨時數」、「約當全職人數」或「成本」角色會顯示下列其中一項： </p> 
     <ul> 
      <li> <p>可用時間或成本與角色的預算時間或成本之間的差異：</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>當在NET計算設定中啟用使用計畫(PLN)值時，可用時間或成本與角色的計畫時間或成本之間的差異：</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>秘訣</b> <span>

只有當您自訂[顯示選取的專案]區段中的檢視時，才會套用此選項。</span> </p> <p><span>如需詳細資訊，請參閱</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront資源規劃工具檢閱資源可用性和配置</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>使用者</td> 
   <td> 
    <div> 
     <p>使用者「淨時數」、「約當全職人數」或「成本」會顯示下列其中一項： </p> 
     <ul> 
      <li> <p>可用的時間或成本與使用者的預算時間或成本之間的差異：</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>當在NET計算設定中啟用使用計畫(PLN)值時，可用的時間或成本與使用者的計畫時間或成本之間的差異：</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>秘訣</b> <span>

只有當您自訂[顯示選取的專案]區段中的檢視時，才會套用此選項。</span> </p> <p><span>如需詳細資訊，請參閱</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">使用Adobe Workfront資源規劃工具檢閱資源可用性和配置</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>當「淨時數」、「約當全職人數」或「成本」顯示為紅色時，沒有足夠的「可用時間」或「預算」可涵蓋與工作相關的預算或計畫時間或成本。 在這種情況下，資源會過度配置。

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
