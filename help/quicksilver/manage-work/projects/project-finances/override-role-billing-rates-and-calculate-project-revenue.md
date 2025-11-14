---
product-area: projects
navigation-topic: financials
title: 覆寫工作角色帳單費率與計算專案收入的概要
description: 當您將記帳費率乘以專案所花費的時數時，您可以使用記帳費率來計算專案的收入。 如需有關收費率和收入的詳細資訊，請參閱文章帳單和收入概觀。
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '3859'
ht-degree: 0%

---

# 覆寫工作角色帳單費率與計算專案收入的概要

{{highlighted-preview}}

當您將記帳費率乘以專案所花費的時數時，您可以使用記帳費率來計算專案的收入。 如需有關記帳費率和收入的詳細資訊，請參閱文章[記帳和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)。

## 職務角色帳單費率與角色每小時收入型態概要

身為Adobe Workfront管理員，您可以將收費率與使用者和職位角色建立關聯。\
如需有關建立使用者以及將使用者與計費率建立關聯的詳細資訊，請參閱文章[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。 如需有關建立工作角色並將其與收費率關聯的詳細資訊，請參閱文章[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

無法覆寫與使用者相關的收費率。

與工作角色相關的收費率可在公司或專案層級覆寫。

若要根據工作角色的收費率來計算專案的收入，專案上任務的&#x200B;**收入型別**&#x200B;必須是下列其中一項：

* 角色每小時
* 受限角色小時
* 角色小時加固定

如需&#x200B;**收入型別**&#x200B;和記帳費率的詳細資訊，請參閱[記帳與收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)。

## 計算收入時帳單費率覆寫的階層

職務角色可以透過下列方式與其產生相關的收費率：

* 身為Workfront管理員，您可以在建立工作角色時，定義與工作角色相關聯的系統層級收費率。\
  如需有關建立工作角色的詳細資訊，請參閱[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

* 身為Workfront管理員，您可以在建立公司時，為相同職務角色定義公司層級的收費率。\
  當Workfront計算與此公司相關聯的專案收入時，當角色指派給任務時使用公司收費率，而不是此職務角色的系統層級收費率。\
  在公司層級變更的工作角色費率將影響與該公司相關聯的所有專案。

  >[!NOTE]
  >
  >如果您需要更新公司收費率，專案費率不會自動更新。 您必須先從專案中移除公司、更新公司的費率，然後將公司重新附加至專案，新公司費率才會對專案生效。 如需將公司附加到專案的指示，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

  如需有關建立公司特定工作角色收費率的詳細資訊，請參閱[建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

* 身為Workfront管理員，您可以在編輯專案時啟用選項，以在使用者手動重新計算專案財務時，將變更套用至專案的公司層級收費率。\
  如需詳細資訊，請參閱[以公司層級的收費率覆寫專案層級的收費率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)。

<div class="preview">

* 身為Workfront管理員，您可以根據位置與日期，定義每個角色有多個收費率的費率卡。 將費率卡附加到專案時，所有角色（如果使用位置，則按位置）及其關聯的計費費率會新增到專案的計費費率區段。 附加費率卡會覆寫專案上任何現有的收費率。

  如需詳細資訊，請參閱[管理費率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)和[將費率卡附加至專案](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)。

</div>

* 身為專案經理，您可以在專案層次為相同職務角色定義收費率。\
  專案上工作角色費率的變更只會影響該專案。

  如需有關覆寫專案角色費率的資訊，請參閱專案層級[的](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)覆寫工作角色收費率。

>[!IMPORTANT]
>
>如果工作角色在系統層級、公司層級和專案層級與計費率相關聯，Workfront會在使用工作角色費率時，使用專案層級的工作角色的計費率來計算任務的收入。 來自所有任務的收入將累計至專案的收入。

## 覆寫專案層級的工作角色收費率

身為專案經理，您可以指定特定專案上工作角色的收費率。 此專案層級的收費率會覆寫此工作角色之系統層級的收費率。 Workfront使用工作角色的專案層級收費率來計算收入，而不使用系統層級收費率。

<span class="preview">您也可以在專案中附加費率卡，這會從費率卡將工作角色收費率匯入專案。</span>

若要瞭解如何在專案層級覆寫工作角色收費率，請參閱[在專案層級覆寫工作角色收費率](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)。

如需有關哪一個工作角色用於計算專案收入的詳細資訊，請參閱[帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的「根據使用者和角色指派的任務收入計算」一節。 <span class="preview">如需有關將費率卡附加至專案的資訊，請參閱[將費率卡附加至專案](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)。</span>

>[!NOTE]
>
>在實際收入中，套用至新增至標示為已記帳之記帳記錄時數的記帳費率，不應受記帳記錄記帳後發生的記帳費率覆寫影響。

## 專案的「收費率」區段概要

在您指定與專案相關之職務角色的覆寫收費率後，即可在專案的&#x200B;**收費率**&#x200B;索引標籤中看到所有職務角色及其覆寫。

請注意&#x200B;**記帳費率**&#x200B;清單中的下列資訊：

* [工作角色群組](#job-role-grouping)
* [專案收費率值](#project-billing-rate-value)
* [預設收費率值](#default-billing-rate-value)
* [公司收費率值](#company-billing-rate-value)
* [多個收費率值和時間範圍](#multiple-billing-rate-values-and-timeframes)

### 職務角色群組 {#job-role-grouping}

記帳費率在&#x200B;**記帳費率**&#x200B;區域中依其各自的工作角色分組。 <span class="preview">如果專案附有評等卡，則職位角色也會依評等卡分組。 如果將位置套用至工作角色，則會將位置名稱納入工作角色名稱中。 您可以為多個位置列出相同的工作角色。</span>

### 專案收費率值 {#project-billing-rate-value}

在與工作角色相對應的群組行中，在&#x200B;**專案收費率**&#x200B;欄位中的專案層級，注意該工作角色的收費率。 如果工作角色有多個覆寫費率，則與目前日期對應的覆寫費率會顯示在&#x200B;**專案收費率**&#x200B;欄的群組明細行中。

### 預設收費率值 {#default-billing-rate-value}

在工作角色的分組明細行中，在&#x200B;**預設收費率**&#x200B;欄位中，注意系統層級該工作角色的收費率。

>[!NOTE]
>
>如果工作角色有專案收費率，**預設收費率**&#x200B;絕不會套用於計算專案的收入。 只套用&#x200B;**專案收費率**&#x200B;來計算收入。

### 公司收費率值 {#company-billing-rate-value}

在工作角色的分組明細行中，在&#x200B;**公司收費率**&#x200B;欄位中，注意該工作角色在公司層級的收費率。 這表示有一個公司與此專案相關聯，而且此工作角色對該公司有不同的收費率。 公司的收費率會顯示，即使它與專案費率相同。

>[!NOTE]
>
><span class="preview">將費率卡附加至專案時，**公司收費率**&#x200B;不會匯入收費率。 計算是以職務角色的費率卡費率或公司費率為基礎。</span>
>
>如果工作角色有專案收費率，**公司收費率**&#x200B;絕不會套用於計算專案的收入。 只套用&#x200B;**專案收費率**&#x200B;來計算收入。

### 多個收費率值和時間範圍 {#multiple-billing-rate-values-and-timeframes}

如果您有多個覆寫特定工作角色的收費率，則會列在該工作角色的群組下方。 使用內嵌編輯，您可以在此標籤上變更覆寫收費率的&#x200B;**開始** **日期**&#x200B;和&#x200B;**結束日期**&#x200B;的覆寫收費率。

>[!NOTE]
>
>您不能為第一個覆寫率指定&#x200B;**開始日期**，也不能為最後一個覆寫率指定&#x200B;**結束日期**。 Workfront假設第一個覆寫率適用於日期早於第一個覆寫的&#x200B;**結束日期**&#x200B;的所有時數，而最後一個覆寫率適用於日期晚於最後一個覆寫的&#x200B;**開始日期**&#x200B;的所有時數。\
>如果在專案的計劃開始日期之前記錄了一小時，則使用第一個收費率。\
>如果是在專案的計畫完成日期後記錄一小時，則會使用最後一個收費率。

## 計算計畫收入

* [根據一次性記帳費率覆寫計算計畫收入](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [根據多個記帳費率覆寫計算計畫收入](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [在任務期間中的計畫時數分佈](#distribution-of-planned-hours-across-the-duration-of-a-task)

### 根據一次性記帳費率覆寫計算計畫收入 {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

根據一次性「收費率」覆寫計算「計畫收入」時，請考量下列事項：

* 當任務的&#x200B;**收入型別**&#x200B;是&#x200B;**每小時角色數**&#x200B;時，Workfront會將任務的計畫時數乘以與任務相關聯之工作角色的計費率，以計算任務的計畫收入。

* 在專案層級覆寫工作角色的計費費率時，Workfront會使用專案的覆寫費率來計算計畫收入。
* 當任務有多個指派時，計畫收入的計算方式為將每個指派的工作角色及其各自計畫時數配置的計費率相乘。

>[!NOTE]
>
>在多個指派的情況下，每個指派的計畫時數與任務的計畫時數不同。

如需有關使用哪個工作角色來計算計畫收入的詳細資訊，請參閱文章[帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的「瞭解根據使用者和角色指派的任務收入計算」一節。

### 根據多重記帳費率覆寫計算計畫收入 {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

根據多重記帳費率覆寫來計算計畫收入時，請考量下列事項：

* 當任務的&#x200B;**收入型別**&#x200B;是&#x200B;**每小時角色數**&#x200B;時，Workfront會將任務的計畫時數乘以與任務相關聯之工作角色的計費率，以計算任務的計畫收入。

  如需有關使用哪個工作角色來計算計畫收入的詳細資訊，請參閱文章[帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的「瞭解根據使用者和角色指派的任務收入計算」一節。

* 如果覆寫了多個帳單費率，則計畫時數在任務持續期間所乘以的費率會變更。 依預設，Workfront會將計畫時數平均分配至任務的持續期間，並為任務的每天分配相等的時數。 計算任務的&#x200B;**計畫收入**&#x200B;時，Workfront會將每日計畫時數乘以當天的收費率。 若是多個收費率，該費率每天可能都不相同。

  例如，您有一個任務具有角色每小時&#x200B;**收入型別**。 該任務的工期為5天，而計畫時數的值為40小時。 每日計畫時數為8小時。 將「專案經理」工作角色指派給作業，並覆寫此工作角色在作業最後3天的收費率，因此您會擁有此工作角色在前兩天的費率1收費率，以及剩餘3天的費率2收費率。

  計算此任務之&#x200B;**計畫收入**&#x200B;的公式為：

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

如需在Workfront中尋找每日計畫時數數量的詳細資訊，請參閱本文章的[工作期間中計畫時數的分佈](#distribution-of-planned-hours-across-the-duration-of-a-task)一節。

>[!NOTE]
>
>如果任務有多個受指派人，計畫時數會先分配給每個受指派人，然後在任務持續期間分配給每一天。 在此情況下，計畫收入的計算將考量每個受指派人的每日時數金額，以及每個職務角色的計費率，若有多個計費率，則會在任務持續期間變更。

### 在任務期間中的計畫時數分佈 {#distribution-of-planned-hours-across-the-duration-of-a-task}

瞭解任務期間中計畫時數的分佈時，請考慮下列事項：

* 依預設，Workfront會根據專案排程的可用性，將計畫時數平均分配至任務的整個期間，並為任務的每一天分配相等的計畫時數。

  如需瞭解跨任務期間之計畫時數分佈的詳細資訊，請參閱文章[計畫時數概觀](../../../manage-work/tasks/task-information/planned-hours.md)中的「瞭解跨任務期間之計畫時數分佈」一節。

  >[!NOTE]
  >
  >每日計畫時數是任務期間每天的計畫時數配置。 如果任務有一個指派，則此數字也代表每個指派的每日計畫時數。 如果任務有多個指派，則每個指派的每日計畫時數與任務的每日計畫時數不同。 對於具有多個指派的任務，Workfront中沒有每日計畫時數每個指派的視覺化表示法。
  >
  >
  >每日計畫時數乘以當天指派給任務之工作角色的收費率，即可計算該任務的每日計畫收入。 以這種方式計算的所有每日計畫收入的總和等於該任務的計畫收入。

## 計算實際收入

* [根據一次性收費率覆寫計算實際收入](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [根據多重記帳費率覆寫計算實際收入](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### 根據一次性記帳費率覆寫計算實際收入 {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

根據一次性「收費率」覆寫計算「實際收入」時，請考量下列事項：

* 當任務的&#x200B;**收入型別**&#x200B;是&#x200B;**每小時角色數**&#x200B;時，Workfront會將任務的&#x200B;**實際小時數**&#x200B;乘以與任務相關聯之工作角色的收費率，以計算任務的&#x200B;**實際收入**。 實際時數是直接記錄至工作的時數。

  如需有關使用哪個工作角色來計算&#x200B;**實際收入**&#x200B;的詳細資訊，請參閱文章[帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的「瞭解根據使用者和角色指派的任務收入計算」一節。

* 如果在專案層次已覆寫工作角色的收費率，Workfront會使用專案的覆寫費率來計算實際收入。 當您覆寫專案上工作角色的收費率時，將會使用新調整後的費率自動重新計算專案的&#x200B;**實際收入**。

  如需有關覆寫專案角色費率的資訊，請參閱專案層級[的](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)覆寫工作角色收費率。

>[!NOTE]
>
>如果您想要保留在覆寫以原始費率記帳的原始記帳費率之前已登入專案的時數，您必須將其納入&#x200B;**記帳記錄**，並且您必須將&#x200B;**記帳記錄**&#x200B;標籤為&#x200B;**已記帳**。 否則，在覆寫專案的記帳費率之前記錄的時數的&#x200B;**實際收入**&#x200B;將在重新計算專案的財務時使用新的費率重新計算。\
>如需在付費記錄中包含時數並標示為&#x200B;**已記帳**&#x200B;的詳細資訊，請參閱文章[建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md)。

### 根據多重記帳費率覆寫計算實際收入 {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

根據多重記帳費率覆寫來計算實際收入時，請考量下列事項：

* 當任務的&#x200B;**收入型別**&#x200B;是&#x200B;**每小時**&#x200B;角色時，Workfront會將任務的&#x200B;**實際時數**&#x200B;乘以指派給任務之工作角色的收費率，以計算任務的&#x200B;**實際收入**。 實際時數是直接記錄至工作的時數。

* 如果覆寫了多個收費率，**實際時數**&#x200B;乘以計算&#x200B;**實際收入**&#x200B;的費率可能會在工作期間變更。 Workfront使用時間範圍符合任務所記錄時數之&#x200B;**輸入日期**&#x200B;的工作角色的收費率來計算&#x200B;**實際收入。**

  例如，任務具有&#x200B;**收入型別** （每小時&#x200B;**角色**），且已指派給專案經理的工作角色。 以1的費率覆寫此職務角色在6月19日至6月25日之間的收費率。 從6月26日開始，使用費率2覆寫收費率。 6月20日記錄2小時，6月28日記錄3小時。

  Workfront使用下列公式計算此任務的&#x200B;**實際收入**：

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  如需有關使用哪個工作角色來計算&#x200B;**實際收入**&#x200B;的詳細資訊，請參閱文章[帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的「瞭解根據使用者和角色指派的任務收入計算」一節。

## 根據多個收費率計算收入時時區的影響

使用者與Workfront中的其他實體之間若發生時區差異，可看見與其他使用者不同的每日計畫時數。 以下情形可能會將使用者的每日計畫時數資訊與其他使用者看到的資訊有所偏差：

* 兩個使用者可能將其電腦設定為兩個不同的時區
* Workfront中的兩個使用者設定檔可能設定為兩個不同的時區
* 與使用者設定檔相關聯的時區可能與Workfront中的系統時區不同
* 與使用者設定檔相關聯的時區可能與專案排程的時區不同。

在這些情況下，兩個不同時區設定相同的使用者之間，每天的計畫時數可能會不同。 在專案上使用多個收費率覆寫時，他們也會看到不同的計畫收入數字。

* [計算不同時區使用者的計畫收入](#calculate-planned-revenue-for-users-in-different-time-zones)
* [計算不同時區使用者的實際收入](#calculate-actual-revenue-for-users-in-different-time-zones)

### 計算不同時區使用者的計畫收入 {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>如果您讓不同時區的使用者處理相同的專案，我們建議您不要在該周變更專案的計費率覆寫。 這麼做可能會因為使用者排程的時區與Workfront系統時區之間的時區差異，而顯示錯誤的專案計畫收入金額。 大多數排程都允許將週末排除在計畫時數計算之外。 如果工作角色的計費率覆寫發生變更，最好在週末進行，而不是在周中進行，因為這可能與任務期間的中間時間一致。

計算不同時區之使用者的計畫收入時，請考慮下列各項：

* 對於具有&#x200B;**收入型別** （每小時&#x200B;**個角色**）並指派給工作角色的工作，**計畫收入**&#x200B;的計算方式為將任務的&#x200B;**計畫時數**&#x200B;乘以工作角色的計費率。

* **計畫時數**&#x200B;平均分佈於任務的&#x200B;**期間**。

* **期間**&#x200B;是介於任務的&#x200B;**計劃開始** **日期**&#x200B;和&#x200B;**計畫完成日期**&#x200B;之間的時段。 由於任務的&#x200B;**計劃開始日期**&#x200B;和&#x200B;**計畫完成日期**&#x200B;會根據檢視任務之使用者的時區而有所不同，因此兩個使用者在兩個不同時區的每日計畫時數可能會不同。

* 若未變更工作角色的計費率或僅有一個計費率覆寫，每日計畫時數金額不會變更專案的計畫收入。 在此案例中，即使來自兩個不同時區的兩個使用者每天看到不同的規劃時數，兩個使用者之間的專案整體規劃收入仍相同。

  但是，若是多重計費率覆寫，則兩個不同時區的兩個使用者可能會覺得專案的整體&#x200B;**計畫收入**&#x200B;不同，因為它有賴於每日計畫時數的數量（兩個使用者可能不同）和計費率覆寫（當每個使用者在自己的時區中檢視任務時，當天可能會不同）。

* 準確的&#x200B;**計畫收入**&#x200B;金額是與Workfront執行個體時區具有相同時區的使用者看到的金額。 您的Workfront管理員會在系統客戶資訊區域中定義Workfront時區。\
  如需定義系統時區的詳細資訊，請參閱文章[設定系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

### 計算不同時區使用者的實際收入 {#calculate-actual-revenue-for-users-in-different-time-zones}

計算不同時區使用者的實際收入時，請考慮下列事項：

* 當任務的&#x200B;**收入型別**&#x200B;是&#x200B;**每小時**&#x200B;角色時，Workfront會將任務的&#x200B;**實際時數**&#x200B;乘以指派給任務之工作角色的收費率，以計算&#x200B;**實際收入**。 實際時數是直接記錄至工作的時數。

* 如果覆寫了多個收費率，Workfront會使用時間範圍符合任務所記錄時數之&#x200B;**輸入日期**&#x200B;的工作角色的收費率來計算&#x200B;**實際收入**。

* 由於在記錄時數的&#x200B;**輸入日期**&#x200B;沒有時間戳記，且多個收費率覆寫的日期範圍沒有時間戳記，因此&#x200B;**實際收入**&#x200B;計算不受與使用者相關聯的時區影響。

如需有關使用哪個工作角色來計算&#x200B;**實際收入**&#x200B;的詳細資訊，請參閱文章[帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的「瞭解根據使用者和角色指派的任務收入計算」一節。

## 重新計算專案財務

當專案記錄的時數發生變更時，會在專案上計算財務。

如果在專案存留期期間費率發生變更，您可以使用專案上的「重新計算財務」選項，手動重新計算專案的成本和收入。 此外，某些動作會觸發自動重新計算。

如需重新計算專案財務的詳細資訊，請參閱文章[重新計算專案財務](../../../manage-work/projects/project-finances/recalculate-project-finances.md)。

## 使用API新增收費率

若要使用API為工作角色新增收費率，請使用&#x200B;*PUT方法*&#x200B;為&#x200B;**Rate**&#x200B;物件執行&#x200B;*setRatesForRole*動作。
**Rate**物件上的動作和日期欄位可在API 8.0版中使用。
如果您已為專案中的工作角色定義了數個收費率，並且想要使用新的日期範圍為其新增收費率，則必須在同一API呼叫中同時包含現有收費率和要新增的收費率。 這類似於更新物件上的集合的方式。

下列API呼叫的範例中，**attachableID**&#x200B;是您新增收費率之專案的&#x200B;**專案識別碼**，**RoleID**&#x200B;是您新增收費率的&#x200B;**工作角色識別碼**。<pre>{</pre><pre>&quot;attachableID&quot;：&quot;593f01500000557d75fdd4fdfcc624f2&quot;，</pre><pre>&quot;attachableObjCode&quot;：&quot;PROJ&quot;，</pre><pre>&quot;roleID&quot;：&quot;544820df000014148cda5136d4b79d09&quot;， </pre><pre>&quot;rates&quot;：[</pre><pre>         {&quot;rateValue&quot;：&quot;0.00&quot;，&quot;startDate&quot;:null，&quot;endDate&quot;：&quot;2017-06-11&quot;}，</pre><pre>         {&quot;rateValue&quot;：&quot;45.00&quot;，&quot;startDate&quot;：&quot;2017-06-12&quot;，&quot;endDate&quot;：&quot;2017-06-17&quot;}，</pre><pre>         {&quot;rateValue&quot;：&quot;95.00&quot;，&quot;startDate&quot;：&quot;2017-06-21&quot;，&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>如需使用Workfront API的詳細資訊，請參閱文章[API基本知識](https://experience.workfront.com/s/article/API-Basics-638808549)。
