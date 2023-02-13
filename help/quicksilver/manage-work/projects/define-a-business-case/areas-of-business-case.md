---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 業務案例領域概述
description: 本文介紹了項目的業務案例。
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 2%

---

# 業務案例領域概述

本文介紹了項目的業務案例。

有關為項目建立業務案例的資訊，請參閱 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

您的Adobe Workfront管理員或組管理員必須先啟用「業務案例」中的所有部分，才能在項目上顯示這些部分，「項目資訊」部分除外。 預設會啟用「專案資訊」區段。

有關啟用「業務案例」區域的詳細資訊，請參閱  [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

以下是項目「業務案例」中的部分：

* 專案資訊
* 目標
* 費用
* 資源預算
* 風險
* 計分卡
* 自訂表單
* 業務案例摘要

## 專案資訊

此 **專案資訊** 「業務案例」的區域不可由Workfront管理員配置。 在「業務案例」中，所有項目都有「項目資訊」區域。 

「業務案例」的「項目資訊」部分包括項目實際開始之前的基本資訊。

請考慮編輯下列欄位：

* **說明**:指定專案的說明。
* **專案所有者**

   依預設，建立專案的使用者也是專案擁有者。 您可以編輯此欄位，並指定另一個使用中使用者為專案的擁有者。

* **專案贊助者**

   請考慮將項目所有者以外的其他人添加為項目的贊助商。 保薦機構受理《營業案例》批准。 

* **Portfolio**:指定專案的Portfolio。 您必須建立Portfolio，並將其置於 **作用中** 開始供您在此下拉式功能表中選取。

   如需產品組合的詳細資訊，請參閱 [PortfolioAdobe Workfront概觀](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   如需建立Portfolio的詳細資訊，請參閱 [建立產品組合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **計畫福利**:在完成此項目時，估計貴組織的預計貨幣利益。 可以是任何貨幣金額，且必須為正值。 例如10,000美元。
* **狀態**:依預設，專案要求的狀態會設為 **構想**.

   如果您將「狀態」變更為「構想」或「規劃」以外的任何項目，則 **提交** 按鈕從「業務案例摘要」區域消失，您無法再提交「業務案例」以進行批准。 

* **固定開始日期**:指定您要開始專案的日期。
* **固定結束日期**:指定您要結束專案的日期。

   >[!NOTE]
   >
   >業務案例的固定起始日期和終止日期不會影響項目的計畫起始日期和完成日期。 這些日期代表專案建立者要求的專案理想開發日期。 相反，項目的「計劃開始日期」和「計畫完成日期」顯示基於項目任務的項目計畫時間表。

## 目標

目標定義項目的目標。 此區域預設會在「業務案例」中啟用，但Workfront管理員可能會選擇不顯示。 此欄位會依優先順序顯示目標。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
您可以為組織建立未與專案個別業務案例連結的策略目標。 您必須擁有Adobe Workfront目標的存取權，才能建立策略目標。 然後，您就可以將他們與其業務案例以外的專案連結。 如需使用Workfront目標建立目標的相關資訊，請參閱 [Adobe Workfront目標概覽](../../../workfront-goals/goal-management/wf-goals-overview.md).

為專案定義目標是選用的，以在Portfolio最佳化程式中接收分數。 本節是「業務案例」中唯一的選用節。 必須先完成業務案例的所有其他部分，然後才能在Portfolio優化程式中對項目進行評分。 您可以在建立目標時指定目標的優先順序。

如需目標的詳細資訊，請參閱  [建立業務案例目標](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## 費用

開支指在項目期間可能發生的非人工成本。 此區域預設會在「業務案例」中啟用，但Workfront管理員可能會選擇不顯示。 

您在「業務案例」中輸入的任何費用也將作為「計畫費用」輸入到項目的「費用」標籤中。

費用會影響項目的以下欄位：

* 預算成本
* 淨值

有關預算成本和淨值的詳細資訊，請參閱 [業務案例財務欄位概覽](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

如需有關費用的詳細資訊，請參閱  [管理項目費用](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

您的Workfront管理員可以設定自訂費用類型。

有關建立自定義費用類型的詳細資訊，請參閱 [建立自定義支出類型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## 資源預算

您可以在「業務」案例的「資源預算」區域中執行以下操作：

* 將資源池與項目關聯。
* 在專案層級預算資源。

項目上資源的預算小時數顯示在「業務案例」的「資源預算」區域中，從而生成項目的預算人工成本。 預設情況下，會啟用「業務案例」的此區域。

有關Business Case中項目預算資源的詳細資訊，請參閱 [業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

查看業務案例的「資源預算」部分時，請考慮以下事項：

* 您可以使用下列工具在此對資源資訊進行預算：

   * 資源計畫員

      如需詳細資訊，請參閱 [使用資源計畫器在業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * 方案計畫員，如果貴公司已為Adobe方案計畫員購買了附加許可證

      如需詳細資訊，請參閱 [使用方案計畫器在業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      方案規劃器僅適用於新的Adobe Workfront體驗，需要額外的許可。 有關Workfront方案計畫器的資訊，請參閱 [方案計畫員概覽](../../../scenario-planner/scenario-planner-overview.md).

* 此處顯示的資訊也顯示在系統層資源計畫員或方案計畫員中。 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* 將資源預算編製成預算後，如果這些職責與「每小時成本」費率關聯，則項目的「預算人工成本」將顯示在「資源預算」區域中。 預算人工成本以項目幣種顯示。

   >[!IMPORTANT]
   「預算人工成本」是與項目上的職責相關的成本，而不是與用戶相關的成本。 用戶的所有預算人工成本的總和可能等於或不等於與用戶相關聯的職務職責的預算人工成本。 

   有關預算人工成本的詳細資訊，請參閱 [業務案例財務欄位概覽](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   有關建立任務角色以及將每小時成本費率與其關聯的詳細資訊，請參閱 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## 風險

風險是可能阻止項目按時或按預算完成的因素。 對於Portfolio經理或項目贊助商來說，定義這些因素對於在項目批准上做出明智決策非常重要。 此區域預設會在「業務案例」中啟用，但Workfront管理員可能會選擇不顯示。

您可以將潛在成本與您正在定義的風險關聯，以防其發生。 項目的風險成本會影響項目的淨值。 

如需專案淨值的詳細資訊，請參閱 [業務案例財務欄位概覽](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

有關建立風險的詳細資訊，請參閱  [建立和編輯項目風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

您的Workfront管理員可以設定自訂風險類型。

有關建立和編輯自定義風險類型的詳細資訊，請參閱 [編輯和建立風險類型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## 計分卡

計分卡可測量專案的對齊方式。 此區域預設會在「業務案例」中啟用，但Workfront管理員可能會選擇不顯示。

如需如何將計分卡套用至專案及產生對齊分數的詳細資訊，請參閱 [將計分卡套用至專案並產生對齊分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

若要套用計分卡，您的Workfront管理員必須建立計分卡。 此 **計分卡** 除非建立計分卡，否則不會顯示「業務案例」區域。

如需建立計分卡的詳細資訊，請參閱  [建立計分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## 自訂表單

定義業務案例時，您可以將自訂Forms附加至專案。 預設情況下，不會在「業務案例」中啟用此區域。 Workfront管理員必須啟用它，才能在「業務案例」中顯示。

有關啟用業務案例區域的詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

若要套用自訂表單，您的Workfront管理員必須先建立自訂表單。

如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

您可以使用自訂表單來收集未顯示在「業務案例」其他欄位中的其他資訊。

如需套用自訂表單的詳細資訊，請參閱 [將自訂表單附加至業務案例](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## 業務案例摘要

* [業務案例概要](#overview-of-the-business-case-summary)
* [導出業務案例](#export-the-business-case)

### 業務案例概要 {#overview-of-the-business-case-summary}

您可以在「業務案例摘要」面板的商業案例右上角查看主要項目財務摘要，以及項目是否與計分卡對齊。

您無法編輯業務案例摘要。 這只是與財務欄位和計分卡相關的專案狀態快速檢視。 \
 

「業務案例摘要」中顯示以下欄位：

* 項目淨值
* 項目預算成本
* 潛在風險成本
* 計畫的福利
* 對齊分數

如需這些欄位的詳細資訊，請參閱 [業務案例財務欄位概覽](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### 導出業務案例 {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

您可以將Business Case導出到PDF檔案，以備需要打印它或以更精簡的格式將其附加到電子郵件時使用。 

如需詳細資訊，請參閱 [導出項目的業務案例](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
