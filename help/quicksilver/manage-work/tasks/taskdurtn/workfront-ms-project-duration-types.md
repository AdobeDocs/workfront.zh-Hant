---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe Workfront和Microsoft專案中的期間類型
description: Adobe Workfront中可用的持續時間類型與Microsoft專案中相對應的「任務類型」不同。 在Workfront和Microsoft專案之間匯出或匯入專案時，有時會造成混淆。
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Adobe Workfront和Microsoft專案中的期間類型

Adobe Workfront中可用的持續時間類型與Microsoft專案中相對應的「任務類型」不同。 在Workfront和Microsoft專案之間匯出或匯入專案時，有時會造成混淆。

如需有關在Workfront和Microsoft專案之間匯入和匯出專案的資訊，請參閱下列文章：

* [將專案匯出至Microsoft專案](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [從Microsoft專案匯入專案](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Workfront和Microsoft專案中的期間類型

Workfront有四種工作期間類型：

* 簡單
* 投入比導向
* 已計算的工作
* 已計算的任務指派

如需詳細資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Microsoft專案無法辨識這些持續時間類型。 目前，Microsoft專案有三種類似Workfront中「持續時間類型」的任務類型：

* 固定件數
* 固定工作
* 固定持續時間

## 從Workfront匯出至MS專案時，持續時間類型會變更

將專案從Workfront匯出至Microsoft專案時，工作導向的工作會變成固定工作。 簡單、計算的工作和計算的分配變成固定單位。

## 從MS專案匯入Workfront時，持續時間類型會變更

將專案從Microsoft專案匯入Workfront時，「固定單位」會變成「工作驅動」。 「固定工作」和「固定持續時間」接收您的Workfront管理員為系統選取的預設持續時間類型。 如需詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
