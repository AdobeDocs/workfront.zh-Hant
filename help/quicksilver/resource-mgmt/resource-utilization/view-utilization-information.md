---
product-area: resource-management
navigation-topic: resource-utilization
title: 檢視資源使用率資訊
description: 您可以使用「使用率」報表來檢視資源的使用率。
author: Alina, Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '7854'
ht-degree: 0%

---

# 檢視資源使用率資訊

{{highlighted-preview}}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

您可以使用「使用率」報表來檢視資源的使用率。

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

您必須具備下列條件才能存取「使用率」報表：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視以下專案或更高存取權：</p> 
    <ul> 
     <li> <p>資源管理 </p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>專案組合</p> </li> 
     <li> <p>計劃</p> </li> 
     <li> <p>財務資料（如果您要依成本檢視資訊）</p> </li> 
    </ul> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視對專案、專案組合和方案的存取權，以存取資源區域中的「使用率」區段</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>管理專案的存取權以存取專案的「使用率」區段</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡Workfront管理員。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

以下各節說明如何檢視和使用使用率資訊。

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

## 使用率報表概要 {#overview-of-the-utilization-report}

您可以使用「使用率」報表，在單一報表中檢視專案、方案或投資組合的進度、成本或收入。 您也可以比較收入與成本。

您可以在「資源配置」區域中檢視「使用率」報表，以顯示多個專案的使用率，或者您可以在一個專案層次中檢視該報表，以顯示與該專案相關聯的個別資源（職務角色和使用者）的使用率。

