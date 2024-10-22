---
product-area: projects
navigation-topic: issue-information
title: 問題計畫完成日期總覽
description: 問題的計畫完成日期是預期完成問題的日期。
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# 問題計畫完成日期總覽

問題的計畫完成日期是預期完成問題的日期。

您可以指定問題的規劃完成日期，或讓Adobe Workfront根據特定條件決定如何計算。

問題的計畫完成日期不會影響專案的計畫完成日期。 只有任務的計畫完成日期會影響專案的計畫完成日期。 如需有關專案計畫完成日期的詳細資訊，請參閱[設定專案計畫完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)。

>[!NOTE]
>
>問題的計畫完成日期與問題的認可日期或問題的預計完成日期有下列不同：
>
>* 認可日期是指派給問題的人員手動估計將完成問題的日期。 如需詳細資訊，請參閱下列文章：
>
>   * [認可日期總覽](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * 認可日期與計畫完成日期之間的[互動](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md)。
>
>* 「預計完成日期」是Workfront計算的日期，該日期會考慮外部因素，以確定實際完成問題的日期。 如需詳細資訊，請參閱[專案、任務和問題的預計完成日期總覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)。
>

## 手動設定問題的計畫完成日期

您必須擁有問題的編輯存取權和管理許可權，才能更新問題的規劃完成日期。

您可以在Workfront的下列區域中手動設定問題的規劃完成日期：

* 在「編輯問題」方塊中或在建立或編輯問題時在「問題詳細資訊」區域中。 如需詳細資訊，請參閱[編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md)。
* 若在檢視問題時顯示規劃完成日期，則位於首頁區域。 如需詳細資訊，請參閱[更新或編輯首頁區域的工作專案](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)。
* 在問題標題中。 如需詳細資訊，請參閱[新物件標頭](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)。
* 問題清單或報告中，規劃完成日期欄位何時顯示在檢視中。

  如需詳細資訊，請參閱[編輯清單](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md)中的問題。

## Workfront如何自動計算問題的規劃完成日期

當Workfront自動計算問題的規劃完成日期時，以下專案可能會影響日期：

* 規劃開始日期

  輸入日期和計劃開始日期應在您首次建立問題時與問題相符。

* 預設期間，如專案的佇列詳細資料區段中所設定。 如需詳細資訊，請參閱[建立要求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

  如果預設期間為0天，則計畫完成日期與問題的計劃開始日期匹配。

* 專案排程

自動設定時，「計畫完成日期」會根據下列計算方式決定：

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**範例：**&#x200B;例如，如果您的任務開始日期是1月14日（星期五），而預設期間是5天，則計畫完成日期是1月21日（星期五），如果專案排程是每日8小時的星期一至星期五。

存在下列情況：

* 如果專案沒有排程，則會考慮Workfront系統的預設排程。 如需詳細資訊，請參閱[排程總覽](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)。
* 如果排程是星期一至星期五上午9點至下午1點（一天4小時），且您的Workfront系統的每工作日一般時數為8小時，則計畫完成日期為1月27日。

>[!TIP]
>
>在計算「計畫完成日期」時，Workfront會考量如假日和週末等排程例外。


