---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe Workfront和Microsoft專案中的期間型別
description: Adobe Workfront中可用的期間型別與Microsoft專案中稱為任務型別的對應期間型別不同。 在Workfront和Microsoft專案之間匯出或匯入專案時，這有時可能會令人困惑。
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 2%

---

# Adobe Workfront和Microsoft專案中的期間型別

Adobe Workfront中可用的期間型別與Microsoft專案中稱為任務型別的對應期間型別不同。 在Workfront和Microsoft專案之間匯出或匯入專案時，這有時可能會令人困惑。

如需有關在Workfront和Microsoft專案之間匯入和匯出專案的資訊，請參閱下列文章：

* [將專案匯出至Microsoft專案](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [從Microsoft專案匯入專案](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Workfront和Microsoft專案中的期間型別

Workfront有四種任務期間型別：

* 簡單
* 投入比導向
* 已計算的工作
* 已計算的任務指派

如需詳細資訊，請參閱[任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

Microsoft專案無法辨識這些期間型別。 目前，Microsoft專案有三個與Workfront中的期間型別類似的任務型別：

* 固定單位
* 固定工時
* 固定期間

## 從Workfront匯出至MS Project時期間型別變更

將專案從Workfront匯出至Microsoft專案時，投入比導向的任務會變成「固定工作」。 簡單、已計算的工作和已計算的指派會變成固定單位。

## 從MS Project匯入至Workfront時期間型別變更

從Microsoft專案匯入到Workfront時，固定單位會變成投入比導向。 「固定工時」和「固定期間」會收到Workfront管理員為您的系統選取的預設期間型別。 如需詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
 
(drafting this because it is misleading)
 
</note>
-->
