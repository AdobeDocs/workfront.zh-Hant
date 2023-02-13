---
product-area: resource-management
navigation-topic: resource-utilization
title: 查看資源利用資訊
description: 您可以使用「利用率」報告查看資源的利用率。
author: Alina
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '7758'
ht-degree: 0%

---

# 查看資源利用資訊

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

您可以使用「利用率」報告查看資源的利用率。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## 存取需求

您必須具備以下條件才能訪問「利用率」報告：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高存取權：</p> 
    <ul> 
     <li> <p>資源管理 </p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>專案組合</p> </li> 
     <li> <p>計劃</p> </li> 
     <li> <p>財務資料（如果要按成本查看資訊）</p> </li> 
    </ul> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看對項目、產品組合和程式的訪問權限，以訪問「資源配置」區域中的「利用率」部分</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>管理對項目的訪問權限以訪問項目的「利用率」部分</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

以下各節介紹如何查看和使用利用率資訊。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## 利用率報告概述 {#overview-of-the-utilization-report}

使用「利用率」報告，您可以在單個報告中查看項目、項目群或產品組合的進度、成本或收入。 您也可以比較收入與成本。

您可以在「資源」區域中查看「利用率」報表，以顯示多個項目的利用率，也可以在一個項目的級別查看它，以顯示與該項目關聯的單個資源（職務角色和用戶）的利用率。

