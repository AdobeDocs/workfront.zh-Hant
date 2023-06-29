---
product-area: projects
navigation-topic: financials
title: 覆寫工作角色帳單費率與計算專案收入的概要
description: 當您將專案收入乘以專案逗留時數時，可使用收費率來計算專案收入。 如需有關收費率和收入的詳細資訊，請參閱文章帳單和收入概觀。
author: Alina, Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '3852'
ht-degree: 0%

---

# 覆寫工作角色帳單費率與計算專案收入的概要

{{highlighted-preview}}

當您將專案收入乘以專案逗留時數時，可使用收費率來計算專案收入。 如需有關收費率和收入的詳細資訊，請參閱文章 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## 職務角色帳單費率與角色每小時收入型態概要

身為Adobe Workfront管理員，您可以將收費率與使用者和職位角色建立關聯。\
如需建立使用者及建立使用者與計費率關聯的詳細資訊，請參閱文章 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). 如需有關建立職位角色並將其與計費率相關聯的詳細資訊，請參閱文章 [建立和管理職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

無法覆寫與使用者相關聯的計費費率。

與工作角色相關的計費率可在公司或專案層級覆寫。

若要根據職務角色的收費率計算專案收入，請 **收入型別** 專案上任務必須為下列其中一項：

* 角色小時
* 受限角色小時
* 角色小時加固定

如需有關的詳細資訊 **收入型別** 和收費率，請參閱 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 計算收入時帳單費率覆寫的階層

職務角色可以透過下列方式與其相關聯的計費率：

* 身為Workfront管理員，您可以在建立工作角色時，定義與工作角色相關聯的系統層級收費率。\
  如需建立工作角色的詳細資訊，請參閱 [建立和管理職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 身為Workfront管理員，您可以在建立公司時，為相同職務角色定義公司層級的收費率。\
  當Workfront計算與此公司相關聯的專案收入時，當角色指派給任務時使用公司收費率，而不是此職務角色的系統層級收費率。\
  在公司層級變更的工作角色費率將影響與該公司關聯的所有專案。

  >[!NOTE]
  >
  >如果您需要更新公司收費率，專案費率不會自動更新。 您必須先從專案中移除公司、更新公司的費率，然後重新將公司附加至專案，新的公司費率才會對專案生效。 如需將公司附加至專案的指示，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

  如需建立公司特定職務角色收費率的詳細資訊，請參閱 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* 身為Workfront管理員，您可以在編輯專案時啟用選項，以在使用者手動重新計算專案財務時，將變更套用至公司層級的計費費率至專案。\
  如需詳細資訊，請參閱 [以公司層級的收費率覆寫專案層級的收費率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* 身為Workfront管理員，您可以根據位置與日期，定義每個角色擁有多個收費率的費率卡。 將費率卡附加至專案時，所有角色（如果使用了地點，則按地點）及其關聯的計費費率會新增至專案的計費費率區段。 附加費率卡會覆寫專案上任何現有的計費費率。

  如需詳細資訊，請參閱 [管理費率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) 和 [將費率卡附加至專案](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* 身為專案經理，您可以在專案層次為相同職務角色定義收費率。\
  專案上變更的工作角色費率只會影響該專案。

  如需有關覆寫專案角色比例的資訊，請參閱 [覆寫專案層次的工作角色收費率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>如果工作角色在系統層級、公司層級及專案層級與計費率相關聯，Workfront會在使用工作角色費率時，使用專案層級的工作角色計費率來計算任務的收入。 來自所有任務的收入累計至專案的收入。

## 覆寫專案層次的工作角色收費率

身為專案經理，您可以指定特定專案上工作角色的收費率。 此專案層級的收費率會覆寫此職務角色之系統層級的收費率。 Workfront使用工作角色的專案層級收費率來計算收入，而不使用系統層級收費率。

<span class="preview">您也可以將費率卡附加至專案，這樣會將職務角色帳單費率從費率卡匯入專案。</span>

如需如何在專案層次覆寫工作角色收費率的相關資訊，請參閱 [覆寫專案層次的工作角色收費率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

如需有關哪個工作角色用於計算專案收入的詳細資訊，請參閱以下的「根據使用者和角色指派的任務收入計算」一節： [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">如需將費率卡附加至專案的詳細資訊，請參閱 [將費率卡附加至專案](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>在實際收入中，套用至新增至標示為已記帳之記帳記錄時數的記帳費率，不應受記帳記錄記帳後發生的記帳費率覆寫影響。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 專案的「收費率」區段概要

在您指定與專案相關之職務角色的覆寫收費率後，您便可以在 **收費率** 索引標籤中。

請注意以下清單中的資訊 **收費率**：

* [職務角色群組](#job-role-grouping)
* [專案收費率值](#project-billing-rate-value)
* [預設收費率值](#default-billing-rate-value)
* [公司收費率值](#company-billing-rate-value)
* [多個收費率值和時間範圍](#multiple-billing-rate-values-and-timeframes)

### 職務角色群組 {#job-role-grouping}

記帳費率會分組在 **收費率** 區域（按其各自的工作角色）。 <span class="preview">如果專案附加了費率卡，則職務角色也會依費率卡分組。 如果將位置套用至工作角色，則位置名稱會包含為工作角色名稱的一部分。 您可以為多個位置列出相同的工作角色。</span>

### 專案收費率值 {#project-billing-rate-value}

在與職務角色對應的群組明細行中，請注意中專案層次該職務角色的計費率。 **專案收費率** 欄。 如果職務角色有多個覆寫費率，則與目前日期對應的覆寫費率會顯示在 **專案收費率** 欄。

### 預設收費率值 {#default-billing-rate-value}

在職務角色的分組明細行中，請注意系統層次中該職務角色的計費費率。 **預設收費率** 欄。

>[!NOTE]
>
>如果工作角色有專案收費率，則 **預設收費率** 絕不會套用於計算專案的收入。 僅限 **專案收費率** 套用於計算收入。

### 公司收費率值 {#company-billing-rate-value}

在職務角色的分組明細行中，請注意中公司層次該職務角色的計費率。 **公司收費率** 欄。 這表示有公司與此專案相關聯，而且此工作角色對該公司有不同的收費率。 即使公司收費率與專案收費率相同，也會顯示公司收費率。

>[!NOTE]
>
><span class="preview">將費率卡附加至專案時， **公司收費率** 不會匯入帳單費率。 計算是以職務角色的費率卡費率或公司費率為基礎。</span>
>
>如果工作角色有專案收費率，則 **公司收費率** 絕不會套用於計算專案的收入。 僅限 **專案收費率** 用於計算收入。

### 多個收費率值和時間範圍 {#multiple-billing-rate-values-and-timeframes}

如果您有多個覆寫特定職務角色的收費率，則會列在該職務角色的分組底下。 使用內聯編輯，您可以變更覆寫率和 **開始** **日期** 和 **結束日期** 此標籤上的覆寫收費率。

>[!NOTE]
>
>您無法指定 **開始日期** 對於首次覆寫率，您不能指定 **結束日期** 上次覆寫率的。 Workfront假設第一個覆寫率適用於日期早於以下日期的所有時數： **結束日期** ，且最後覆寫率適用於日期晚於以下時間的所有時數： **開始日期** 上次覆寫的。\
>如果在專案的計劃開始日期之前記錄了一個小時，則使用第一個收費率。\
>如果是在專案的計畫完成日期後記錄一小時，則使用最後一個收費率。

## 計算計畫收入

* [根據一次性記帳費率覆寫計算計畫收入](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [根據多重記帳費率覆寫來計算計畫收入](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [整個任務持續期間的計畫時數分佈](#distribution-of-planned-hours-across-the-duration-of-a-task)

### 根據一次性記帳費率覆寫計算計畫收入 {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

根據一次性記帳費率覆寫計算計畫收入時，請考量下列事項：

* 當 **收入型別** 任務的 **角色小時**，Workfront會將任務的計畫時數乘以與任務相關的工作角色的計費率，以計算任務的計畫收入。

* 當在專案層級覆寫工作角色的計費率時，Workfront會使用專案的覆寫率來計算計畫收入。
* 當任務有多個指派時，計畫收入的計算方式是將每個指派的工作角色的計費率乘以它們各自的計畫時數分配。

>[!NOTE]
>
>若有多個指派，則每個指派的計畫時數與任務的計畫時數不同。

如需有關哪一個職務角色用於計算計畫收入的詳細資訊，請參閱本文章的「瞭解根據使用者和角色指派的任務收入計算」一節 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### 根據多重記帳費率覆寫來計算計畫收入 {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

根據多重記帳費率覆寫來計算計畫收入時，請考量下列事項：

* 當 **收入型別** 任務的 **角色小時**，Workfront會將任務的計畫時數乘以與任務相關的工作角色的計費率，以計算任務的計畫收入。

  如需有關哪一個職務角色用於計算計畫收入的詳細資訊，請參閱本文章的「瞭解根據使用者和角色指派的任務收入計算」一節 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 如果覆寫了多個計費費率，則計畫時數在任務持續期間所乘以的費率會變更。 根據預設，Workfront會在任務期間平均分配計畫時數，並為任務的每天分配相等的時數。 計算時 **計畫收入** 對於任務，Workfront會將每日計畫時數乘以當天的計費率。 若是多個收費率，該費率每天可能都不相同。

  例如，您有一個任務具有每小時的角色 **收入型別**. 任務的持續時間為5天，計畫時數的值為40小時。 計畫每日時數為8小時。 將「專案經理」工作角色指派給任務，並覆寫此工作角色在任務最後3天的收費率，因此您在前兩天會有「費率1」的收費率，在此工作角色在任務剩餘的3天會有「費率2」的收費率。

  計算下列專案的公式： **計畫收入** 此任務為：

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

如需在Workfront中尋找每日計畫時數數量的詳細資訊，請參閱區段 [整個任務持續期間的計畫時數分佈](#distribution-of-planned-hours-across-the-duration-of-a-task) 本文章內容。

>[!NOTE]
>
>如果任務有多個受指派人，則計畫時數會先分配給每個受指派人，然後在任務持續期間分配給每一天。 在此情況下，計畫收入的計算將考量每個受指派人的每日時數金額，以及每個工作角色的計費率，若有多個計費率，則計費率可能會在工作期間變更。

### 整個任務持續期間的計畫時數分佈 {#distribution-of-planned-hours-across-the-duration-of-a-task}

瞭解任務期間中計畫時數的分佈時，請考量下列事項：

* 依預設，Workfront會根據專案排程的可用性，將計畫時數平均分配給任務的期間，並為任務的每天分配相等數量的計畫時數。

  如需瞭解跨任務期間計畫時數分佈的詳細資訊，請參閱文章中的「瞭解跨任務期間計畫時數分佈」一節 [計畫時數概觀](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >「每日計畫時數」是在任務期間每天的計畫時數配置。 如果任務有一個指派，則此數字也代表每個指派的每日計畫時數。 如果任務有多個指派，則每個指派的每日計畫時數與任務的每日計畫時數不同。 對於具有多個指派的任務，Workfront中沒有每個指派的每日計畫時數視覺化表示法。
  >
  >
  >每日計畫時數乘以當天指派給任務的工作角色的收費率，以計算該任務的每日計畫收入。 以這種方式計算的所有每日計畫收入的總和等於該任務的計畫收入。

## 計算實際收入

* [根據一次性記帳費率覆寫來計算實際收入](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [根據多重記帳費率覆寫來計算實際收入](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### 根據一次性記帳費率覆寫來計算實際收入 {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

根據一次性「收費率」覆寫計算「實際收入」時，請考量下列事項：

* 當 **收入型別** 任務的 **角色小時**，Workfront會將 **實際小時** 按與要計算之任務相關之職務角色的收費率排列的任務金額 **實際收入** 在任務上。 實際時數是直接記錄至任務的時數。

  有關使用哪個工作角色進行計算的詳細資訊 **實際收入**，請參閱文章中的「瞭解根據使用者和角色指派的任務收入計算」一節 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 如果已在專案層次覆寫工作角色的計費費率，Workfront會使用專案的覆寫費率來計算實際收入。 當您覆寫專案上工作角色的計費費率時， **實際收入** 會使用新的調整後費率自動重新計算專案的。

  如需有關覆寫專案角色比例的資訊，請參閱 [覆寫專案層次的工作角色收費率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>如果您想要保留在覆寫以原始費率計費的原始計費率之前已登入專案的時數，則必須將其納入 **付費記錄**，而且您必須標籤 **付費記錄** 作為 **已記帳**. 否則， **實際收入** 從覆寫專案的計費費率之前記錄的時數，將在重新計算專案的財務時使用新費率重新計算。\
>如需在付費記錄中包含時數並標示為的詳細資訊 **已記帳**，請參閱文章 [建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

### 根據多重記帳費率覆寫來計算實際收入 {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

根據多重記帳費率修訂來計算實際收入時，請考量下列事項：

* 當 **收入型別** 任務的 **角色小時**，Workfront會將 **實際小時** 具有指派給要計算之任務之職務角色計費率的任務上 **實際收入** 在任務上。 實際時數是直接記錄至任務的時數。

* 若有多項帳單費率覆寫，則為下列專案的費率： **實際小時** 乘以計算 **實際收入** 在任務持續期間可能會變更。 Workfront使用時間範圍符合以下條件的工作角色的計費率： **輸入日期** 任務要計算的記錄時數 **實際收入。**

  例如，任務具有 **收入型別** 之 **角色小時** 和會指派給Project Manager的工作角色。 以6月19日至6月25日期間的費率1覆寫此職務角色的計費費率。 從6月26日開始，使用費率2覆寫收費率。 記錄6月20日的2小時，以及6月28日的3小時。

  Workfront計算 **實際收入** 對於此工作，請使用下列公式：

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  有關使用哪個工作角色進行計算的詳細資訊 **實際收入**，請參閱文章中的「瞭解根據使用者和角色指派的任務收入計算」一節 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 根據多個記帳費率計算收入時的時區影響

使用者與其他使用者相比，如果他們與Workfront中的其他實體之間發生時區差異，則他們可能會看到不同的每日計畫時數。 以下情況可能會將使用者的「每日計畫時數」資訊與其他使用者看到的資訊有所偏差：

* 這兩個使用者的電腦可能設定為兩個不同的時區
* Workfront中的兩個使用者設定檔可能設定為兩個不同的時區
* 與使用者設定檔相關聯的時區可能與Workfront中的系統時區不同
* 與使用者設定檔相關聯的時區可能與專案排程的時區不同。

在這些情況下，兩個不同時區設定相同的使用者之間，每天的計畫時數可能會不同。 在專案上使用多個收費率覆寫時，他們也會看到不同的計畫收入數字。

* [計算不同時區使用者的計畫收入](#calculate-planned-revenue-for-users-in-different-time-zones)
* [計算不同時區使用者的實際收入](#calculate-actual-revenue-for-users-in-different-time-zones)

### 計算不同時區使用者的計畫收入 {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>如果您讓不同時區的使用者處理相同的專案，我們建議您不要在當週變更專案的計費率覆寫。 這樣做可能會因為使用者排程中的時區與Workfront系統時區之間的時區差異，而導致您的專案顯示錯誤的計畫收入金額。 大多數排程允許將週末從計畫時數計算中排除。 如果工作角色的計費率覆寫發生變更，最好在週末進行，而不是在周中進行，因為這可能與任務期間的中間時間一致。

計算不同時區之使用者的計畫收入時，請考量下列事項：

* 針對具有下列專案的任務： **收入型別** 之 **角色小時** 和指派至職務角色， **計畫收入** 的計算方式為將 **計畫時數** 按工作角色的計費率排列的任務。

* 此 **計畫時數** 平均分佈於 **持續時間** 任務的。

* 此 **持續時間** 是介於以下時間之間的時段： **計劃開始** **日期** 和 **計畫完成日期** 任務的。 因為&#x200B;**計劃開始日期** 和 **計畫完成日期** 其中一項任務可能因檢視任務之使用者的時區而異，兩個使用者在兩個不同時區的每日計畫時數可能不同。

* 若未變更工作角色的計費率或僅有一個計費率覆寫，則每日計畫時數金額不會變更專案的計畫收入。 在此情況下，即使來自兩個不同時區的兩名使用者看到不同的每日計畫時數，兩個使用者之間的專案整體計畫收入仍相同。

  不過，若有多個計費率覆寫，則整體的 **計畫收入** 兩個使用者在兩個不同時區中的專案可能會看起來不同，因為它依賴於每日計畫時數（兩個使用者可能不同）和計費率覆寫（當每個使用者在自己的時區檢視任務時，當天可能會不同）。

* 精確的 **計畫收入** amount是與Workfront執行個體時區具有相同時區的使用者所看到的數量。 您的Workfront管理員會在系統客戶資訊區域中定義Workfront時區。\
  如需定義系統時區的詳細資訊，請參閱文章 [為您的系統設定基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 計算不同時區使用者的實際收入 {#calculate-actual-revenue-for-users-in-different-time-zones}

計算不同時區中使用者的實際收入時，請考量下列事項：

* 當 **收入型別** 任務的 **角色小時**，Workfront會將 **實際小時** 對具有指派給任務以計算之職務角色之收費率的任務而言 **實際收入**. 實際時數是直接記錄至任務的時數。

* 如果覆寫了多個收費率，Workfront會使用時間範圍符合以下條件的工作角色的收費率： **輸入日期** 任務要計算的記錄時數 **實際收入**.

* 因為沒有時間戳記 **輸入日期** 時數，且多個計費率覆寫的日期範圍上沒有時間戳記， **實際收入** 計算不受與使用者相關聯的時區影響。

有關使用哪個工作角色進行計算的詳細資訊 **實際收入**，請參閱文章中的「瞭解根據使用者和角色指派的任務收入計算」一節 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 重新計算專案財務

當專案記錄的時數發生變更時，會在專案上計算財務。

如果在專案存留期內費率已變更，您可以使用專案的「重新計算財務」選項，手動重新計算專案的成本和收入。 此外，某些動作會觸發自動重新計算。

如需重新計算專案財務的詳細資訊，請參閱文章 [重新計算專案財務](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## 使用API新增收費率

若要使用API為工作角色新增收費率，請執行 *setRatesForRole* 的動作 **評等** 物件 *PUT方法*.
上的動作和日期欄位 **評等** 物件可在API 8.0版中使用。如果您已為專案中的工作角色定義了數個收費率，並且想要使用新的日期範圍為其新增新的收費率，則必須同時包含現有收費率和要新增在同一API呼叫中的收費率。 這類似於更新物件集合的方式。

以下API呼叫為範例，其中 **attachableID** 是 **專案ID** 要新增費率與優惠方案的專案 **角色ID** 是 **工作角色ID** 您正在為其新增計費費率。<pre>{</pre><pre>&quot;attachableID&quot;：&quot;593f01500000557d75fdd4fdfcc624f2&quot;，</pre><pre>&quot;attachableObjCode&quot;：&quot;PROJ&quot;，</pre><pre>&quot;roleID&quot;：&quot;544820df000014148cda5136d4b79d09&quot;， </pre><pre>&quot;rates&quot;：[</pre><pre>         {&quot;rateValue&quot;：&quot;0.00&quot;，&quot;startDate&quot;：null，&quot;endDate&quot;：&quot;2017-06-11&quot;}，</pre><pre>         {&quot;rateValue&quot;：&quot;45.00&quot;，&quot;startDate&quot;：&quot;2017-06-12&quot;，&quot;endDate&quot;：&quot;2017-06-17&quot;}，</pre><pre>         {&quot;rateValue&quot;：&quot;95.00&quot;，&quot;startDate&quot;：&quot;2017-06-21&quot;，&quot;endDate&quot;：null}</pre><pre>]</pre><pre>}</pre>如需使用Workfront API的詳細資訊，請參閱文章 [API基本需知](https://experience.workfront.com/s/article/API-Basics-638808549).
