---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 方案計畫器中的方案概覽
description: 方案規劃器僅適用於新的Adobe Workfront體驗，需要額外的許可。 有關Workfront方案計畫員的資訊，請參閱：方案計畫員概覽
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# 計畫概覽 [!DNL Scenario Planner]

此 [!DNL Scenario Planner] 只能在新 [!DNL Adobe Workfront] 體驗，且需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 [此 [!DNL Scenario Planner] 概述](../scenario-planner/scenario-planner-overview.md).
身為業務經理，您可以在 [!DNL Adobe Workfront Scenario Planner]. 有關建立計畫的資訊，請參閱文章 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## 計畫概覽

使用 [!DNL Workfront Scenario Planner]，您可以估計並檢閱每個計畫的下列資訊：

* 估計完成該計畫可能需要的職務類型和數量。 這將增加計畫的「必需」職務職責計數，並計算您可以複核計畫的人員成本。
* 估計與完成計畫所需的工作相關的固定成本。
* 估計計畫完成時您公司可能獲得的計畫福利。

要查看有關計畫的資訊，您可以訪問計畫內的各個計畫。 有關建立和訪問計畫的資訊，請參閱文章 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## 有關計畫的考慮事項

建立計畫時，請考慮以下事項：

* 您必須先建立計畫，然後才能建立計畫。
* 您可以從頭建立方案，也可以將項目導入計畫中。 這些項目成為計畫內的倡議。

   有關從頭建立計畫的資訊，請參見 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   有關將項目導入計畫以從項目建立方案的資訊，請參閱 [將專案匯入至 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 方案是比計畫小的規劃單位，它們僅作為計畫的一部分建立。
* 最短的倡議可以有1個月的期限。 最長的計畫可以有5年的時間。
* 你不能在計畫上做實際工作。 在計畫層，您可以定義需要哪些資源以及這些資源將產生哪些成本，以便您可以開始執行計畫的其中一項需求。 例如，如果貴公司計畫在新位置擴展和收購新辦事處，則貴部門可能計畫為該新位置安裝網路基礎架構。
* 您可以在計畫中建立多個方案。 通過每個計畫，您可以概述完成部門工作的高級策略。
* 您可以在計畫內排定計畫的優先順序，以確保最重要的計畫獲得最多的預算和最多資源。
* 當您在計畫內建立方案時，查看該計畫的每個人也可以查看該計畫內的所有方案。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* 您可以發佈活動以建立項目或更新連結到它們的項目。 如需發佈活動的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## 有關計畫的財務資訊

您可以查看有關各個計畫的財務資訊，以了解計畫中的計畫如何適應。 有關訪問計畫的資訊，請參閱文章 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

您可以通過在計畫內訪問計畫來查看有關計畫的以下財務指標：

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL成本合計金額]</td> 
   <td> <p style="font-weight: normal;">這是計算計畫總費用的方法。 </p> <p style="font-weight: normal;">[!DNL Workfront] 使用以下公式計算方案的總成本值：</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL固定成本]</td> 
   <td> <p><span style="font-weight: normal;">這是手動輸入，您可在其中估計 <span>計畫每月的固定成本金額。</span> 這不包括與在[!UICONTROL人員成本]欄位中捕獲的添加到計畫的角色相關的成本。</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL人員成本]</td> 
   <td> <p style="font-weight: normal;">這是在計畫期間與計畫的工作角色相關的費用的總計計算。 此數取決於您為計畫每個月的工作職責估計的FTE或小時數。 </p> 
     <p><b>提示</b>  
     <ul> 
      <li> <p>相同職務角色的每月FTE數量可能會因月而異。</p> </li> 
      <li> <p>[!DNL Workfront] 認為一個月內有160個工作小時。 </p> </li> 
     </ul> 
     <p>[!DNL Workfront] 使用以下公式計算計畫的[!UICONTROL人員成本]:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] 使用以下公式計算方案期間每個月的每月人員成本：</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>範例</b></p>
      <p>如果您的計畫持續時間為6個月，需要1個每月1名FTE的每小時費率為$50的Designer，以及計畫期間2個月的每小時費率為$100的Web設計器，則計畫的人員成本計算如下：</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL計畫福利]</td> 
   <td>這是一個手動輸入項，您可以在其中估計完成此計畫後，您的部門將獲得的總體收益。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL淨值金額]</td> 
   <td> <p style="font-weight: normal;">這表示您的計畫在考慮總體成本和根據計畫估計的計畫效益時的價值。 [!DNL Workfront] 使用以下公式計算方案的淨值：</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

## 報告中的倡議資訊

您可以在報表中顯示方案資訊，如下表所述。 只有在貴公司已購買Workfront方案規劃程式授權時，您的Workfront例項才能取得此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>報表類型</b></td> 
   <td><b>計畫資訊</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫] </td> 
   <td>名稱、持續時間、開始和結束日期、輸入者、ID、上次發佈日期*、所有專案欄位，包括自訂欄位*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫作業角色]</td> 
   <td>上面列出的所有計畫資訊，（職務職責）ID，項目*，項目分配計畫小時數*，計畫職務職責小時數，（職務職責）計數，包括自定義欄位的所有項目欄位*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL項目]*</p></td> 
   <td> <p>上面列出的所有計畫資訊*</p> </td> 
  </tr> 
 </tbody> 
</table>

*這些欄位填入連結至計畫的項目中的資訊，只有當計畫是從項目建立的，或已至少發佈到項目一次時。 如需發佈活動的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
