---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案實際完成日期概要
description: Adobe Workfront中的專案、任務和問題有實際完成日期。 這是將專案、任務或問題標示為完成的日期。
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 專案實際完成日期概要

Adobe Workfront中的專案、任務和問題有實際完成日期。 這是將專案、任務或問題標示為完成的日期。

## 實際完成日期

實際完成日期代表工作完成的即時日期和時間。 當任務或問題標籤為完成或完成時，Workfront會自動將專案狀態的變更日期設定為任務或問題的實際完成日期。 如果該日期不能準確反映任務或問題實際完成的時間，則可以手動編輯實際完成日期。

例如，您可以將任務或問題標示為星期一完成，但您知道工作已在上個星期五完成。 將任務或問題標示為「完成」後，您就可以手動將任務或問題的實際完成日期更新為上個星期五的日期，以反映實際完成。

您無法手動編輯專案的實際完成日期，但可以手動變更專案狀態，以觸發對其實際完成日期的變更。

專案的「實際完成日期」設定方式如下：

* 透過手動更新專案狀態：如果專案的「完成模式」設為「手動」，而您手動將專案狀態變更為「完成」，這會觸發要更新至上次完成任務之日期與時間之專案的「實際完成日期」。
* 當專案的最後一項作業完成時，自動進行：如果專案的「完成模式」設定為「自動」，且您將最後一項作業標示為「完成」或更新最後一項作業的「實際完成日期」，專案的「實際完成日期」也會以該日期更新。

  如需有關設定專案完成模式的資訊，請參閱文章 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront使用專案任務中上次完成的實際完成日期作為整個專案的實際完成日期。

Workfront或群組管理員會決定Workfront使用今天的日期還是任務的規劃完成日期，或是當任務或問題設為完成或關閉時的問題日期。 有關設定任務和問題偏好設定的資訊，請參閱 [設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 尋找實際完成日期

實際完成日期位於Workfront的下列區域中：

* 專案、任務和問題詳細資訊區域
* 編輯專案、任務和問題方塊
* 作為系統更新的專案、任務和問題更新區域。
* 專案、任務或問題清單或報告。

如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
