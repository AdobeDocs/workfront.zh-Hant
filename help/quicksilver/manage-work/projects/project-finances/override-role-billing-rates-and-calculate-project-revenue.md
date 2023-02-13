---
product-area: projects
navigation-topic: financials
title: 改寫任務職責開單費率和計算項目收入概覽
description: 當您將專案的收入乘以專案逗留時間時，可使用計費率來計算收入。 有關開單費率和收入的詳細資訊，請參閱開單和收入概覽一文。
author: Alina
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3644'
ht-degree: 0%

---

# 改寫任務職責開單費率和計算項目收入概覽

當您將專案的收入乘以專案逗留時間時，可使用計費率來計算收入。 如需帳單費率和收入的詳細資訊，請參閱文章 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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

## 職務職責開單費率和職責每小時收入類型概覽

身為Adobe Workfront管理員，您可以將計費率與使用者和工作角色建立關聯。\
有關建立用戶以及將其與計費費率關聯的詳細資訊，請參閱文章 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). 有關建立職務職責並將其與開單費率關聯的詳細資訊，請參閱文章 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

無法覆蓋與用戶關聯的計費率。

在公司或項目層，可以改寫與職務角色關聯的開單費率。

要根據任務職責的開單費率計算項目收入，請 **收入類型** 項目任務中必須有下列任務之一：

* 角色小時
* 受限角色小時
* 角色每小時加固定

如需 **收入類型** 和計費率，請參閱 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 計算收入時開單率覆蓋的層次結構

職務角色可以通過以下方式與其相關聯的計費率：

