---
product-area: projects
navigation-topic: issue-information
title: 發行計畫完成日期概覽
description: 發行的計畫完成日期是預計發行完成的日期。
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 發行計畫完成日期概覽

發行的計畫完成日期是預計發行完成的日期。

您可以指定問題的「計畫完成日期」，或根據特定標準，讓Adobe Workfront自行計算。 

問題的計畫完成日期不會影響項目的計畫完成日期。 只有任務的計畫完成日期會影響項目的計畫完成日期。 有關項目計畫完成日期的詳細資訊，請參閱 [設定項目計畫完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>問題的計畫完成日期與問題的提交日期或問題的預計完成日期不同，具體方式如下：
>
>* 「提交日期」是指派給問題的人員手動估計他們將完成問題的日期。 如需詳細資訊，請參閱下列文章：
   * [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [提交日期與計畫完成日期之間的交互](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* 預計完成日期是Workfront計算的日期，該日期考慮外部因素，以確定實際可完成問題的實際實際日期。 如需詳細資訊，請參閱 [項目、任務和問題的預計完成日期概覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## 人工設定問題的計畫完成日期

您必須擁有「編輯」問題存取權和「管理」問題權限，才能更新問題的「計畫完成日期」。

您可以在Workfront的下列區域中手動設定問題的計畫完成日期：

* 建立或編輯期刊時，在「編輯期刊」方塊或「期刊詳細資訊」區域中。 如需詳細資訊，請參閱 [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md).
* 在「首頁」區域中，如果查看問題時顯示了「計畫完成日期」。 如需詳細資訊，請參閱 [在「首頁」區域更新或編輯工作項](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* 在問題標題中。 如需詳細資訊，請參閱 [新物件標題](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* 在「計畫完成日期」欄位顯示在視圖中的問題清單或報告中。

   如需詳細資訊，請參閱 [編輯清單中的問題](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Workfront如何自動計算問題的計畫完成日期

當Workfront自動計算發行的計畫完成日期時，以下內容可能會影響日期：

* 計劃開始日期

   首次建立問題時，問題的登入日期和計劃開始日期應相符。

* 在項目的「隊列詳細資訊」部分中配置的「預設持續時間」。 如需詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   如果預設持續時間為0天，則計畫完成日期與問題的計畫起始日期匹配。

* 專案排程

自動設定後，計畫完成日期將根據以下計算確定： 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**範例：** 例如，如果任務的開始日期是1月14日星期五，而預設持續時間是5天，則計畫完成日期是1月21日星期五，如果項目計畫是星期一至星期五，每天8小時。

存在下列情況：

* 如果專案沒有排程，則會考慮Workfront系統的預設排程。 如需詳細資訊，請參閱 [排程概觀](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* 如果計畫是星期一至星期五上午9:00至下午1:00（每天4小時），而您的Workfront系統的每工作日一般小時數是8小時，則計畫完成日期是1月27日。

>[!TIP]
Workfront在計算計畫完成日期時，會考慮計畫例外（如節假日和週末）。

 