有關訪問和使用「利用率」報告的資訊，請參閱 [使用「利用率」報告跟蹤進度、成本和收入](#track-progress-cost-and-revenue-with-the-utilization-report) 一節。

* [追蹤時數（進度）](#track-hours-progress)
* [追蹤成本](#track-cost)
* [追蹤收入](#track-revenue)
* [比較收入與計畫成本和實際成本](#compare-revenue-against-planned-and-actual-costs)

### 追蹤時數（進度） {#track-hours-progress}

您可以查看預算小時數和計畫小時數與實際小時數的比較，以跟蹤進度。

在跟蹤項目、項目群或項目組合的進度時，針對任務和問題的進度都包括在「利用率」報告中。

跟蹤小時數時，「利用率」報告中提供以下資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>檢視小時數時的欄標題</strong> </th> 
   <th><strong>函數</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>預算時數</strong> </td> 
   <td scope="col"> <p>所包括項目的總預算小時數。 您可以查看包含的項目的整個生命週期的總預算小時數，也可以僅查看指定日期範圍內的總預算小時數（您可以指定單個周或月）。 </p> <p>預算小時數是從「業務案例」或「資源計畫員」的新「資源預算」區域中可用的資訊填入的<em>.</em></p> <p>預算小時數顯示在以下任意行中的「利用率」報告中：</p> 
    <ul> 
     <li> 在「利用率」報告中，按職務職責和單個用戶匯總預算的工時，如下所示：<br><strong>個別使用者：</strong> 使用率報告中會匯總每個用戶的預算小時數。 這些預算小時數與用戶在包含的項目上分配給的任務和問題相關聯。 （您可以展開對應工作角色的列，以檢視具有該工作角色的使用者清單。）<br><strong>工作角色：</strong> 預算小時數按工作職責匯總在利用率報告中。<br>由於以下任何情況，預算的小時數會出現在特定職務角色中： 
     <li>作業角色定義為分配給任務或與預算小時數關聯的問題的用戶的主要作業角色。 </li> 
       <li>查看單個項目的利用率資訊時，無論任務或問題上沒有分配，還是沒有分配給另一個用戶，沒有分配任務角色，分配另一個用戶具有不同的作業角色，或分配另一個團隊，都會使用分配小時的用戶的作業角色。</li> 
       <li>當您查看多個項目、項目群或產品組合的利用率資訊時，只有在為項目中的任務或問題分配了該角色時，才會使用分配了該小時的用戶的作業角色。 </li> 
       <li>作業角色被分配給與預算小時數關聯的任務或問題，而分配給該任務或問題的用戶沒有在系統中定義作業角色。</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>未分配小時數</strong>:當預算小時數與任務或問題相關聯，且未分配任務或問題的用戶或角色時，預算小時數將顯示在「未分配小時數」部分的利用率報告中。<br>只有當項目上有符合此描述的小時，以及按項目或從項目查看「利用率」報表時，才會顯示此部分。 </p> <p>只有當項目上有符合此描述的小時，以及按項目或從項目查看「利用率」報表時，才會顯示此部分。 </p> </li> 
    </ul> <p>如需有關預算小時數的詳細資訊，請參閱 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解項目的預算人工成本和預算工時</a> 文章。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫小時</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
與每個任務和問題的分配關聯的所包括項目的計畫小時數。 您可以查看項目上所有分配在包含的項目的整個生命週期中的總計畫小時數，或者您只能查看指定日期範圍內的總計畫小時數（您可以指定單個周或月）。 
</p>
<p>
<strong>筆尖 </strong>
</p>
<p>
不會考慮來自持續時間為0的項目的計畫小時數。 
</p>
<p>
「利用率」報表中的「計畫小時數」將考慮計畫小時數是否已在任務或問題的整個期間重新分配。 
</p>
<p>
使用工作負載平衡器修改了用戶的小時的每日分配時，如果「利用率」報告中選擇的日期僅包含任務或問題的持續時間的一部分，則可能會影響「利用率」報告中的資料。 
</p>
<p>
有關修改用戶分配的資訊，請參閱 <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">在工作負載平衡器中管理用戶分配</a>.


</p>
<p>
「計畫小時數」(Plannedd Hours)顯示在以下任意行中的「利用率」(Utilization)報告中：
</p>
<ul>

<li>計畫小時數按職務職責和使用率報告中的個別用戶匯總，如下所示： 
<ul>

<li><strong>個別使用者</strong>:在利用率報告中匯總了每個用戶的計畫小時數。 這些「計畫小時數」與用戶在包含的項目上被分配給的任務和問題相關聯。 （您可以展開對應工作角色的列，以檢視具有該工作角色的使用者清單。）

<li><strong>工作角色</strong>:在單個項目的利用率報告中，按職務職責匯總計畫小時數。<br>計畫小時數會因下列任何情況而出現在特定作業角色中：  
<ul>

<li>作業角色定義為分配給任務或與計畫小時數相關聯的問題的用戶的主要作業角色。

<li>在以下情況下，查看單個項目的利用率資訊時，與作業角色關聯的小時數不會針對作業角色顯示：   
<ul>

<li>任務或問題上沒有分配

<li>分配的用戶沒有分配任務角色

<li>為用戶分配了不同的作業角色

<li>已為任務或問題分配一個小組
</li>   
</ul>

<li>當您查看多個項目、項目群或產品組合的利用率資訊時，只有在為項目中的任務或問題分配了該角色時，才會使用分配了該小時的用戶的作業角色。 查看多個項目的「利用率」報告時，任務職責小時數不單獨顯示。

<li>作業角色被分配給與計畫小時數關聯的任務或問題，而分配給任務或問題的用戶在系統中沒有定義作業角色。
</li>  
</ul>

<li><strong>未分配小時數</strong>:當「計畫小時數」與任務或問題關聯，並且沒有為任務或問題分配用戶或角色時，「計畫小時數」將顯示在「未分配小時數」部分的「利用率」報表中。僅當項目上存在與此說明匹配的小時數以及查看單個項目的「利用率」報表時，才會顯示此部分。 <br>有關計畫時間的詳細資訊，請參閱 <a href="../../manage-work/tasks/task-information/planned-hours.md">計畫小時數概觀</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>實際工作</strong> </td> 
   <td> <p> 記錄任務、問題、 <span>和項目</span> ，針對包含的專案。 您可以查看包含的項目的整個有效期內的實際總小時數，也可以僅查看指定日期範圍內的實際總小時數（您可以指定單個周或月）。 </p> <p>警告：利用率報告包括記錄到項目的小時數、子任務、問題和至少具有一個分配的父任務。 它不包括記錄到沒有分配的父任務的小時數。 建議您不要使用父任務作為工作任務，並僅將子任務指派給資源。 </p> <p>以下任意行中的「實際小時數」(Actual Hours)出現在「利用率」報告中：</p> 
    <ul> 
     <li> 在項目的利用率報告中，按職務職責和個別用戶匯總實際工時，如下所示：<br><strong>個別使用者：</strong> 實際小時數顯示在利用率報告中記錄小時數的用戶行中。 （您可以展開對應工作角色的列，以檢視具有該工作角色且已記錄小時的使用者清單。）<br><strong>工作角色：</strong> 與這些角色關聯的用戶記錄的實際小時數將匯總在相應作業角色行的利用率報告中。<br>由於以下任何情況，特定作業角色中會出現實際小時數： 
      <ul> 
       <li>作業角色定義為記錄小時數之使用者的主要作業角色。</li> 
       <li>任務或問題上沒有分配</li> 
       <li>分配了另一個用戶，但沒有分配任務角色</li> 
       <li>另一個用戶被分配了不同的作業角色</li> 
       <li> <p>已指派一個團隊。</p> </li> 
      </ul></li>  
     <p>如果記錄小時的用戶沒有與其配置檔案關聯的作業角色，則「利用率」報告中使用的作業角色是分配給任務或問題的作業角色，其中記錄了小時，或與任務或問題的「主要所有者」關聯的作業角色。 </p> 
     <li><strong>其他小時：</strong> 實際小時數顯示在「其他小時數」部分的「利用率」報告中，該小時位於登錄用戶的行中。<br>記錄小時的用戶未在系統中定義作業角色時，小時數將顯示在此部分。<br>只有在項目上有符合此說明的小時時，才會顯示此部分。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>預算差異（小時數）</strong> </td> 
   <td> <p>預算小時總數減去所包括項目的實際小時總數。 您可以查看包含的項目的整體壽命的預算差異總額，也可以僅查看指定日期範圍的預算差異總額（您可以指定單個周或月）。 </p> <p>如果值為正數，則會以綠色顯示。 這表示總預算小時數大於實際小時數。</p> <p>如果值為負，則會以紅色顯示。 這表示預算小時總數小於實際小時數。</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>計畫差異（小時數）</strong> </td> 
   <td> <p>總計畫小時數減去包含項目的實際總時數。 您可以查看包含的項目的整個使用壽命的計畫差異合計，也可以僅查看指定日期範圍的計畫差異合計（您可以指定單個周或月）。</p> <p>如果值為正數，則會以綠色顯示。 這表示總計畫小時數大於實際小時數。</p> <p>如果值為負，則會以紅色顯示。 這表示總計畫小時數小於實際小時數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 追蹤成本 {#track-cost}

您可以查看預算成本和計畫成本與實際成本的比較來跟蹤成本。

跟蹤項目、項目群或產品組合的成本時，「利用率」報告中的資訊來自任務。 「利用率」報告中始終提供任務的成本資訊。 任務成本是根據任務的成本類型計算的。 有關任務成本類型的資訊，請參閱 [追蹤成本](../../manage-work/projects/project-finances/track-costs.md).

您可以通過以下方式在「利用率」報表上顯示成本資訊：

* 針對指定的周或月，或整體專案、方案或產品組合。
* 依角色或個人，針對專案。

利用率報表上使用的幣種由項目上設定的幣種確定。 有關如何調整項目貨幣的資訊，請參閱 [更改項目幣種](../../manage-work/projects/project-finances/change-project-currency.md).

跟蹤成本時，「利用率」報告中提供以下資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>查看成本時的列標題</strong> </th> 
   <th> <p><strong>函數</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>預算成本</strong> </td> 
   <td scope="col"> <p>已包括項目的預算成本。 您可以查看包含項目的整體使用期的預算成本合計，也可以僅查看指定日期範圍的預算成本合計（您可以指定單個周或月）。</p> <p>由於「利用率報表中的預算成本」按職責分列，因此其計算方式與Workfront其他地區的預算人工成本相同。 有關如何計算預算人工成本的資訊，請參閱 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解項目的預算人工成本和預算工時</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫成本</strong> </td> 
   <td scope="col"> <p>包含項目的總計畫成本。 您可以查看包含的項目的整個生命週期的計畫成本合計，也可以僅查看指定日期範圍的計畫成本合計（您可以指定單個周或月）。</p> <p>有關如何計算項目計畫成本的資訊，請參閱文章中的「Workfront如何計算計畫成本、預算成本和實際成本」一節 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>實際成本</strong> </td> 
   <td scope="col"> <p>包含項目的實際總成本。 您可以查看包含的項目的整個有效期內的「實際成本合計」，也可以僅查看指定日期範圍內的「實際成本合計」（您可以指定單個周或月）。</p> <p>有關如何計算項目實際成本的資訊，請參閱文章中的「Workfront如何計算計畫成本、預算成本和實際成本」一節 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>預算差異（成本）</strong> </td> 
   <td scope="col"> <p>預算總成本減去所包括項目的實際總成本。 您可以查看包含的項目的整體壽命的預算差異總額，也可以僅查看指定日期範圍的預算差異總額（您可以指定單個周或月）。</p> <p>如果值為正數，則會以綠色顯示。 這表示總預算成本大於實際成本。</p> <p>如果值為負，則會以紅色顯示。 這表示總預算成本小於實際成本。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>計畫差異（用於成本）</strong> </td> 
   <td> <p>總計畫成本減去已包括項目的總實際成本。 您可以查看包含的項目的整個使用壽命的計畫差異合計，也可以僅查看指定日期範圍的計畫差異合計（您可以指定單個周或月）。 </p> <p>如果值為正數，則會以綠色顯示。 這表示總計畫成本大於實際成本。</p> <p>如果值為負，則會以紅色顯示。 這表示總計畫成本小於實際成本。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 追蹤收入 {#track-revenue}

您可以檢視預算和計畫收入與實際收入的比較，以追蹤收入。

跟蹤項目、項目群或產品組合的收入時，「利用率」報告中僅包括來自任務的收入。

追蹤收入時，下表中的資訊可在「利用率」報表中取得。

如需特定欄位及Workfront計算欄位方式的資訊，另請參閱下列文章：

* [追蹤成本](../../manage-work/projects/project-finances/track-costs.md)
* [帳單和收入概觀](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>檢視收入時的欄標題</strong> </th> 
   <th> <strong>函數</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>預算收入</strong> </td> 
   <td scope="col"> <p>總預算小時數乘以所包括項目的「職責開單率」。 您可以查看包含項目的整體使用期內的總預算收入，也可以僅查看指定日期範圍內的總預算收入（您可以指定單個周或月）。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫收入</strong> </td> 
   <td scope="col"> <p>「利用率」報表中的「計畫收入」是與分配給項目任務的資源的「計畫時數」關聯的收入。</p> <p>Workfront使用以下公式計算「利用率」報表的項目計畫收入：</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>附註</b>
   <p>「利用率」報表中顯示的項目計畫收入與「項目詳細資訊」區域和項目報表中顯示的計畫收入不同。 </p> <p>「項目詳細資訊」區域中的「計畫收入」將反映項目的任務收入和固定收入。 「利用率報表」中的「計畫收入」僅顯示與項目中的任務關聯的「計畫收入」。 </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>如果項目有1個10小時的任務，並分配給一個每小時費率為$20的顧問，而項目有$100的固定收入，則「利用率」報表將顯示「計畫收入」為$200（與任務上的小時相關聯的計畫收入）。 「項目詳細資訊」部分顯示$300（任務的計畫收入和項目的固定收入）。 </p> 
     </div> <p>有關「利用率」報表外的任務和項目計畫收入的詳細資訊，請參閱 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a>.</p> </p> <p>「利用率」報表計算和顯示已包括項目的計畫收入的方式將考慮任務上設定的收入類型。 </p> <p>根據項目中每個任務的「收入類型」，存在以下方案： </p> <p><strong>固定收入：</strong> 無論任務分配如何，任務上的收入始終使用任務上指定的固定金額計算。</p> <p><b>重要</b>

與Workfront的其他區域不同，「利用率」報表通過將固定收入平均除以任務上的計畫小時數來計算固定收入任務的計畫收入。 </p> <p>例如，任務的收入為$200。 如果任務中有4個計畫小時，則每小時為$50。 這會分發在使用者和角色層級。 此分配對「利用率」報告是唯一的。</p> <p><b>附註</b>

如果您有「固定收入」任務，並且該任務沒有「計畫小時數」，則「收入」不會顯示在「利用率」報表中，因為沒有方法將其分配給小時數。 如果您在具有固定收入且沒有分配的任務上具有計畫小時數，則收入將顯示為未分配收入。 </p> <p><strong>每小時角色：</strong> 任務上的收入使用特定職責的開單率集乘以與該職責關聯的計畫小時數來計算。 Workfront使用下列公式：</p> <p>職責每小時計畫收入= SUM（所有任務中職責的計畫小時數）*職責開單率</code></p> <p><strong>每小時用戶：</strong> 任務上的收入是使用特定用戶的開單費率集乘以與該用戶關聯的計畫小時數來計算的。 Workfront使用下列公式：</p> <p>用戶每小時計畫收入= SUM（所有任務中用戶的計畫小時數）*用戶開單率</code> </p> <p><b>角色每小時或用戶每小時加固定</b> </p> <p><b>重要</b>

與Workfront的其他區域不同，「利用率」報表通過將固定收入除以任務上的計畫小時數來計算計畫收入。 </p> <p>存在下列情況： </p>
<ul>
<li> <p><strong>角色每小時加固定：</strong> 任務上的收入使用特定職責的開單費率集乘以與職責關聯的計畫小時數來計算。 此外，在任務上指定的固定金額將添加到角色比率中。 Workfront使用下列公式：</p> <p>每小時角色加固定計畫收入= [SUM（所有任務上的角色計畫小時數）*角色開單率] + SUM（任務的上限或固定金額/任務的計畫小時數）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>每小時用戶加固定值：</strong> 為特定用戶設定的開單費率，乘以該用戶的任務上的計畫小時數。 此外，在任務上指定的固定金額被添加到用戶費率中。 Workfront使用下列公式：</p> <p>使用者每小時加固定計畫收入= [SUM（所有任務中來自用戶的計畫小時數）*用戶計費率] + SUM（任務的上限或固定金額/任務的計畫小時數）</code> </p> </li>
</ul> <p><b>角色或用戶每小時數（含上限）</b> </p> <p><b>重要</b>

與Workfront其他地區不同，如果計畫收入超過上限，超出上限金額的金額即視為固定收入。 「計畫收入」的計算方式是將固定收入除以任務上的「計畫小時數」，然後將「上限金額」和角色或用戶每小時收入相加。 <br></p> <p>存在下列情況： </p>
<ul>
<li> <p><strong>每小時角色/上限：</strong> 任務在「角色每小時」中按小時計費，但您可以指定任務的最大限額。 Workfront使用下列公式：</p> <p>每小時角色（具有上限）計畫收入= [SUM（所有任務和問題上的角色計畫小時數）*角色開單率] +任務的上限額+ SUM（超過上限額的金額/任務的計畫小時數）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>每小時用戶數/上限：</strong> 任務按每小時用戶計費，但您可以指定任務的最大限額。 Workfront使用下列公式： </p> <p>使用者每小時計畫收入上限= [SUM（所有任務中來自用戶的計畫小時數）*用戶計費率] +任務的上限額+ SUM（超過上限額的金額/任務的計畫小時數）</code> </p> </li>
</ul> <p>有關計算計畫收入時要考慮哪些角色或用戶的詳細資訊，請參閱 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>實際收入</strong> </td> 
   <td> <p>「實際收入」是與任務的「實際小時數」關聯的收入 <span>和</span>. 如需實際收入的詳細資訊，請參閱文章中的「追蹤收入金額」一節 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a>.</p>

<p>「利用率」報表計算所包括項目的「實際收入」的方式因任務上設定的「收入類型」而異，如下所示：</p> <p><strong>固定收入：</strong> 無論任務分配如何，任務上的收入始終使用任務上指定的固定金額計算。</p> <p><b>重要</b>

與Workfront的其他區域不同，「利用率」報表通過將固定收入平均除以任務記錄的小時數來計算實際收入。 </p> <p> </p> <p>例如，任務的實際收入為$200。 如果任務中有4個實際小時，則每小時為$50。 這會分發在使用者和角色層級。 此分配對「利用率」報告是唯一的。</p> <p><b>附註</b>

如果您有「固定收入」任務，並且該任務沒有「實際小時數」，則「實際收入」不會顯示在「利用率報表」中，因為無法分配小時數。 </p> <p><strong>每小時角色：</strong> 任務上的收入使用特定職責的開單率集乘以計畫小時數來計算。</p> <p>Workfront使用下列公式：</p> <p>角色每小時實際收入= SUM（所有任務中角色的實際小時數）*角色開單率</code> </p> <p><strong>每小時用戶：</strong> 任務上的收入是使用特定用戶的計費率集，乘以該用戶針對任務記錄的小時數來計算的。 Workfront使用下列公式：</p> <p>用戶每小時實際收入= SUM（所有任務中用戶的實際小時數）*用戶開單率</code></p> <p><b>角色或用戶每小時加固定</b> </p> <p><b>重要</b>

與Workfront的其他區域不同，「利用率」報表通過將固定收入平均除以任務記錄的小時數來計算實際收入。 </p> <p>存在下列情況： </p>
<ul>
<li> <p><strong>角色每小時加固定：</strong> 為特定角色設定的計費比率，乘以該角色的用戶針對任務記錄的小時數。 此外，在任務上指定的固定金額將添加到角色比率中。 </p> <p>Workfront使用下列公式：</p> <p>每小時角色加固定實際收入= [SUM（所有任務上角色的實際小時數）*角色開單率] + SUM（任務的上限或固定數量/任務的實際小時數）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>每小時用戶加固定值：</strong> 為特定用戶設定的計費率，乘以該用戶針對任務記錄的小時數。 此外，在任務上指定的固定金額被添加到用戶費率中。 </p> <p>Workfront使用下列公式：</p> <p>使用者每小時加固定實際收入= [SUM（所有任務上角色的實際小時數）*用戶計費率] + SUM（任務的上限或固定數量/任務的用戶小時數）</code> </p> </li>
</ul> <p><b>角色或用戶每小時數（含上限）</b> </p> <p><b>重要</b>

與Workfront其他地區不同，如果計畫收入超過上限，超出上限金額的金額即視為固定收入。 「計畫收入」的計算方式是將固定收入除以任務上的「計畫小時數」，然後將「上限金額」和角色或用戶每小時收入相加。 <br></p> <p>存在下列情況：</p>
<ul>
<li> <p><strong>每小時角色/上限：</strong> 任務在「角色每小時」中按小時計費，但您可以指定任務的最大限額。 Workfront使用下列公式：</p> <p>每小時角色（含上限）實際收入= [SUM（所有任務和問題上角色的實際小時數）*角色開單率] +任務的上限額+ SUM（超過上限額的金額/任務的實際小時數）</code></p> </li>
</ul>
<ul>
<li> <p><strong>每小時用戶數/上限：</strong> 任務按每小時用戶計費，但您可以指定任務的最大限額。</p> <p> Workfront使用下列公式：</p> <p>具有上限的使用者每小時實際收入= [SUM（所有任務和問題上角色的實際小時數）*用戶計費率] +任務的上限額+ SUM（超過上限額的金額/任務的實際小時數）</code> </p> </li>
</ul>
<div>
<p><strong>項目收入</strong>:計算與項目上記錄的小時數相關聯的收入時，會考慮記錄該時間的用戶的主要工作角色的「按小時計費」金額。 我們不建議在專案上記錄時間。 </p>
<p><b>附註</b>

如果用戶未與職務職責關聯，或者主要職責的每小時開單為零，則Workfront會使用用戶的每小時開單金額計算實際收入。 如果使用者的設定檔中沒有每小時計費金額，則實際收入為零。 </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>預算差異（收入）</strong> </td> 
   <td> <p>包含項目的「實際收入」減去「預算收入」。<br>您可以查看包含的項目的整體壽命的預算差異總額，也可以僅查看指定日期範圍的預算差異總額（您可以指定單個周或月）。</p> <p>如果值為正數，則會以綠色顯示。 這表示總預算收入大於實際收入。</p> <p>如果值為負，則會以紅色顯示。 這表示總預算收入小於實際收入。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>計畫差異（用於收入）</strong> </td> 
   <td> <p>「實際收入」總計減去包含項目的「計畫收入」總計。<br>您可以查看包含的項目的整個使用壽命的計畫差異合計，也可以僅查看指定日期範圍的計畫差異合計（您可以指定單個周或月）。 </p> <p>如果值為正數，則會以綠色顯示。 這表示總計畫收入大於實際收入。</p> <p>如果值為負，則會以紅色顯示。 這表示總計畫收入小於實際收入。</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### 比較收入與計畫成本和實際成本 {#compare-revenue-against-planned-and-actual-costs}

您可以查看計畫收入和計畫成本。 也會顯示毛利(%)（毛利以「收入 — 成本/收入」計算）。

在比較收入與計畫成本和實際成本時，「利用率」報表中提供以下資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>檢視收入與成本時的欄標題（計畫）</strong> </th> 
   <th> <strong>函數</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>計畫成本</strong> </td> 
   <td scope="col"> 包含項目的總計畫成本。 您可以查看包含的項目的整個生命週期的計畫成本合計，也可以僅查看指定日期範圍的計畫成本合計（您可以指定單個周或月）。 </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫收入</strong> </td> 
   <td scope="col"> <p>計畫收入是與任務的計畫小時數關聯的收入。 </p> <p>「利用率」報表計算和顯示已包括項目的計畫收入的方式因任務上設定的「收入類型」而有所不同，如 <a href="#track-revenue" class="MCXref xref">追蹤收入</a> 一節。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>邊界</strong> </td> 
   <td scope="col"> <p>毛利百分比的計算方式如下：</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>附註</b>

如果計畫收入等於0，則利潤顯示為0。 </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>檢視收入與成本時的欄標題（實際）</strong> </p>  </td> 
   <td scope="col"><p><strong>函數</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>實際成本</strong> </td> 
   <td scope="col"> <p>包含項目的實際總成本。 您可以查看包含的項目的整個有效期內的「實際成本合計」，也可以僅查看指定日期範圍內的「實際成本合計」（您可以指定單個周或月）。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>實際收入</strong> </td> 
   <td> <p>「實際收入」是與任務的「實際小時數」關聯的收入。</p> <p>實際收入僅在任務標籤為「完成」或「完成」（或與「完成」相等的狀態）後才顯示在「利用率」報表中。</p> <p>「利用率」報表計算所包括項目的「實際收入」的方式因任務上設定的「收入類型」而有所不同，如 <a href="#track-revenue" class="MCXref xref">追蹤收入</a> 一節。 </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>邊界</strong> </td> 
   <td> <p>毛利百分比的計算方式如下：</p> <p>實際收入 — 實際成本/實際收入x 100。 </p> <p><b>附註</b>

如果實際收入等於0，則利潤會顯示為0。 </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## 使用「利用率」報告跟蹤進度、成本和收入 {#track-progress-cost-and-revenue-with-the-utilization-report}

您可以追蹤專案、方案或產品組合的進度或成本。

您可以顯示指定周或月的「利用率」報告或項目總壽命的資訊。

要跟蹤具有「利用率」報表的一個或多個項目的進度或成本，請執行以下操作：

1. 根據您是查看單個項目、多個項目、項目群還是產品組合的利用率資訊，執行以下任一操作：

   * 要查看單個項目的利用率資訊，請執行以下操作：

      1. 轉到要查看其利用率資訊的項目，然後按一下 **顯示更多>利用率**.
      1. 檢視個別專案時，會自動顯示使用率資訊，且不需要套用篩選器。\
         如果要篩選「利用率」報表，可以套用篩選，然後按一下 **執行**.\
         有關如何篩選「利用率」報表的資訊，請參閱 [篩選利用資訊](#filter-utilization-information) 這篇文章。\
         系統會顯示個別使用者和角色的使用率資訊（使用者會在其相關聯角色中分組）。
   * 要查看多個項目的利用率資訊，請執行以下操作：

      1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 中。
      1. 將篩選器應用於「利用率」報表，然後按一下 **執行**.\
         在運行「利用率」報表之前，必須在篩選器中指定一個或多個項目。 有關如何篩選「利用率」報表的資訊，請參閱 [篩選利用資訊](#filter-utilization-information) 這篇文章。\
         系統會顯示各個角色和項目的利用率資訊（將角色分組到其關聯項目中）。
   * 要查看程式的利用率資訊，請執行以下操作：

      1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 在左側面板中，按一下 **顯示**>**方案**.
      1. 將篩選器應用於「利用率」報表，然後按一下 **執行**.\
         在運行「利用率」報表之前，必須在篩選器中指定一個或多個程式。 有關如何篩選「利用率」報表的資訊，請參閱 [篩選利用資訊](#filter-utilization-information) 這篇文章。\
         顯示個別項目和方案的利用率資訊（項目在其關聯方案中分組）。
   * 要查看產品組合的利用率資訊，請執行以下操作：

      1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 在左側面板中，按一下 **顯示**>**Portfolio**.
      1. 將篩選器應用於「利用率」報表，然後按一下 **執行**.\
         在執行「利用率」報表之前，您必須在篩選器中指定一或多個產品組合。 有關如何篩選「利用率」報表的資訊，請參閱 [篩選利用資訊](#filter-utilization-information) 這篇文章。\
         顯示個別項目、項目群和產品組合的利用率資訊（項目在其關聯項目中分組，方案在其關聯項目組合中分組）。




1. 在「利用率」報告的右上角，按一下 **檢視** 下拉式功能表，然後選取下列項目：

   * **成本**
   * **時數**
   * **收入**
   * **收入 vs. 成本 (計畫)**
   * **收入與成本（實際）**.

   您選取的選項會決定報表中可用的欄和資訊。 如需各欄中可用資訊的詳細資訊，請參閱步驟5中的表格。\
   ![](assets/utilization-view-dropdown.png)

1. （可選）選擇要顯示其利用率資訊的日期範圍。 您可以在 **整體** 欄。 整體專案、方案或產品組合的資訊一律顯示在 **整體** 欄。\
   如需詳細資訊，請參閱 [調整顯示資訊的日期範圍](#adjust-the-date-range-for-which-information-is-displayed) 這篇文章。

1. （可選）按一下任何列標題，按該列中的資訊對利用率報告進行排序。 排序只有在報表中包含多個項目時才有效。 例如，當您查看多個專案（或產品組合或方案）時，可以排序報表結果。 一次只查看一個項目（或一個項目組合或一個方案）時，無法對結果進行排序。
1. 使用區段中的資訊 [利用率報告概述](#overview-of-the-utilization-report) 以了解「利用率」報告中的每一列。

## 篩選利用資訊 {#filter-utilization-information}

您可以篩選專案的「使用率」報表中顯示的內容。 您可以篩選任務、問題、角色和自訂資料。 將篩選器應用於「利用率」報表時，「利用率」報表將根據您選擇的標準包含資訊。

您可以建立篩選，或套用您先前建立的篩選。

* [建立或修改篩選器](#create-or-modify-a-filter)
* [套用儲存的篩選](#apply-a-saved-filter)
* [複製篩選器](#duplicate-a-filter)
* [重新命名篩選器](#rename-a-filter)
* [刪除篩選器](#delete-a-filter)

### 建立或修改篩選器 {#create-or-modify-a-filter}

建立篩選器時，所有可存取「利用率」報表的Workfront使用者也可存取您建立的篩選器。 同樣地，當您修改現有篩選器時，將為所有有權訪問「利用率」報告的用戶修改該篩選器。

要建立或修改篩選器，請執行以下操作：

1. 要篩選單個項目的利用率資訊，請轉至要篩選利用率資訊的項目，然後按一下 **顯示更多>利用率** 中。

   或

   要篩選多個項目、方案或產品組合的利用率資訊，請按一下「主菜單」表徵圖 ![](assets/main-menu-icon.png) 在Workfront的右上角， **資源**, **利用率** 在左側面板中，然後 **顯示**>**方案** 或 **Portfolio** 或&#x200B;**專案**.

1. 按一下 **篩選** 圖示來顯示篩選選項。

1. （條件性）若要修改現有篩選，請按一下 **篩選** 下拉式功能表，然後選取您要修改的篩選器。
1. 指定下列資訊以建立或修改篩選器：

   * **Portfolio:** 開始鍵入包含您要包括在「利用率」報表中的資訊的產品組合名稱，然後在下拉菜單中顯示該名稱時按一下。\
      重複此過程，在「利用率」報告中包括來自多個產品組合的資訊。\
      若要在篩選器中納入系統的所有產品組合，請按一下 **全部新增**. （只有在系統中的產品組合少於10個時，才可使用此選項。）

   * **計畫：** 開始鍵入包含要包括在「利用率」報告中的資訊的程式的名稱，然後在下拉菜單中顯示該名稱時按一下。\
      重複此過程，在「利用率」報告中包括來自多個任務的資訊。\
      如果您已在篩選中指定任何產品組合，您指定的方案必須來自已包含在篩選中的產品組合。 如果未包含，則來自程式的資料不會包含在「利用率」報告中。\
      若要將系統中的所有程式納入篩選器，請按一下 **全部新增**. （只有在您的系統中的程式少於20個時，才可使用此選項。）

   * **專案：** 開始鍵入項目名稱（其中包含您要在「利用率」報表中包括的資訊），然後在下拉菜單中顯示該名稱時按一下。\
      重複此過程，在「利用率」報告中包括來自多個項目的資訊。\
      如果您已在篩選器中指定任何產品組合或方案，您指定的專案必須來自篩選器中已包含的其中一個產品組合或方案。 如果未包含，則來自項目的資料不會包含在「利用率」報告中。\
      若要在篩選器中納入系統中的所有專案，請按一下 **全部新增**. （只有在系統中的專案少於250個時，才能使用此選項。）

   * **任務：** 開始鍵入任務的名稱，該任務包含您要在「利用率」報表中包括的資訊，然後在下拉菜單中顯示該名稱時按一下該名稱。\
      重複此過程，在「利用率」報告中包括來自多個任務的資訊。\
      如果您已在篩選器中指定任何產品組合、方案或專案，您指定的任務必須來自篩選器中已包含的其中一個產品組合、方案或專案。 如果未包含，則任務中的資料不會包含在「利用率」報告中。

   * **問題：** 開始鍵入問題名稱，該名稱包含您要在「利用率」報告中包括的資訊，然後在下拉菜單中顯示該名稱時按一下該名稱。\
      重複此過程，在「利用率」報告中納入多個問題的資訊。\
      如果您已在篩選器中指定任何產品組合、方案或專案，您指定的問題必須來自篩選器中已包含的其中一個產品組合、方案或專案。 如果未包含，則問題中的資料不會包含在「利用率」報告中。\
      問題的成本資訊並不總是包含在「利用率」報告中。 有關問題成本資訊何時包括在「利用率」報表中的詳細資訊，請參閱 [使用「利用率」報告跟蹤進度、成本和收入](#track-progress-cost-and-revenue-with-the-utilization-report) 這篇文章。

   * **角色：** 開始在「利用率報告」中鍵入要表示的角色的名稱，然後在下拉菜單中顯示該名稱時按一下該名稱。 重複此過程以包含其他角色。\
      「利用率報告」僅包含您指定的角色的資訊。 例如，任務包含10個實際小時。 其中6小時來自設計人員角色，4小時來自開發人員角色。 如果按設計器角色篩選「利用率報表」，則來自「開發人員」角色的4小時將從報表中排除。

   * **新增篩選規則：** 按一下 **新增篩選規則**，按一下第一個欄位，然後開始輸入您要篩選的欄位名稱。 如果欄位可用，則會填入每個物件的關聯位置。 按一下欄位名稱，將其新增至篩選器。

      >[!IMPORTANT]
      >
      >您必須輸入欄位名稱，而非欄位標籤。 欄位標籤會顯示在附加至物件的自訂表單上。 如需自訂欄位名稱與標籤之間差異的詳細資訊，請參閱  [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

      如需您在欄中看到欄位的詳細資訊，請參閱 [Adobe Workfront術語表](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
      選擇篩選的篩選條件修飾元。 可用修改量在 [篩選條件修飾元](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. 若要建立新篩選器，請按一下 **儲存篩選**.\
   或\
   若要修改現有篩選器，請按一下 **儲存篩選** 按鈕，然後按一下 **儲存新篩選器**.\
   在 **篩選器名稱** 欄位，指定篩選器的名稱，然後按一下 **儲存**.\
   「利用率」區域會以您包含在篩選器中的資訊進行篩選。

### 套用儲存的篩選 {#apply-a-saved-filter}

1. 要對單個項目的「利用率報表」應用篩選器，請轉至要篩選的項目，然後按一下 **顯示更多>利用率** 中。

   或

   要對多個項目、方案或產品組合的「利用率報表」應用篩選器，請按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角， **資源**, **利用率** 在左側面板中，然後 **顯示**>**方案** 或&#x200B;**Portfolio** 或&#x200B;**專案**.

1. 按一下 **儲存的篩選**，然後從下拉式功能表中選取您要套用的篩選。

### 複製篩選器 {#duplicate-a-filter}

1. 要對單個項目的「利用率報表」複製篩選器，請轉至要為其複製篩選器的項目，然後按一下 **顯示更多>利用率** 中。

   或

   要對多個項目、方案或產品組合的「利用率報告」複製篩選器，請按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 中。

1. 按一下 **儲存的篩選**，將滑鼠移至下拉式功能表中您要複製的篩選器上方，然後按一下 **複製** 表徵圖。

   ![](assets/utilization-filter-duplicate.png)\
   將顯示「複製篩選器」對話框。

1. 在 **篩選器名稱** 欄位，指定新篩選器的名稱，然後按一下 **儲存**.

### 重新命名篩選器 {#rename-a-filter}

重新命名篩選器時，所有可存取「利用率」報表的Workfront使用者都會看到您選擇的新名稱。

若要重新命名篩選器：

1. 要更名單個項目的「利用率報告」上的篩選器，請轉至要為其更名篩選器的項目，然後按一下 **顯示更多>利用率** 中。

   或

   要更名多個項目、方案或產品組合的「利用率報告」上的篩選器，請按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 中。

1. 按一下 **儲存的篩選**，將滑鼠移至下拉式功能表中您要複製的篩選器上方，然後按一下 **重新命名** 表徵圖。\
   ![](assets/utilization-filter-rename.png)\
   將顯示「更名篩選器」對話框。

1. 在 **篩選器名稱** 欄位，指定新篩選器的名稱，然後按一下 **儲存**.

### 刪除篩選器 {#delete-a-filter}

刪除篩選器時，系統會為所有可存取「利用率」報表的Workfront使用者刪除篩選器。

若要刪除篩選器：

1. 要刪除單個項目的「利用率報告」上的篩選器，請轉至要刪除該篩選器的項目，然後按一下 **顯示更多>利用率** 中。

   或

   要刪除多個項目、方案或產品組合的「利用率報表」上的篩選器，請按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 中。

1. 按一下 **儲存的篩選**，將滑鼠移至下拉式功能表中您要複製的篩選器上方，然後按一下 **刪除** 表徵圖。

   ![](assets/utilization-filter-delete.png)

1. 按一下 **刪除** 當系統提示您是否要刪除篩選器時。

## 調整顯示資訊的日期範圍 {#adjust-the-date-range-for-which-information-is-displayed}

您可以調整顯示利用率資訊的日期範圍。 您可以選取過去或未來的日期。 您所做的變更只會顯示給您。

1. 要調整單個項目的「利用率報表」的日期範圍，請轉至要調整其日期範圍的項目，然後按一下 **顯示更多>利用率** 中。

   或

   要調整多個項目、方案或產品組合的「利用率」報告的日期範圍，請按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 中。

1. 按一下 **匯出** 按鈕。

   預設會選取目前的周。

1. 從下列選項中選取：

   * **周：** 選擇此選項以選取指定的周（從星期日到星期六）。
   * **月：** 選擇此選項以選取指定月份。

   您選擇的日期範圍將顯示在利用率報表中，位於 **整體** 欄。\
   Workfront會記住您要檢視周還是月。 下次訪問利用率報告時，將根據您選擇的選項顯示當前周或當月。

## 導出利用率資訊

您可以從Workfront導出項目、項目群或產品組合的利用率資訊。 資訊只能以XLSX、TSV和PDF格式匯出。

在Microsoft Excel中檢視時，負數會以括弧顯示。

要導出利用率資訊，請執行以下操作：

1. 要導出單個項目的利用率資訊，請轉至要導出利用率資訊的項目，然後按一下 **利用率** 標籤(視您的版面設定而定，這可能位於 **更多** 標籤)。

   或

   要導出多個項目、方案或產品組合的利用率資訊，請按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **資源**，然後 **利用率** 中。

1. 按一下 **匯出**，位於 **利用率** 標籤。

1. 從下列選項中選取：

   * **PDF:** 以PDF格式匯出報表。 如果您打算列印報表，建議使用此格式。\
      選取 **字母 — 縱向**, **字母 — 橫向**，或 **其他大小** (提供用於在法律（8.5英吋x 14英吋）、分類帳（11英吋x 17英吋）和A4中導出的選項。\
      視您使用的作業系統而定，您可能可以選擇開啟或儲存檔案。 開啟包含關聯應用程式的檔案或將其保存到硬碟。

   * **Excel:** 匯出XLSX格式的報表。 如果您打算在Excel中進一步分析資料，建議使用此格式。\
      視您使用的作業系統而定，您可能可以選擇開啟或儲存檔案。 開啟包含關聯應用程式的檔案或將其保存到硬碟。

   * **分隔標籤：** 匯出TSV格式的報表。 如果您打算將資料匯入協力廠商軟體以進行進一步分析，此為建議的格式。\
      視您使用的作業系統而定，您可能可以選擇開啟或儲存檔案。 開啟包含關聯應用程式的檔案或將其保存到硬碟。

1. 閱讀文章中的資訊 [匯出資料](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) 了解如何使用匯出的檔案。

## 在圖表中查看利用率資訊

您可以以圖表視圖將「利用率」報表中的資料視覺化。

1. 要以圖表格式查看單個項目的利用率報告，請轉至要查看的項目，然後按一下 **顯示更多>利用率** 中。

   或

   要以圖表格式查看多個項目、方案或產品組合的利用率報告，請按一下 **報表** 前往「報表」區域，然後按一下 **利用率** 標籤。

1. 在「利用率」報告的右上角，按一下 **圖表** 表徵圖。\
   ![](assets/utilization-chart.png)\
   「利用率」報告將以圖表視圖顯示。

1. （選用）選取適當的選項，將此設定為顯示專案、方案或Portfolio **顯示** 下拉式功能表。
1. （可選）將滑鼠移至報表上的特定時間點，以檢視該時間點的資料。

   ![](assets/utilization-chart-hover-350x176.png)

1. （選用）調整篩選條件，以決定圖表中顯示的資訊。 如需調整篩選器的相關資訊，請參閱區段 [篩選利用資訊](#filter-utilization-information) 這篇文章。
1. （選用）設定圖表報表的時間範圍，如 [調整顯示資訊的日期範圍](#adjust-the-date-range-for-which-information-is-displayed) 這篇文章。