* 作為Workfront管理員，您可以在建立作業角色時定義與作業角色相關聯的系統層級計費率。\
   有關建立作業角色的詳細資訊，請參閱 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 作為Workfront管理員，您可以在建立公司時為相同職務角色定義公司層級的計費率。\
   當Workfront計算與此公司關聯的項目的收入時，將在將職責分配給任務時使用公司開單費率，而不是此職務職責的系統層開單費率。\
   在公司層級變更的職務角色比率將影響與該公司相關聯的所有專案。

   >[!NOTE]
   >
   >如果您需要更新公司開單費率，則項目費率不會自動更新。 您必須先將公司從項目中刪除，更新公司費率，然後將公司重新附加到項目，新公司費率才會對項目生效。 如需將公司附加至專案的說明，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

   有關建立公司特定職務職責開單費率的詳細資訊，請參閱 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* 作為Workfront管理員，您可以在編輯項目時啟用選項，以在用戶手動重新計算項目財務時，將公司層開單費率的更改應用於項目。\
   如需詳細資訊，請參閱 [用公司層開單費率改寫項目層開單費率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* 作為項目經理，您可以在項目層定義相同職務職責的開單費率。\
   項目上更改的職務費率只會影響該項目。

   有關覆蓋項目的角色費率的資訊，請參閱 [在項目層改寫任務職責開單費率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>如果職務職責與系統層、公司層和項目層的開單費率關聯，則Workfront在使用職務職責費率時，使用項目層職務職責的開單費率計算任務的收入。 所有任務的收入累計到項目的收入。

## 在項目層改寫任務職責開單費率

作為項目經理，您可以指定特定項目上某個職務角色的計費費率。 此項目層開單費率將改寫此職務職責的系統層開單費率。 Workfront會使用工作角色的專案層開單比率來計算收入，而非使用系統層開單比率。

有關如何改寫項目層職務開單費率的資訊，請參閱 [在項目層改寫任務職責開單費率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

有關使用哪個職務來計算項目收入的詳細資訊，請參閱 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>在實際收入情況下，應用於添加到標籤為「開單」的開單記錄的小時的開單費率，不應受在開單記錄開單後發生的開單費率改寫的影響。

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

## 項目的「計費率」部分概覽

在為與項目關聯的任務角色指定改寫開單費率後，您可以在 **計費率** 頁簽。

請注意 **計費率**:

* [作業角色分組](#job-role-grouping)
* [項目開單費率值](#project-billing-rate-value)
* [預設開單費率值](#default-billing-rate-value)
* [公司開單費率值](#company-billing-rate-value)
* [多個開單費率值和時間範圍](#multiple-billing-rate-values-and-timeframes)

### 作業角色分組 {#job-role-grouping}

開單率按 **計費率** 區域。

### 項目開單費率值 {#project-billing-rate-value}

在與任務職責對應的分組行中，注意項目層中該任務職責的開單率。 **項目開單率** 欄。 如果任務職責具有多個改寫率，則與當前日期對應的改寫率將顯示在 **項目開單率** 欄。

### 預設開單費率值 {#default-billing-rate-value}

在任務職責的分組行中，注意系統層中該任務職責的開單率。 **預設開單率** 欄。

>[!NOTE]
>
>如果職務職責有項目開單費率，則 **預設開單率** 不會套用至計算專案的收入。 僅 **項目開單率** 套用以計算收入。

### 公司開單費率值 {#company-billing-rate-value}

在職務職責的分組行中，請注意該職務職責在公司層(位於 **公司帳單率** 欄。 這表示有一個公司與此項目關聯，而此職務角色對該公司的計費率不同。 即使與項目費率相同，也會顯示公司的開單費率。

>[!NOTE]
>
>如果職務職責有項目開單費率，則 **公司帳單率** 不會套用至計算專案的收入。 僅 **項目開單率** 套用以計算收入。

### 多個開單費率值和時間範圍 {#multiple-billing-rate-values-and-timeframes}

如果特定職務職責有多個改寫開單費率，則這些費率將列在該職務職責的分組下。 您可以使用內嵌編輯來變更覆寫率，以及 **開始** **日期** 和 **結束日期** 標籤中的覆蓋開單費率。

>[!NOTE]
>
>您無法指定 **開始日期** 對於第一個覆蓋率，您不能指定 **結束日期** 上次覆蓋率。 Workfront假設第一個覆寫率套用至所有日期早於 **結束日期** 的值，且最後一個覆蓋率會套用至日期早於 **開始日期** 上次覆寫的。\
>如果在項目的計畫起始日期之前記錄了一個小時，則使用第一個開單費率。\
>如果在項目的計畫完成日期之後記錄了一個小時，則使用最後的開單率。

## 計算計畫收入

* [根據一次性開單費率改寫計算計畫收入](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [根據多個開單費率改寫計算計畫收入](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [在任務期間內的計畫時數分配](#distribution-of-planned-hours-across-the-duration-of-a-task)

### 根據一次性開單費率改寫計算計畫收入 {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

根據一次性開單費率改寫計算計畫收入時，請考慮以下事項：

* 當 **收入類型** 是 **角色每小時**,Workfront會將任務的計畫小時數乘以與任務關聯的任務職責的開單比率，以計算任務的計畫收入。

* 當在項目層改寫了職務職責的開單費率時，Workfront將使用項目的改寫費率來計算計畫收入。
* 當任務具有多個分配時，計畫收入的計算方法是將每個分配的任務職責的開單比率與各自的計畫小時分配相乘。

>[!NOTE]
>
>對於多個分配，每個分配的計畫小時數與任務的計畫小時數不同。

有關用於計算計畫收入的職務職責的詳細資訊，請參閱文章中的「了解基於用戶和職責分配的任務的收入計算」部分 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### 根據多個開單費率改寫計算計畫收入 {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

根據多個開單費率改寫計算計畫收入時，請考慮以下事項：

* 當 **收入類型** 是 **角色每小時**,Workfront會將任務的計畫小時數乘以與任務關聯的任務職責的開單比率，以計算任務的計畫收入。

   有關用於計算計畫收入的職務職責的詳細資訊，請參閱文章中的「了解基於用戶和職責分配的任務的收入計算」部分 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 在多個開單費率改寫的情況下，在任務期間計畫小時數的乘數變化。 依預設，Workfront會在任務期間平均分配計畫小時數，為任務的每天分配相同的小時數。 計算時 **計畫收入** 對於任務，Workfront會將每日計畫小時數乘以當天的計費率。 若是多個計費費率，該費率可能每天有所差異。

   例如，您的任務為每小時角色 **收入類型**. 任務的持續時間為5天，「計畫小時數」值為40小時。 每天計畫小時數為8小時。 為任務分配項目經理職務職責，並改寫任務最後3天的此職務職責的開單費率，因此，您將為前2天的費率1開單費率，為此職務職責的剩餘3天的任務設定費率2開單費率。

   計算 **計畫收入** 其中：

   ```
   Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
   ```

如需在Workfront中尋找「每日計畫小時數」金額的詳細資訊，請參閱區段 [在任務期間內的計畫時數分配](#distribution-of-planned-hours-across-the-duration-of-a-task) 這篇文章。

>[!NOTE]
>
>如果任務上有多個受分配人，則計畫小時數量首先分配給每個受分配人，然後分配給任務期間的每天。 在此情況下，計畫收入將考慮每個受託人的每日小時數和每個任務職責的開單費率，在多個開單費率的情況下，這些費用在任務期間可能會更改。

### 在任務期間內的計畫時數分配 {#distribution-of-planned-hours-across-the-duration-of-a-task}

了解任務期間計畫小時的分配時，請考慮以下事項：

* 依預設，Workfront會根據專案排程的可用性，在任務的持續時間內平均分配計畫小時數，為每天的任務分配相等數量的計畫小時數。

   有關了解任務期間計畫小時數分配的詳細資訊，請參閱文章中的「了解任務期間計畫小時數的分配」部分 [計畫小時數概觀](../../../manage-work/tasks/task-information/planned-hours.md).

   >[!NOTE]
   >
   >「每天計畫小時數」是任務期間每天的計畫小時數分配。 如果任務有一個分配，則此數字表示每個分配的每天計畫小時數。 如果任務具有多個分配，則每個分配的「每天計畫小時數」與任務的「每天計畫小時數」不同。 對於具有多個分配的任務，Workfront中沒有每天計畫小時數的可視表示。
   >
   >
   >計畫小時數乘以分配給該日任務的任務職責的開單費率，以計算該任務的「每日計畫收入」。 以此方式計算的所有每日計畫收入的總和等於該任務的計畫收入。

## 計算實際收入

* [根據一次性開單費率改寫計算實際收入](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [根據多個開單費率改寫計算實際收入](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### 根據一次性開單費率改寫計算實際收入 {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

根據一次性開單費率改寫計算實際收入時，請考慮以下事項：

* 當 **收入類型** 是 **角色每小時**, Workfront **實際小時數** 按與任務關聯的任務職責的計費率計算任務的 **實際收入** 任務。 實際小時數直接記錄到任務中。

   有關用於計算的作業角色的詳細資訊 **實際收入**，請參閱文章的「了解根據使用者和角色指派的任務的收入計算」一節 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 如果在項目層改寫了職務職責的開單費率，則Workfront將使用項目的改寫費率來計算實際收入。 當您改寫項目上職務職責的開單率時， **實際收入** 使用新的調整率自動重新計算項目的。

   有關覆蓋項目的角色費率的資訊，請參閱 [在項目層改寫任務職責開單費率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>如果您想在按原始費率計算原始計費費率之前保留已登錄項目的小時數，則必須將其納入 **帳單記錄**，且您必須將 **帳單記錄** as **已計費**. 否則， **實際收入** 在重新計算項目的財務時，將使用新費率重新計算項目在改寫開單費率之前記錄的小時數。\
>有關將小時數納入計費記錄並標籤為 **已計費**，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

### 根據多個開單費率改寫計算實際收入 {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

根據多個開單費率改寫計算實際收入時，請考慮以下事項：

* 當 **收入類型** 是 **角色每小時**, Workfront **實際小時數** 任務，其任務職責的開單費率分配給任務以計算 **實際收入** 任務。 實際小時數直接記錄到任務中。

* 如果是多個開單費率改寫， **實際小時數** 被乘以計算 **實際收入** 可能會在任務期間變更。 Workfront使用時間範圍符合 **參加日期** 記錄的任務小時數以計算 **實際收入。**

   例如，任務具有 **收入類型** of **角色每小時** 和被分配給項目經理的工作角色。 在6月19日至6月25日之間，使用費率1改寫此職務職責的開單費率。 從6月26日開始，用費率2改寫開單費率。 6月20日記錄2小時，6月28日記錄3小時。

   Workfront會計算 **實際收入** 使用下列公式執行此任務：

   ```
   Actual Revenue = 2 * Rate 1 + 3 * Rate 2
   ```

   有關用於計算的作業角色的詳細資訊 **實際收入**，請參閱文章的「了解根據使用者和角色指派的任務的收入計算」一節 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 根據多個計費率計算收入時，時區的影響

如果使用者與Workfront中的其他實體之間發生時區差異，則使用者每日可以看見與其他使用者不同的計畫小時數。 下列案例可能會將使用者的每日計畫時數資訊與其他使用者看到的內容扭曲：

* 這兩個使用者的電腦可能設定為兩個不同的時區
* Workfront中的兩個使用者設定檔可能會設為兩個不同的時區
* 與使用者設定檔相關聯的時區可能與Workfront中的系統時區不同
* 與使用者設定檔相關聯的時區可能與專案排程的時區不同。

在這些情況下，不共用相同時區設定的兩個使用者之間的「每日計畫小時數」可能會不同。 對專案使用多個計費率覆寫時，他們也會看到不同的計畫收入編號。

* [計算不同時區中使用者的計畫收入](#calculate-planned-revenue-for-users-in-different-time-zones)
* [計算不同時區中使用者的實際收入](#calculate-actual-revenue-for-users-in-different-time-zones)

### 計算不同時區中使用者的計畫收入 {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>如果您讓位於不同時區的使用者處理相同的專案，建議您不要在當周變更專案的計費率覆寫。 這麼做可能會因為使用者排程中的時區與Workfront系統時區之間的小時差，而顯示您專案的錯誤計畫收入金額。 大多數計畫允許將週末從「計畫小時數」計算中排除。 如果工作職責的開單費率改寫發生了更改，則週末期間發生更改比一週中間發生更好，因為該更改可能與任務持續時間的中間時間重合。

計算不同時區使用者的「計畫收入」時，請考量下列事項：

* 對於具有 **收入類型** of **角色每小時** 並被指派給作業角色， **計畫收入** 是乘以 **計畫小時數** 按任務角色的計費率計算的任務。

* 此 **計畫小時數** 均分 **持續時間** 任務。

* 此 **持續時間** 是 **計劃開始** **日期** 和 **計畫完成日期** 任務。 因為&#x200B;**計劃開始日期** 和 **計畫完成日期** 視檢視任務的使用者的時區而定，這些任務的「每天計畫小時數」量可能會因兩個不同時區的兩個使用者而異。

* 如果任務職責的開單費率未更改，或者只有一個開單費率改寫時，每日計畫小時數的金額不會更改項目的計畫收入。 在此情況下，即使來自兩個不同時區的兩個使用者每天看見不同的計畫小時數，專案的整體計畫收入仍會在兩個使用者之間相同。

   但是，如果是多個計費率覆蓋，則整體 **計畫收入** 兩個不同時區的兩個使用者似乎不同專案，因為其依賴「每天計畫小時數」（兩個使用者可能不同）和計費率覆寫（當每個使用者在自己的時區中查看任務時，同一天可能不同）。

* 準確 **計畫收入** amount是使用者所檢視的時區，與您Workfront執行個體的時區相同。 您的Workfront管理員會在「系統客戶資訊」區域中定義Workfront時區。\
   如需定義系統時區的詳細資訊，請參閱文章 [配置系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 計算不同時區中使用者的實際收入 {#calculate-actual-revenue-for-users-in-different-time-zones}

計算不同時區使用者的實際收入時，請考量下列事項：

* 當 **收入類型** 是 **角色每小時**, Workfront **實際小時數** 任務，其任務職責的開單費率分配給任務以計算 **實際收入**. 實際小時數直接記錄到任務中。

* 若是多個計費費率覆寫，Workfront會使用時間範圍符合 **參加日期** 記錄的任務小時數以計算 **實際收入**.

* 因為 **參加日期** 記錄小時數，且多個計費率覆寫的日期範圍上沒有時間戳記， **實際收入** 計算不受與使用者相關聯的時區影響。

有關用於計算的作業角色的詳細資訊 **實際收入**，請參閱文章的「了解根據使用者和角色指派的任務的收入計算」一節 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 重新計算項目財務

財務會在項目記錄的時數中發生更改時，在項目上計算。

如果在項目的使用期間更改了費率，則您可以使用項目上的「重新計算財務」選項，人工重新計算項目的成本和收入。 此外，有些動作會觸發自動重新計算。

有關重新計算項目財務的詳細資訊，請參閱文章 [重新計算項目財務](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## 使用API新增計費率

若要使用API為工作角色新增計費率，請執行 *setRatesForRole* 針對 **比率** 物件使用 *PUT方法*.
上的動作和日期欄位 **比率** 對象在API 8.0版中可用。如果已為項目上的職務職責定義了多個計費費率，並且您想要為該費率添加新的日期範圍，則必須將現有費率和要添加到同一API調用中的費率都包含在內。 這類似於更新對象上集合的方式。

以下是範例，其中 **可附加ID** 是 **專案ID** 的 **角色ID** 是 **作業角色ID** 您要為其添加新的計費率。<pre>{</pre><pre>&quot;acchapleID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;acceptableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         { &quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         { &quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>如需使用Workfront API的詳細資訊，請參閱文章 [API基本介紹](https://experience.workfront.com/s/article/API-Basics-638808549).
