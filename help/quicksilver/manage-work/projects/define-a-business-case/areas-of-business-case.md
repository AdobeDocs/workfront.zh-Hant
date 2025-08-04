---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 業務案例的領域概述
description: 本文會說明專案的業務案例領域。
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: 14b6b9c4a184131cfdc33b6156c578218ed9119a
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 1%

---

# 業務案例區域概覽

<!-- Audited: 4/2025 -->

本文會說明專案的業務案例領域。

如需為專案建立業務案例的相關資訊，請參閱[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

您的Adobe Workfront管理員或群組管理員必須啟用「業務案例」中的所有區段，才能在專案中看到這些區段，但「專案資訊」區段除外。 專案資訊區段預設為啟用。

如需有關啟用業務案例區域的詳細資訊，請參閱文章[設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)中的業務案例區段。

以下是專案業務案例中的區域：

* 專案資訊
* 目標
* 費用
* 資源預算
* 風險
* 計分卡
* 自訂表單
* 業務案例摘要

## 專案資訊

「業務案例」的「專案資訊」區段包含專案實際開始前的基本資訊。

所有專案在業務案例中都有一個包含預先設定欄位的專案資訊區域，這表示Workfront管理員無法設定要在此區域顯示哪些欄位。

請考慮編輯下列欄位：

* **描述**：新增專案的描述。

* **專案所有者**：依照預設，建立專案的使用者也是專案所有者。 編輯此欄位以選取其他作用中使用者作為專案所有者。

* **專案贊助者**：選取將會是專案贊助者的作用中使用者。 贊助者會收到業務案例的核准。

* **Portfolio**：選取專案的Portfolio。 您必須建立Portfolio並將其置於作用中狀態，才能在此下拉式選單中進行選取。

  如需投資組合的詳細資訊，請參閱[Adobe Workfront中的Portfolio概觀](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)。

  如需關於建立投資組合的詳細資訊，請參閱[建立投資組合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)。

* **計畫收益**：預估此專案完成時，貴組織計畫的貨幣收益。 它可以是任何數量的貨幣，且必須是正值（例如$10,000）。

* **狀態**：依預設，專案要求的狀態設定為Idea。 如果您將「狀態」變更為「創意」或「計畫」以外的任何專案，「提交」按鈕會從「業務案例彙總」區域消失，您無法再提交「業務案例」進行核准。

* **固定開始日期**：指定您想要專案開始的日期。

* **固定結束日期**：指定您想要專案結束的日期。

  >[!NOTE]
  >
  >業務案例的固定開始和結束日期不會影響專案的計劃開始和完成日期。 這些代表專案建立者要求的專案理想開發日期。 相反地，專案的計劃開始和計畫完成日期會顯示根據專案任務的專案計畫時間表。

## 目標

目標會定義專案的目標。 此區域在業務案例中預設為啟用，但Workfront管理員可能會選擇不顯示。 此欄位會依優先順序顯示目標。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>您可以為組織建立未與專案的個別業務案例連結的戰略目標。 您必須擁有Adobe Workfront目標的存取權才能建立策略目標。 然後，您可以將他們與業務案例以外的專案連線。 如需使用Workfront目標建立目標的相關資訊，請參閱[Adobe Workfront目標總覽](../../../workfront-goals/goal-management/wf-goals-overview.md)。

若要讓專案在Portfolio Optimizer中取得分數，可自行選擇定義目標。 此區段是業務案例中唯一的選用區段。 您必須先完成業務案例的所有其他區段，專案才能在Portfolio Optimizer中計分。 您可以在建立目標時指定目標的優先順序層級。

如需詳細資訊，請參閱[建立業務案例目標](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md)。

## 費用

費用代表專案期限內可能產生的非人力成本。 此區域在業務案例中預設為啟用，但Workfront管理員可以選擇不顯示。

您在業務案例中輸入的任何費用也會在專案的「費用」標籤上輸入為「計畫費用」。

費用會影響專案的下列欄位：

* 預算成本
* 淨值

您的Workfront管理員可以設定自訂費用型別。

如需預算成本與淨值的詳細資訊，請參閱[業務案例財務欄位概觀](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

如需費用的詳細資訊，請參閱[管理專案費用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

如需建立自訂費用型別的詳細資訊，請參閱[建立自訂費用型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md)。

## 資源預算

您可以在「業務案例」的「資源預算」區域中執行下列動作：

* 將資源集區與專案建立關聯。
* 在專案層次編列您的資源預算。

專案資源的預算時數會顯示在業務案例的資源預算區域中，產生專案的預算勞力成本。 此區域預設為啟用。

如需商務案例中專案預算資源的詳細資訊，請參閱商務案例中的[預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

<!--![Business case resource budgeting](assets/business-case-sp-selected-with-choose-button-350x121.png)-->

檢視業務案例的「資源預算」區段時，請考量下列事項：

* 您可以使用下列工具在此預算資源資訊：

   * 資源規劃工具

     如需詳細資訊，請參閱使用資源規劃工具[的業務案例中的](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md)預算資源。

   * 情境規劃工具

     如需詳細資訊，請參閱使用案例規劃工具[的業務案例中的](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)預算資源。

     Scenario Planner僅在新的Adobe Workfront體驗中可用，並且需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../../scenario-planner/scenario-planner-overview.md)。

* 此處顯示的資訊也會顯示在系統層級的「資源規劃工具」或「案例規劃工具」中。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* 編列資源預算後，如果角色與每小時成本費率相關聯，則專案的預算勞力成本會顯示在「資源預算」區域中。 預算勞力成本會以專案的貨幣顯示。

  >[!IMPORTANT]
  >
  >預算勞力成本是與專案中的角色相關聯而不是與使用者相關聯的成本。 使用者的所有預算勞力成本總和可能等於或不等於與使用者相關聯之工作角色的預算勞力成本。

  如需預算勞力成本的詳細資訊，請參閱[業務案例財務欄位概觀](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

  如需有關建立工作角色以及將每小時成本與其產生關聯的詳細資訊，請參閱[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

## 風險

風險是可能會阻止專案準時或準時完成的因素。 定義這些因素對Portfolio經理或專案贊助者來說很重要，因為這樣就能在專案核准上做出明智的決策。 此區域在業務案例中預設為啟用，但Workfront管理員可以選擇不顯示。

您可以將潛在成本與所定義的風險建立關聯，以防發生風險。 風險成本會影響專案的淨值。

您的Workfront管理員可以設定自訂風險型別。

如需有關專案淨值的詳細資訊，請參閱[業務案例財務欄位概觀](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

如需建立風險的詳細資訊，請參閱[在專案上建立和編輯風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。

如需建立與編輯自訂風險型別的詳細資訊，請參閱[編輯與建立風險型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md)。

## 計分卡

計分卡可測量專案的對齊方式。 此區域在業務案例中預設為啟用，但Workfront管理員可以選擇不顯示。

若要套用計分卡，您的Workfront管理員必須先建立計分卡。 除非建立計分卡，否則不會顯示業務案例的計分卡區域。

如需將計分卡套用至專案及產生一致性分數的詳細資訊，請參閱[將計分卡套用至專案並產生一致性分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

如需建立計分卡的詳細資訊，請參閱[建立計分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

## 自訂表單

定義業務案例時，您可以將自訂Forms附加至專案。 此區域在業務案例中預設為未啟用，Workfront管理員必須啟用它才能在業務案例中顯示。

若要套用自訂表單，您的Workfront管理員必須先建立自訂表單。

您可以使用自訂表單來收集未顯示在業務案例其他欄位中的其他資訊。

如需有關啟用業務案例區域的詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

如需建立自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

如需套用自訂表單的詳細資訊，請參閱[將自訂表單附加至業務案例](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md)。

## 業務案例摘要

* [業務案例摘要概要](#overview-of-the-business-case-summary)
* [匯出業務案例](#export-the-business-case)

### 業務案例摘要概要 {#overview-of-the-business-case-summary}

您可以在位於業務案例右上角的業務案例摘要面板中檢視主要專案財務的摘要，以及專案是否與計分卡對齊。

業務案例摘要只是專案狀態的快速檢視，因為它與財務欄位和計分卡有關，並且無法編輯。

「業務案例彙總」中會顯示下列欄位：

* 專案淨值
* 專案預算成本
* 潛在風險成本
* 計畫收益
* 一致性分數

如需這些欄位的詳細資訊，請參閱[業務案例財務欄位概觀](../../../manage-work/projects/define-a-business-case/business-case-finances.md)。

### 匯出業務案例 {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

如果您需要列印業務案例或將其附加至電子郵件，以更精簡的格式列印，您可以將業務案例匯出至PDF檔案。

如需詳細資訊，請參閱[匯出專案的業務案例](../../../manage-work/projects/define-a-business-case/export-business-case.md)。

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