如需有關存取及使用「使用率」報告的資訊，請參閱 [使用使用情況報告追蹤進度、成本和收入](#track-progress-cost-and-revenue-with-the-utilization-report) 章節。

* [追蹤小時（進度）](#track-hours-progress)
* [追蹤成本](#track-cost)
* [追蹤收入](#track-revenue)
* [比較收入與計畫成本與實際成本](#compare-revenue-against-planned-and-actual-costs)

### 追蹤小時（進度） {#track-hours-progress}

您可以透過檢視預算和計畫時數與實際時數的比較來追蹤進度。

在追蹤專案、方案或投資組合的進度時，針對任務和問題的進度會包含在使用率報告中。

追蹤時數時，「使用率」報表中會顯示下列資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>檢視時數時的欄標題</strong> </th> 
   <th><strong>函數</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>預算時數</strong> </td> 
   <td scope="col"> <p>已包含專案的總預算時數。 您可以檢視所包含專案整個生命週期的總預算時數，或僅檢視指定日期範圍內的總預算時數（您可以指定個別周或月）。 </p> <p>預算時數會從業務案例或資源規劃工具之新資源預算區域中的可用資訊植入<em>.</em></p> <p>預算時數會顯示在「使用率」報表的下列任一列中：</p> 
    <ul> 
     <li> 預算時數在「使用率」報表中依職務角色和個別使用者進行彙總，如下所示：<br><strong>個別使用者：</strong> 已在使用率報告中摘要每個使用者的預算時數。 這些預算時數與使用者在包含的專案中受指派的任務和問題相關聯。 （您可以展開對應工作角色的列，以檢視具有該工作角色的使用者清單。）<br><strong>工作角色：</strong> 已編列預算時數會依使用率報表中的工作角色進行彙總。<br>預算時數會因下列任一情況而出現在特定工作角色中： 
     <li>工作角色定義為指派給與預算時數相關聯之任務或問題的使用者的主要工作角色。 </li> 
       <li>當您檢視單一專案的使用率資訊時，無論任務或問題中沒有指派、指派另一個使用者沒有工作角色指派、指派另一個使用者有不同的工作角色或指派另一個團隊，都會使用指派了時數的使用者工作角色。</li> 
       <li>當您檢視數個專案、方案或投資組合的利用資訊時，僅當針對專案中的任務或問題指派角色時，才會使用指派了時數的使用者工作角色。 </li> 
       <li>工作角色已指派給與預算時數相關聯的任務或問題，而指派給任務或問題的使用者沒有在系統中定義的工作角色。</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>未配置時數</strong>：當預算時數與任務或問題相關聯，且沒有使用者或角色指派給任務或問題時，預算時數會顯示在未分配時數區段的使用率報告中。<br>僅當專案上有符合此說明的小時數，以及按專案或從專案檢視使用情況報告時，才會顯示此區段。 </p> <p>僅當專案上有符合此說明的小時數，以及按專案或從專案檢視使用情況報告時，才會顯示此區段。 </p> </li> 
    </ul> <p>如需預算時數的詳細資訊，請參閱 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">瞭解專案的預算勞力成本和預算時數</a> 文章。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫小時</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
與每個任務和問題的工作分派相關聯的已包含專案上的計畫時數。 您可以檢視專案上所有工作分派在包含專案之整個生命週期中的總計畫時數，或者只能檢視指定日期範圍內的總計畫時數（您可以指定個別周或月）。 
</p>
<p>
<strong>秘訣 </strong>
</p>
<p>
持續期間為0的專案中的計畫時數未考慮在內。 
</p>
<p>
「使用率」報表中的計畫時數會考慮計畫時數是否已重新分配至任務或問題的整個期間。 
</p>
<p>
當使用工作負載平衡器修改使用者每日的時數分配時，如果利用率報告中選擇的日期僅包含任務或問題的持續時間的一部分，則利用率報告中的資料可能會受到影響。 
</p>
<p>
如需修改使用者配置的相關資訊，請參閱 <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">在工作負載平衡器中管理使用者配置</a>.


</p>
<p>
「計畫時數」會顯示在「使用率」報表的下列任一列中：
</p>
<ul>

<li>計畫時數會依職務角色和使用率報表中的個別使用者進行彙總，如下所示： 
<ul>

<li><strong>個人使用者</strong>：使用率報告中會摘要列出每個使用者的計畫時數。 這些計畫時數與使用者在包含的專案中受指派的任務和問題相關聯。 （您可以展開對應工作角色的列，以檢視具有該工作角色的使用者清單。）

<li><strong>工作角色</strong>：計畫時數依單一專案之使用報告中的工作角色摘要。<br>計畫時數會因下列任一情況而出現在特定工作角色中：  
<ul>

<li>工作角色定義為指派給與計畫時數相關聯之任務或問題的使用者的主要工作角色。

<li>當您檢視單一專案的使用率資訊時，與工作角色相關聯的時數不會針對下列案例中的工作角色顯示：   
<ul>

<li>任務或問題上沒有指派

<li>使用者指派時沒有工作角色指派

<li>使用者被指派了不同的工作角色

<li>已將團隊指派給任務或問題
</li>   
</ul>

<li>當您檢視數個專案、方案或投資組合的利用資訊時，僅當針對專案中的任務或問題指派角色時，才會使用指派了時數的使用者工作角色。 檢視多個專案的「使用率」報告時，工作角色時數不會個別顯示。

<li>工作角色被指派給與計畫時數相關聯的任務或問題，而指派給任務或問題的使用者沒有在系統中定義的工作角色。
</li>  
</ul>

<li><strong>未配置時數</strong>：當計畫時數與任務或問題相關聯且未指派任何使用者或角色給任務或問題時，計畫時數會顯示在使用率報表中的「未分配時數」區段中。僅當專案上存在符合此說明的時數時，以及檢視單一專案的「使用率」報表時，才會顯示此區段。 <br>如需計畫時數的詳細資訊，請參閱 <a href="../../manage-work/tasks/task-information/planned-hours.md">計畫時數概觀</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>實際工作</strong> </td> 
   <td> <p> 記錄任務、問題和 <span>在專案上和</span> 針對包含的專案。 您可以檢視所包含專案整個生命週期的實際總時數，也可以僅檢視指定日期範圍內的實際總時數（您可以指定個別周或月）。 </p> <p>警告：使用率報表包含記錄至專案的時數、子系任務、問題和至少有一個指派的上層任務。 它不包括記錄到沒有指派的上層任務的時數。 我們建議您不要將父系任務用作工作任務，而只將子系任務指派給您的資源。 </p> <p>實際時數會顯示在使用率報表的下列任一列中：</p> 
    <ul> 
     <li> 實際時數在專案的使用率報表中依職務角色和個別使用者進行彙總，如下所示：<br><strong>個別使用者：</strong> 實際時數會顯示在使用率報告中記錄時數之使用者的列中的位置。 （您可以展開對應工作角色的列，以檢視具有該工作角色且已記錄時數的使用者清單。）<br><strong>工作角色：</strong> 與這些角色相關聯的使用者所記錄的實際時數，會摘要至對應工作角色列中的使用率報告。<br>由於下列任何情況，實際時數會出現在特定工作角色中： 
      <ul> 
       <li>工作角色定義為記錄時數之使用者的主要工作角色。</li> 
       <li>任務或問題上沒有指派</li> 
       <li>已指派另一位使用者，但未指派任何工作角色</li> 
       <li>另一個使用者被指派了不同的工作角色</li> 
       <li> <p>已指派團隊。</p> </li> 
      </ul></li>  
     <p>如果記錄時數的使用者沒有與其設定檔關聯的工作角色，則用於使用情況報告的工作角色是指派給記錄時數的任務或問題的工作角色，或與任務或問題的主要擁有者關聯的工作角色。 </p> 
     <li><strong>其他時數：</strong> 實際時數會顯示在使用率報表的「其他時數」區段中，位於記錄時數之使用者的列中。<br>當記錄時數的使用者沒有在系統中定義工作角色時，時數會顯示在此區段中。<br>僅當專案上有符合此說明的小時時，才會顯示此區段。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>預算差額（以小時計）</strong> </td> 
   <td> <p>總預算時數減去所包含專案的總實際時數。 您可以檢視所包含專案整個生命週期的預算差異總計，或僅檢視指定日期範圍的預算差異總計（您可以指定個別周或月）。 </p> <p>如果值為正數，則會以綠色顯示。 這表示總預算時數大於實際時數。</p> <p>如果值為負數，則會以紅色顯示。 這表示總預算時數小於實際時數。</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>計畫差異（小時）</strong> </td> 
   <td> <p>總計畫時數減去所包含專案的總實際時數。 您可以檢視所包含專案整個生命週期的計畫差異總計，或僅檢視指定日期範圍的計畫差異總計（您可以指定個別周或月）。</p> <p>如果值為正數，則會以綠色顯示。 這表示總計畫時數大於實際時數。</p> <p>如果值為負數，則會以紅色顯示。 這表示總計畫時數小於實際時數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 追蹤成本 {#track-cost}

您可以檢視預算成本與計畫成本與實際成本的比較結果，以追蹤成本。

追蹤專案、方案或投資組合的成本時，「使用率」報表中的資訊來自任務。 作業的成本資訊一律可在「使用率」報表中取得。 根據任務的成本型別計算任務成本。 如需有關作業成本型別的資訊，請參閱下列的「修改個別作業的成本型別」： [追蹤成本](../../manage-work/projects/project-finances/track-costs.md).

您可以透過下列方式在「使用率」報表中顯示成本資訊：

* 針對指定的周或月，或針對整個專案、方案或投資組合。
* 依角色或個人，專案。

使用率報表中使用的幣別是由專案上設定的幣別所決定。 如需有關如何調整專案貨幣的資訊，請參閱 [變更專案貨幣](../../manage-work/projects/project-finances/change-project-currency.md).

追蹤「成本」時，「使用率」報表中會提供下列資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>檢視成本時的欄標題</strong> </th> 
   <th> <p><strong>函數</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>預算成本</strong> </td> 
   <td scope="col"> <p>包含的專案上的預算成本。 您可以檢視包含專案之整個生命週期的總預算成本，或僅檢視指定日期範圍的總預算成本（您可以指定個別周或月）。</p> <p>由於使用率報表中的預算成本主要是依角色區分的成本，因此計算方式與Workfront其他區域中的預算勞力成本相同。 如需如何計算預算勞力成本的資訊，請參閱 <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">瞭解專案的預算勞力成本和預算時數</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫成本</strong> </td> 
   <td scope="col"> <p>包含的專案上的總計畫成本。 您可以檢視所包含專案整個生命週期的計畫成本總計，或僅檢視指定日期範圍的計畫成本總計（您可以指定個別周或月）。</p> <p><span class="preview">請注意，對於周、月和季度檢視，當職位角色或使用者的成本費率生效日期時，計畫成本計算為所選期間的平均值。</span></p><p>如需專案計畫成本計算方式的詳細資訊，請參閱本文章的「Workfront如何計算計畫、預算與實際成本」一節 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>實際成本</strong> </td> 
   <td scope="col"> <p>包含專案的總實際成本。 您可以檢視所包含專案整個生命週期的實際成本總計，或僅檢視指定日期範圍的實際成本總計（您可以指定個別周或月）。</p> <p>如需有關如何計算專案實際成本的資訊，請參閱文章中的「Workfront如何計算計畫、預算與實際成本」一節 <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>預算差額（成本）</strong> </td> 
   <td scope="col"> <p>總預算成本減去所包含專案的總實際成本。 您可以檢視所包含專案整個生命週期的預算差異總計，或僅檢視指定日期範圍的預算差異總計（您可以指定個別周或月）。</p> <p>如果值為正數，則會以綠色顯示。 這表示總預算成本大於實際成本。</p> <p>如果值為負數，則會以紅色顯示。 這表示總預算成本小於實際成本。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>計畫差異（成本）</strong> </td> 
   <td> <p>總計畫成本減去所包含專案的總實際成本。 您可以檢視所包含專案整個生命週期的計畫差異總計，或僅檢視指定日期範圍的計畫差異總計（您可以指定個別周或月）。 </p> <p>如果值為正數，則會以綠色顯示。 這表示總計畫成本大於實際成本。</p> <p>如果值為負數，則會以紅色顯示。 這表示總計畫成本小於實際成本。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 追蹤收入 {#track-revenue}

您可以透過檢視預算和計畫收入與實際收入的比較來追蹤收入。

追蹤專案、方案或投資組合的收入時，「使用率」報表中只會包含來自任務的收入。

追蹤「收入」時，「使用率」報表中會提供下表中的資訊。

如需特定欄位以及Workfront如何計算欄位的資訊，另請參閱下列文章：

* [追蹤成本](../../manage-work/projects/project-finances/track-costs.md)
* [帳單與收入概要](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

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
   <td scope="col"> <p>總預算時數乘以所包含專案中的角色收費率。 您可以檢視所包含專案整個生命週期的預算收入總計，或僅檢視指定日期範圍的預算收入總計（您可以指定個別周或月）。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫收入</strong> </td> 
   <td scope="col"> <p>「使用率」報表中的計畫收入是指與「計畫時數」相關聯的收入，此計畫時數會配置給指派給專案上任務的資源。</p> <p>Workfront會使用下列公式計算「使用率」報表的專案計畫收入：</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>附註</b>
   <p>「使用率」報表中顯示的專案計畫收入，與「專案詳細資訊」區域及專案報表中顯示的計畫收入不同。 </p> <p>專案詳細資訊區域中的計畫收入反映任務收入以及專案的固定收入。 使用率報表中的計畫收入僅顯示與專案中的任務相關的計畫收入。 </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>如果專案有1個時數為10小時的任務，指派給顧問時費率為$20，而專案有$100的固定收入，則使用率報表會顯示計畫收入$200 （與任務時數相關的計畫收入）。 專案詳細資訊區段顯示$300 （任務的計畫收入與專案的固定收入）。 </p> 
     </div> <p>如需「使用率」報表以外之任務與專案計畫收入的詳細資訊，請參閱 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>.</p> </p> <p>「使用率」報表計算與顯示所包含專案之「計畫收入」的方式，會考慮在任務上設定的「收入型別」。 </p> <p>根據專案中每個任務的「收入型態」，會有下列案例： </p> <p><strong>固定收入：</strong> 無論任務指派為何，都會使用任務上指定的「固定金額」來計算任務上的收入。</p> <p><b>重要</b>

與Workfront的其他區域不同，「使用率」報表會平均除以「固定收入」與任務的計畫時數，以計算「固定收入」任務的計畫收入。 </p> <p>例如，任務的收入為$200。 如果任務中有4個計畫時數，則每小時將為$50。 這會分散在使用者與角色層級。 此分佈是利用率報表所獨有的。</p> <p><b>附註</b>

如果您有「固定收入」任務，而且該任務沒有「計畫時數」，則「收入」不會顯示在「使用率報表」中，因為沒有辦法將其分配至時數。 如果您有固定收入且無指派之任務的計畫時數，則收入會顯示為未配置收入。 </p> <p><strong>角色小時：</strong> 使用為特定角色設定的收費率乘以該角色相關聯的計畫時數，即可計算任務的收入。 Workfront會使用以下公式：</p> <p><code>角色每小時計畫收入= SUM（所有任務上角色的計畫時數） *角色記帳費率</code></p><p><span class="preview"><b>注意：</b> 公式中的帳單小時費率會考量費率的任何日期有效變更。</span></p>   <p><strong>使用者小時：</strong> 任務的收入是使用為特定使用者設定的收費率，乘以該使用者相關聯的計畫時數來計算。 Workfront會使用以下公式：</p> <p><code>使用者小時計畫收入= SUM（所有任務中使用者的計畫時數） *使用者收費率</code> </p> <p><span class="preview"><b>注意：</b> 公式中的帳單小時費率會考量費率的任何日期有效變更。</span></p> <p><b>角色小時或使用者小時加固定</b> </p> <p><b>重要</b>

與Workfront的其他區域不同，「使用率」報表會使用「固定收入」除以任務上的「計畫時數」來計算「計畫收入」。 </p> <p>存在下列案例： </p>
<ul>
<li> <p><strong>角色小時加固定：</strong> 任務的收入是使用為特定角色設定的收費率，乘以與角色相關聯的計畫時數來計算。 此外，在任務上指定的固定數量會新增到角色比率。 Workfront會使用以下公式：</p> <p><code>角色小時加固定計畫收入= [SUM（所有任務上角色的計畫時數） *角色收費率] + SUM（任務的上限或固定數量/任務的計畫時數）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>使用者小時加固定：</strong> 為特定使用者設定的計費率，乘以該使用者在該任務上的計畫時數。 此外，在任務上指定的固定數量會新增到使用者比率。 Workfront會使用以下公式：</p> <p><code>使用者小時加固定計畫收入= [SUM（使用者在所有任務上的計畫時數） *使用者收費率] + SUM（任務的上限或固定數量/任務的計畫時數）</code> </p> </li>
</ul> <p><b>受限角色或使用者小時</b> </p> <p><b>重要</b>

與Workfront的其他區域不同，如果計畫收入超過上限，超過上限金額的金額會被視為固定收入。 「計畫收入」的計算方式為將「固定收入」平均除以任務上的「計畫時數」數目，然後加上上限金額與角色或使用者每小時收入。 <br></p> <p>存在下列案例： </p>
<ul>
<li> <p><strong>受限角色小時：</strong> 任務會依照角色每小時的計費方式每小時計費，但是它們有您可以指定的上限金額。 Workfront會使用以下公式：</p> <p><code>具有計畫收入上限的角色小時= [SUM（所有任務和問題的角色計畫時數） *角色收費率] +任務的上限金額+ SUM（超過任務上限金額/計畫時數的金額）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>受限使用者小時：</strong> 任務會以每小時的使用者小時計費，但具有您可指定的上限金額。 Workfront會使用以下公式： </p> <p><code>計畫收入上限的使用者小時= [SUM（使用者在所有任務上的計畫時數） *使用者收費率] +任務的上限金額+ SUM（超過任務上限金額/計畫時數的金額）</code> </p> </li>
</ul> <p>如需有關計算計畫收入時考慮哪個角色或使用者的詳細資訊，請參閱 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>實際收入</strong> </td> 
   <td> <p>實際收入是與任務的實際時數相關聯的收入 <span>和專案</span>. 如需實際收入的詳細資訊，請參閱文章中的「追蹤收入金額」一節 <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>.</p>

<p>「使用率」報表計算所包含專案之實際收入的方式會根據作業上設定的「收入型態」而有所不同，如下所示：</p> <p><strong>固定收入：</strong> 無論任務指派為何，都會使用任務上指定的「固定金額」來計算任務上的收入。</p> <p><b>重要</b>

與Workfront的其他區域不同，「使用率」報表會計算「實際收入」，方法是將「固定收入」平均除以任務上記錄的時數。 </p> <p> </p> <p>例如，任務的實際收入為$200。 如果任務有4個實際小時，則每個小時將為$50。 這會分散在使用者與角色層級。 此分佈是利用率報表所獨有的。</p> <p><b>附註</b>

如果您有「固定收入」作業，而且該作業沒有「實際時數」，則「實際收入」不會顯示在「使用率報表」中，因為沒有分配時數的方式。 </p> <p><strong>角色小時：</strong> 作業上的收入是使用為特定角色設定的收費率，乘以實際時數來計算。</p> <p>Workfront會使用以下公式：</p> <p><code>角色每小時實際收入= SUM（所有任務上角色的實際時數） *角色記帳費率</code> </p> <p><span class="preview"><b>注意：</b> 公式中的帳單小時費率會考量費率的任何日期有效變更。</span></p> <p><strong>使用者小時：</strong> 作業上的收入是使用為特定使用者設定的收費率乘以該使用者的作業記錄時數而計算的。 Workfront會使用以下公式：</p> <p><code>使用者小時實際收入= SUM（使用者在所有任務上的實際小時） *使用者記帳費率</code></p> <p><span class="preview"><b>注意：</b> 公式中的帳單小時費率會考量費率的任何日期有效變更。</span></p> <p><b>角色或使用者小時加固定</b> </p> <p><b>重要</b>

與Workfront的其他區域不同，「使用率」報表會計算「實際收入」，方法是將「固定收入」平均除以任務上記錄的時數。 </p> <p>存在下列案例： </p>
<ul>
<li> <p><strong>角色小時加固定：</strong> 為特定角色設定的計費率，乘以從該角色的使用者記錄的作業時數。 此外，在任務上指定的固定數量會新增到角色比率。 </p> <p>Workfront會使用以下公式：</p> <p><code>角色小時加固定實際收入= [SUM（所有任務上角色的實際時數） *角色記帳費率] + SUM（任務的上限或固定金額/任務的實際時數）</code> </p> </li>
</ul>
<ul>
<li> <p><strong>使用者小時加固定：</strong> 為特定使用者設定的計費率，乘以該使用者針對該任務記錄的時數。 此外，在任務上指定的固定數量會新增到使用者比率。 </p> <p>Workfront會使用以下公式：</p> <p><code>使用者小時加固定實際收入= [SUM（所有任務上角色的實際時數） *使用者收費率] + SUM（任務的上限或固定數量/任務的使用者時數）</code> </p> </li>
</ul> <p><b>受限角色或使用者小時</b> </p> <p><b>重要</b>

與Workfront的其他區域不同，如果計畫收入超過上限，超過上限金額的金額會被視為固定收入。 「計畫收入」的計算方式為將「固定收入」平均除以任務上的「計畫時數」數目，然後加上上限金額與角色或使用者每小時收入。 <br></p> <p>存在下列情況：</p>
<ul>
<li> <p><strong>受限角色小時：</strong> 任務會依照角色每小時的計費方式每小時計費，但是它們有您可以指定的上限金額。 Workfront會使用以下公式：</p> <p><code>角色小時，具有實際收入上限= [SUM（角色在所有任務和問題上的實際時數） *角色收費率] +任務的上限金額+ SUM（超過上限金額的金額/任務的實際時數）</code></p> </li>
</ul>
<ul>
<li> <p><strong>受限使用者小時：</strong> 任務會以每小時的使用者小時計費，但具有您可指定的上限金額。</p> <p> Workfront會使用以下公式：</p> <p><code>具有實際收入上限的使用者小時= [SUM（角色中所有任務和問題的實際時數） *使用者收費率] +任務的上限金額+ SUM（超過上限金額的金額/任務的實際時數）</code> </p> </li>
</ul>
<div>
<p><strong>專案收入</strong>：計算與專案上記錄時數相關聯的收入，會考慮記錄時間之使用者的主要工作角色的每小時計費金額。 我們不建議在此專案上記錄時間。 </p>
<p><b>附註</b>

如果使用者未與工作角色相關聯，或如果主要角色的每小時計費為零，則Workfront會使用使用者的每小時計費金額來計算實際收入。 如果使用者在其設定檔中沒有每小時計費金額，則實際收入為零。 </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>預算差額（用於收入）</strong> </td> 
   <td> <p>包含專案的總實際收入減去預算收入。<br>您可以檢視所包含專案整個生命週期的預算差異總計，或僅檢視指定日期範圍的預算差異總計（您可以指定個別周或月）。</p> <p>如果值為正數，則會以綠色顯示。 這表示總預算收入大於實際收入。</p> <p>如果值為負數，則會以紅色顯示。 這表示總預算收入小於實際收入。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>計畫差異（針對收入）</strong> </td> 
   <td> <p>總實際收入減去所包含專案的總計畫收入。<br>您可以檢視所包含專案整個生命週期的計畫差異總計，或僅檢視指定日期範圍的計畫差異總計（您可以指定個別周或月）。 </p> <p>如果值為正數，則會以綠色顯示。 這表示總計畫收入大於實際收入。</p> <p>如果值為負數，則會以紅色顯示。 這表示總計畫收入小於實際收入。</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### 比較收入與計畫成本與實際成本 {#compare-revenue-against-planned-and-actual-costs}

您可以連同計畫收入檢視計畫或實際成本。 也會顯示利潤(%) （利潤的計算方式為收入 — 成本/收入）。

比較「收入」與「計畫成本」與「實際成本」時，「使用率」報表中會提供下列資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>檢視收入vs成本時的欄標題（計畫）</strong> </th> 
   <th> <strong>函數</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>計畫成本</strong> </td> 
   <td scope="col"> 包含的專案上的總計畫成本。 您可以檢視所包含專案整個生命週期的計畫成本總計，或僅檢視指定日期範圍的計畫成本總計（您可以指定個別周或月）。 </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>計畫收入</strong> </td> 
   <td scope="col"> <p>計畫收入是與任務的計畫時數相關聯的收入。 </p> <p>「使用率」報表計算與顯示內含專案之計畫收入的方式，會因作業上設定的「收入型態」而有所不同，如 <a href="#track-revenue" class="MCXref xref">追蹤收入</a> 章節。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>邊界</strong> </td> 
   <td scope="col"> <p>「利潤」百分比的計算方式如下：</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>附註</b>

如果「計畫收入」等於0，則「利潤」會顯示為0。 </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>檢視收入vs成本時的欄標題（實際）</strong> </p>  </td> 
   <td scope="col"><p><strong>函數</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>實際成本</strong> </td> 
   <td scope="col"> <p>包含專案的總實際成本。 您可以檢視所包含專案整個生命週期的實際成本總計，或僅檢視指定日期範圍的實際成本總計（您可以指定個別周或月）。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>實際收入</strong> </td> 
   <td> <p>實際收入是與任務的實際時數相關聯的收入。</p> <p>僅當任務標籤為「完成」或「完成」（或等同於「完成」的狀態）後，「實際收入」才會顯示在「使用率」報表中。</p> <p>「使用率」報表計算所包含專案之實際收入的方式會根據作業上設定的「收入型態」而有所不同，如 <a href="#track-revenue" class="MCXref xref">追蹤收入</a> 章節。 </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>邊界</strong> </td> 
   <td> <p>「利潤」百分比的計算方式如下：</p> <p>實際收入 — 實際成本/實際收入x 100。 </p> <p><b>附註</b>

如果「實際收入」等於0，則「利潤」會顯示為0。 </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## 使用使用情況報告追蹤進度、成本和收入 {#track-progress-cost-and-revenue-with-the-utilization-report}

您可以追蹤專案、方案或投資組合的進度或成本。

您可以在指定的周或月，或專案整個生命週期的「使用率」報表中顯示資訊。

若要使用「使用率」報表追蹤一或多個專案的進度或成本，請執行下列步驟：

1. 視您檢視的是個別專案、多個專案、方案或投資組合的使用率資訊而定，請執行下列任一作業：

   * 若要檢視單一專案的使用率資訊，請執行下列步驟：

      1. 前往您要檢視使用率資訊的專案，然後按一下 **顯示更多>使用率**.
      1. 檢視個別專案時，使用率資訊會自動顯示，而不需要套用篩選器。\
         如果要篩選「使用率」報表，可以套用篩選器，然後按一下 **執行**.\
         如需如何篩選「使用率」報表的詳細資訊，請參閱區段 [篩選器使用率資訊](#filter-utilization-information) 本文章內容。\
         會顯示個別使用者和角色（使用者會在其相關聯角色中分組）的使用率資訊。

   * 若要檢視多個專案的使用率資訊，請執行下列步驟：

      1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** 在左側面板中。
      1. 將篩選器套用至使用情況報表，然後按一下 **執行**.\
         執行「使用率」報告之前，您必須在篩選器中指定一或多個專案。 如需如何篩選「使用率」報表的詳細資訊，請參閱區段 [篩選器使用率資訊](#filter-utilization-information) 本文章內容。\
         會顯示個別角色和專案的使用率資訊（角色會在其相關聯專案中分組）。

   * 若要檢視方案的使用率資訊，請執行下列步驟：

      1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** ，然後按一下 **顯示**>**計畫**.
      1. 將篩選器套用至使用情況報表，然後按一下 **執行**.\
         執行「使用率」報告之前，您必須在篩選器中指定一或多個程式。 如需如何篩選「使用率」報表的詳細資訊，請參閱區段 [篩選器使用率資訊](#filter-utilization-information) 本文章內容。\
         會顯示個別專案和方案（專案會分組在其相關聯方案內）的使用率資訊。

   * 若要檢視投資組合的使用率資訊，請執行下列步驟：

      1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** ，然後按一下「 」 **顯示**>**Portfolio**.
      1. 將篩選器套用至使用情況報表，然後按一下 **執行**.\
         執行「使用率」報告之前，您必須在篩選器中指定一或多個投資組合。 如需如何篩選「使用率」報表的詳細資訊，請參閱區段 [篩選器使用率資訊](#filter-utilization-information) 本文章內容。\
         會顯示個別專案、方案和投資組合的使用率資訊（專案會分組在其相關聯方案內，而方案會分組在其相關聯投資組合內）。

1. 在「使用率」報表的右上角，按一下 **檢視** 下拉式功能表，然後從下列專案選取：

   * **成本**
   * **時數**
   * **收入**
   * **收入 vs. 成本 (計畫)**
   * **收入vs成本（實際）**.

   您選取的選項決定報告中可用的欄和資訊。 如需各欄可用資訊的詳細資訊，請參閱步驟5中的表格。\
   ![](assets/utilization-view-dropdown.png)

1. （選擇性）選取要顯示使用率資訊的日期範圍。 您可以在左側顯示指定周或月的資訊 **整體** 欄。 整體專案、方案或投資組合的資訊一律顯示在 **整體** 欄。\
   如需詳細資訊，請參閱區段 [調整顯示資訊的日期範圍](#adjust-the-date-range-for-which-information-is-displayed) 本文章內容。

1. （選擇性）按一下任何欄標題，依該欄中的資訊排序使用率報表。 排序只有在報告中包含多個專案時才有作用。 例如，檢視多個專案（或投資組合或方案）時，您可以對報表結果進行排序。 當您一次只檢視一個專案（或一個投資組合或一個計畫）時，無法排序結果。
1. 使用區段中的資訊 [使用率報表概要](#overview-of-the-utilization-report) 本文章以瞭解使用情況報告中的每個欄。

## 篩選器使用率資訊 {#filter-utilization-information}

您可以篩選在專案的使用情況報告中顯示的內容。 您可以按任務、問題、角色和自訂資料進行篩選。 當您套用篩選條件至「使用率」報表時，「使用率」報表會包含根據您選取之條件的資訊。

您可以建立篩選器，或套用先前建立的篩選器。

* [建立或修改篩選器](#create-or-modify-a-filter)
* [套用儲存的篩選器](#apply-a-saved-filter)
* [複製篩選器](#duplicate-a-filter)
* [重新命名篩選器](#rename-a-filter)
* [刪除篩選器](#delete-a-filter)

### 建立或修改篩選器 {#create-or-modify-a-filter}

建立篩選器時，所有有權存取「使用率」報告的Workfront使用者也都有權存取您建立的篩選器。 同樣地，當您修改現有篩選器時，該篩選器會針對有權存取「使用率」報告的所有使用者進行修改。

若要建立或修改篩選，請執行下列動作：

1. 若要篩選單一專案的使用率資訊，請前往您要篩選其使用率資訊的專案，然後按一下 **顯示更多>使用率** 在左側面板中。

   或

   若要篩選多個專案、方案或投資組合的使用率資訊，請按一下主要功能表圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角， **資源分配**， **使用率** 在左側面板中，然後 **顯示**>**計畫** 或 **Portfolio** 或&#x200B;**專案**.

1. 按一下 **篩選** 圖示來顯示篩選選項。

1. （視條件而定）若要修改現有篩選器，請按一下 **篩選** 下拉式功能表，然後選取您要修改的篩選器。
1. 指定下列資訊以建立或修改篩選器：

   * **Portfolio：** 開始輸入投資組合的名稱，其中包含您要納入使用率報告的資訊，然後按一下顯示在下拉式選單中的名稱。\
     重複此程式，將使用率報告中包含來自多個投資組合的資訊。\
     若要在篩選器中包含您系統中的所有投資組合，請按一下 **全部新增**. （只有在系統中擁有少於10個投資組合時，才可使用此選項。）

   * **程式：** 開始輸入包含您要包含在「使用率」報告中的資訊的方案名稱，然後在其出現在下拉式選單中時按一下名稱。\
     重複此程式，在「使用率」報告中包含多個工作的資訊。\
     如果您已在篩選器中指定任何專案組合，則您指定的計畫必須來自已包含在篩選中的專案組合。 若非如此，則使用率報表中不會包含來自方案的資料。\
     若要將您系統中的所有程式都包含在您的篩選器中，請按一下 **全部新增**. （只有在系統中有少於20個程式時，才可使用此選項。）

   * **專案：** 開始輸入專案名稱，該專案包含您要包含在「使用率」報告中的資訊，然後在其出現在下拉式選單中時按一下名稱。\
     重複此程式，將多個專案的資訊納入使用率報告中。\
     如果您已在篩選器中指定任何投資組合或計畫，則您指定的專案必須來自已包含在篩選中的投資組合或計畫之一。 若非如此，則使用率報告中不會包含來自專案的資料。\
     若要將您系統中的所有專案納入您的篩選中，請按一下 **全部新增**. （只有在系統中擁有少於250個專案時，才可使用此選項。）

   * **任務：** 開始輸入工作名稱，其中包含您要納入使用率報告的資訊，然後按一下顯示在下拉式功能表中的名稱。\
     重複此程式，在「使用率」報告中包含多個工作的資訊。\
     如果您已在篩選器中指定任何投資組合、計畫或專案，則您指定的任務必須來自已包含在篩選中的投資組合、計畫或專案之一。 如果沒有，則來自任務的資料不會包含在使用率報告中。

   * **問題：** 開始輸入問題名稱，該問題包含您要包含在Utilization報告中的資訊，然後在其出現在下拉式選單中時按一下名稱。\
     重複此程式，在使用情況報告中包含多個問題的資訊。\
     如果您已在篩選器中指定任何投資組合、計畫或專案，則您指定的問題必須來自已包含在篩選中的投資組合、計畫或專案之一。 如果沒有，問題的資料不會包含在使用率報告中。\
     問題的成本資訊並不一定包含在使用率報表中。 如需問題的成本資訊何時包含在使用率報表中的詳細資訊，請參閱區段 [使用使用情況報告追蹤進度、成本和收入](#track-progress-cost-and-revenue-with-the-utilization-report) 本文章內容。

   * **角色：** 開始輸入您要在「使用報告」中顯示的角色名稱，然後在名稱出現在下拉式功能表中時按一下該名稱。 重複此程式以包含其他角色。\
     「使用率報表」僅包含您指定之角色的資訊。 例如，一個任務包含10個實際小時。 其中6個小時來自設計師角色，4個小時來自開發人員角色。 如果您依「設計人員」的角色來篩選「使用率報表」，則報表會排除來自開發人員角色的4小時。

   * **新增篩選規則：** 按一下 **新增篩選規則**，在第一個欄位中按一下，然後開始輸入您要篩選的欄位名稱。 如果欄位可用，則會填入可與其產生關聯的每個物件。 按一下欄位名稱，將其新增至篩選器。

     >[!IMPORTANT]
     >
     >您必須輸入欄位名稱，而非欄位標籤。 欄位標籤會顯示在附加到物件的自訂表單上。 如需有關標籤與自訂欄位名稱之間差異的資訊，請參閱  [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

     有關您在欄中看到的欄位的詳細資訊，請參閱 [Adobe Workfront術語表](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     選擇篩選的篩選和條件修飾詞。 可用的修飾元說明如下： [篩選和條件修飾元](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. 若要建立新篩選器，請按一下 **儲存篩選器**.\
   或\
   若要修改現有篩選器，請按一下 **儲存篩選器** 按鈕，然後按一下 **儲存新篩選器**.\
   在 **篩選器名稱** 欄位，指定篩選的名稱，然後按一下 **儲存**.\
   系統會使用您包含在篩選器中的資訊來篩選「使用率」區域。

### 套用儲存的篩選器 {#apply-a-saved-filter}

1. 若要在單一專案的「使用情況報表」上套用篩選，請前往您要篩選的專案，然後按一下 **顯示更多>使用率** 在左側面板中。

   或

   若要針對多個專案、方案或投資組合，在「使用情況報表」上套用篩選器，請按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角， **資源分配**， **使用率** 在左側面板中，然後 **顯示**>**計畫** 或&#x200B;**Portfolio** 或&#x200B;**專案**.

1. 按一下 **儲存的篩選器**，然後從下拉式選單中選取您要套用的篩選器。

### 複製篩選器 {#duplicate-a-filter}

1. 若要在單一專案的「使用情況報表」上複製篩選器，請前往您要複製篩選器的專案，然後按一下 **顯示更多>使用率** 在左側面板中。

   或

   若要針對多個專案、方案或投資組合，在使用情況報告中複製篩選器，請按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** 在左側面板中。

1. 按一下 **儲存的篩選器**，將滑鼠移至下拉式功能表中您要複製的篩選器上，然後按一下 **複製** 圖示。

   ![](assets/utilization-filter-duplicate.png)\
   隨即顯示「複製篩選器」對話方塊。

1. 在 **篩選器名稱** 欄位中，指定新篩選器的名稱，然後按一下 **儲存**.

### 重新命名篩選器 {#rename-a-filter}

當您重新命名篩選器時，所有有權存取「使用率」報表的Workfront使用者都會看到您選擇的新名稱。

若要重新命名篩選器：

1. 若要重新命名單一專案之使用報告上的篩選器，請前往您要重新命名篩選器的專案，然後按一下 **顯示更多>使用率** 在左側面板中。

   或

   若要重新命名多個專案、方案或投資組合的使用情況報告上的篩選器，請按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** 在左側面板中。

1. 按一下 **儲存的篩選器**，將滑鼠移至下拉式功能表中您要複製的篩選器上，然後按一下 **重新命名** 圖示。\
   ![](assets/utilization-filter-rename.png)\
   隨即顯示「重新命名篩選器」對話方塊。

1. 在 **篩選器名稱** 欄位中，指定新篩選器的名稱，然後按一下 **儲存**.

### 刪除篩選器 {#delete-a-filter}

當您刪除篩選器時，所有有權存取「使用率」報告的Workfront使用者皆會刪除該篩選器。

若要刪除篩選器：

1. 若要刪除單一專案之使用報告上的篩選器，請前往您要刪除篩選器的專案，然後按一下 **顯示更多>使用率** 在左側面板中。

   或

   若要針對多個專案、方案或投資組合，在使用情況報表中刪除篩選器，請按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** 在左側面板中。

1. 按一下 **儲存的篩選器**，將滑鼠移至下拉式功能表中您要複製的篩選器上，然後按一下 **刪除** 圖示。

   ![](assets/utilization-filter-delete.png)

1. 按一下 **刪除** 系統提示您是否要刪除篩選器時。

## 調整顯示資訊的日期範圍 {#adjust-the-date-range-for-which-information-is-displayed}

您可以調整顯示使用率資訊的日期範圍。 您可以選取過去或未來的日期。 您所做的變更只會顯示給您。

1. 若要調整單一專案之「使用率報表」的日期範圍，請移至您要調整日期範圍的專案，然後按一下 **顯示更多>使用率** 在左側面板中。

   或

   若要針對多個專案、方案或投資組合，調整使用情況報表的日期範圍，請按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** 在左側面板中。

1. 按一下「 」旁邊的日期範圍 **匯出** 按鈕。

   預設會選取目前的一週。

1. 從下列選項中選取：

   * **周：** 選取此選項可選取指定的一週（從星期日到星期六）。
   * **月：** 選取此選項可選取指定月份。

   您選取的日期範圍會顯示在使用率報表的左側 **整體** 欄。\
   Workfront會記住您是要檢視周或月檢視。 下次您存取使用情況報告時，將會根據您選取的選項顯示當週或當月。

## 匯出使用率資訊

您可以從Workfront匯出專案、方案或投資組合的使用率資訊。 資訊只能以XLSX、TSV和PDF格式匯出。

在Microsoft Excel中檢視時，負數會以括弧顯示。

若要匯出使用率資訊，請執行下列動作：

1. 若要匯出單一專案的使用率資訊，請前往您要匯出使用率資訊的專案，然後按一下 **使用率** 索引標籤(視您的版面設定而定，這可能位於 **更多** 標籤)。

   或

   若要匯出多個專案、方案或投資組合的使用率資訊，請按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **資源分配**，則 **使用率** 在左側面板中。

1. 按一下 **匯出**，位於 **使用率** 標籤。

1. 從下列選項中選取：

   * **PDF：** 以PDF格式匯出報表。 如果您計畫列印報表，建議使用此格式。\
     選取 **信件 — 縱向**， **字母 — 橫向**，或 **其他尺寸** (提供在Legal (8.5&quot; x 14&quot;)、Ledger (11&quot; x 17&quot;)和A4中匯出的選項。\
     視您使用的作業系統而定，您可以選擇開啟或儲存檔案。 使用關聯應用程式開啟檔案，或將其儲存至硬碟。

   * **Excel：** 以XLSX格式匯出報告。 如果您打算進一步分析Excel中的資料，建議使用此格式。\
     視您使用的作業系統而定，您可以選擇開啟或儲存檔案。 使用關聯應用程式開啟檔案，或將其儲存至硬碟。

   * **定位字元分隔：** 以TSV格式匯出報告。 如果您打算將資料匯入協力廠商軟體以供進一步分析，建議您使用此格式。\
     視您使用的作業系統而定，您可以選擇開啟或儲存檔案。 使用關聯應用程式開啟檔案，或將其儲存至硬碟。

1. 閱讀文章中的資訊 [匯出資料](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) 以瞭解如何使用匯出的檔案。

## 在圖表中檢視使用率資訊

您可以在圖表檢視中從「使用率」報告以視覺效果呈現資料。

1. 若要以圖表格式檢視單一專案的「使用率」報告，請移至您要檢視的專案，然後按一下 **顯示更多>使用率** 在左側面板中。

   或

   若要以圖表格式檢視多個專案、方案或投資組合的使用率報告，請按一下 **報告** 在全域導覽列中，前往報表區域，然後按一下 **使用率** 標籤。

1. 在「使用率」報表的右上角，按一下 **圖表** 圖示。\
   ![](assets/utilization-chart.png)\
   「使用率」報告會以圖表檢視顯示。

1. （可選）從中選擇適當的選項，設定此項以顯示專案、方案或Portfolio。 **顯示** 下拉式功能表。
1. （可選）將滑鼠移至報表上的特定時間點上，即可檢視該時間點的資料。

   ![](assets/utilization-chart-hover-350x176.png)

1. （可選）調整篩選器以決定要在圖表中顯示哪些資訊。 如需調整篩選器的詳細資訊，請參閱區段 [篩選器使用率資訊](#filter-utilization-information) 本文章內容。
1. （可選）設定圖表報表的時間範圍，如區段所述 [調整顯示資訊的日期範圍](#adjust-the-date-range-for-which-information-is-displayed) 本文章內容。
