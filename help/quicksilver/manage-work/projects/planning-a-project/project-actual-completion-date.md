---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 項目實際完成日期概覽
description: 專案、任務和問題在Adobe Workfront中有實際完成日期。 這是項目、任務或問題標籤為完成的日期。
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: 3a3dc541219706e3f6a4700889db344c110838bb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 項目實際完成日期概覽

專案、任務和問題在Adobe Workfront中有實際完成日期。 這是項目、任務或問題標籤為完成的日期。

## 實際完成日期

實際完成日期表示完成工作的即時日期和時間。 當任務或問題標籤為「完成」或「完成」時，Workfront會自動將項目狀態更改的日期設定為任務或問題的實際完成日期。 如果該日期不能準確反映任務或問題實際完成的時間，則您可以手動編輯實際完成日期。

例如，您可以將任務或問題標籤為「星期一完成」，但您知道工作已在上個星期五完成。 將任務或問題標籤為「完成」後，您可以手動將任務或問題的實際完成日期更新為上星期五的日期，以反映實際完成。

您不能手動編輯項目的實際完成日期，但可以手動更改項目的狀態，以觸發對其實際完成日期的更改。

項目的實際完成日期設定方式如下：

* 手動更新專案的狀態：如果項目的「完成模式」設定為「手動」，並且您手動將項目狀態更改為「完成」，則這會觸發在更改狀態時將項目的實際完成日期更新為日期和時間。
* 當項目的最後一個任務完成時，自動：如果項目的「完成模式」設定為「自動」，並且您將最後一個任務標籤為「完成」或更新最後一個任務的「實際完成日期」，則項目的「實際完成日期」也會隨該日期更新。

   有關設定項目的「完成模式」的資訊，請參閱文章 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!NOTE]
   >
   >Workfront將項目任務的實際完成日期（最後完成）用作整個項目的實際完成日期。

Workfront或群組管理員會判斷Workfront是否使用今天的日期或任務的計畫完成日期，或是當這些設為「完成」或「關閉」時的問題。 有關設定任務和問題首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 查找實際完成日期

實際完成日期位於Workfront的以下區域：

* 項目、任務和問題詳細資訊區域
* 編輯項目、任務和問題框
* 項目、任務和問題更新區域作為系統更新。
* 項目、任務或問題清單或報告。

如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
