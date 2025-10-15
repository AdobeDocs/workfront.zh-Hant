---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 情境規劃工具中的方案概觀
description: Scenario Planner僅在新的Adobe Workfront體驗中可用，並且需要額外的授權。 如需「Workfront案例規劃工具」的相關資訊，請參閱「案例規劃工具」概觀。
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# [!DNL Scenario Planner]中的方案總覽

身為業務經理，您可以在[!DNL Adobe Workfront Scenario Planner]中建立計畫的方案。 如需有關建立計畫的資訊，請參閱文章[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中建立和編輯計畫。

## 行動方案概觀

您可以使用[!DNL Workfront Scenario Planner]來預估及檢閱每個方案的下列資訊：

* 預估完成方案所需的工作角色型別和數量。 這會新增至計畫的「必要」職務角色計數，並計算您可複查方案的「人員成本」。
* 預估與完成方案所需的工作相關的固定成本。
* 預估當方案完成時貴公司可能獲得的計畫收益。

若要檢視關於方案的資訊，您可以存取計畫內的個別方案。 如需有關建立和存取方案的資訊，請參閱文章[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。

## 關於方案的考量事項

建立行動方案時，請考量下列事項：

* 在建立方案之前，您必須先建立計畫。
* 您可以從頭開始建立方案，也可以將專案匯入計畫。 專案會成為計畫內的方案。

  如需從頭開始建立方案的詳細資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。

  如需有關將專案匯入計畫以從專案建立方案的資訊，請參閱[將專案匯入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中的計畫。

* 方案是比計畫小的規劃單位，而且它們只作為計畫的一部分建立。
* 最短方案的持續時間可為1個月。 最長方案的期限可為5年。
* 您無法在方案上執行實際工作。 在方案層次，您可以定義所需的資源以及這些資源所產生的成本，以便開始執行計畫的需求之一。 例如，如果貴公司有計畫在新地點擴充及收購新辦公室，您的部門可能會主動為該新地點安裝網路基礎結構。
* 您可以在計畫中建立多個方案。 對於每個方案，您都可以概述高階策略來完成部門中的工作。
* 您可以排定計畫內方案的優先順序，以確保最重要的方案獲得最多的預算和最多的資源。
* 當您在計畫內建立方案時，所有檢視該計畫的人員也可以檢視該計畫內的所有方案。
* 您可以發佈方案以建立專案或更新連結至它們的專案。 如需有關發佈方案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈方案以更新或建立專案。

## 方案的相關財務資訊

您可以檢閱個別方案的財務資訊，以瞭解方案如何符合計畫。 如需有關存取行動方案的資訊，請參閱文章[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中建立和編輯行動方案。

您可以在計畫中存取方案，以檢視方案的下列財務指標：

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL成本總金額]</td> 
   <td> <p style="font-weight: normal;">這是行動方案總成本的計算。 </p> <p style="font-weight: normal;">[!DNL Workfront] 使用此公式計算方案的總成本值：</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL固定成本]</td> 
   <td> <p><span style="font-weight: normal;">這是手動專案，您可以估計每個月方案的<span>固定成本金額。</span>這不包括與新增至方案的角色相關的成本，這些角色是擷取在[！UICONTROL人員成本]欄位中。</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL人員成本]</td> 
   <td> <p style="font-weight: normal;">這是方案期間與方案工作角色相關成本的總計。 此數字取決於您為方案每個月的工作角色預估的FTE或時數。 </p> 
     <p><b>提示</b>  
     <ul> 
      <li> <p>相同職務角色的每月FTE數量可能依月份而不同。</p> </li> 
      <li> <p>[!DNL Workfront] 認為一個月有160個工作小時。 </p> </li> 
     </ul> 
     <p>[!DNL Workfront] 使用下列公式計算方案的[！UICONTROL人員成本]：</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront]使用下列公式計算方案期間每個月的每月人員成本：</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>範例</b></p>
      <p>如果您的行動方案為期6個月，且每個月需要1個Designer （含1個FTE的$50小時費率）以及2個月的Web Designer （含$100小時費率），則行動方案的「人員成本」計算如下：</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL計畫權益]</td> 
   <td>這是一個手動輸入專案，您可以在此專案中估計部門完成此方案將獲得的整體收益。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL淨值金額]</td> 
   <td> <p style="font-weight: normal;">這代表在考慮整體成本以及計畫上預估的計畫收益時，您計畫的價值。 [!DNL Workfront]使用下列公式計算方案的淨值：</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## 報告中的方案資訊

您可以在報表中顯示方案資訊，如下表所述。 只有當貴公司已購買Workfront Scenario Planner授權時，才能在您的Workfront執行個體中取得此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>報告型別</b></td> 
   <td><b>方案資訊</b></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL方案] </td> 
   <td>名稱、持續時間、開始和結束日期、輸入者、ID、上次發佈日期*、所有專案欄位，包括自訂欄位*</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL方案工作角色]</td> 
   <td>如上列出的所有方案資訊，（工作角色） ID，專案*，專案指派計畫時數*，方案工作角色時數，（工作角色）計數，所有專案欄位，包括自訂欄位*</td> 
  </tr> 
  <tr> 
   <td><p>[！UICONTROL專案]*</p></td> 
   <td> <p>以上列出的所有方案資訊*</p> </td> 
  </tr> 
 </tbody> 
</table>

*這些欄位會填入連結至方案之專案的資訊，但僅限於方案是從專案建立或是至少發佈至專案一次時。 如需有關發佈方案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈方案以更新或建立專案。
