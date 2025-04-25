---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2其他增強功能
description: 本頁說明2020.2版本對生產環境的所有其他增強功能。 這些增強功能已在2020年5月11日當週的生產環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2其他增強功能

本頁說明2020.2版本對生產環境的所有其他增強功能。 這些增強功能已在2020年5月11日當週的生產環境中推出。

如需2020.2版所有可用變更的清單，請參閱[2020.2版總覽](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md)。

## Workfront管理員：新的Workfront Classic體驗現在提供在Workfront Classic中建立的較新版面範本

新的Workfront體驗現在提供2019年秋季之後在Workfront Classic中建立的版面範本。 建議您更新新Workfront體驗中的這些版面配置範本，以運用新功能，並讓這些範本對該環境中的使用者儘可能有用。

如需詳細資訊，請參閱[配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)。

**在以下環境中可用：**

* 全新Adobe Workfront體驗

## 群組特定的核准流程適用於所有物件

若要充分利用群組特定的核准流程，您現在可以在編輯這些物件時，將其新增至任務、問題和專案。

在專案上設定請求佇列或佇列主題時，您也可以自動將群組特定的核准流程附加至「編輯專案」方塊的「任務」區域中的任務以及問題。

如需有關新增核准流程至專案、任務和問題的資訊，請參閱下列文章：

* [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)
* [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md)
* [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## 使用自訂狀態建立群組的核准流程

為了更方便群組管理自己的獨特工作流程，您現在可以在核准流程中使用群組特定的自訂狀態。

過去，群組無法透過其群組特定的核准程式使用自己的自訂狀態。 僅系統範圍狀態可供使用，且這些狀態並不一定適合群組核准流程。

自訂狀態現在可用於單次使用和全系統核准流程：

* 為物件（專案、任務或問題）建立單次使用的核准流程，並以與使用該物件的群組相關聯的狀態為基礎。 這包括任何與群組相關聯的自訂狀態。
* 建立全域核准流程，並僅供群組或系統中的所有人使用。

對於具有核准程式之管理存取權的使用者，有關設定核准程式的資訊可在[建立工作專案的核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)中取得(或者如果您使用Adobe Workfront Classic，請參閱[建立核准程式](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

使用者可在[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (或如果您使用Adobe Workfront Classic，請參閱[將新的或現有的核准程式與工作建立關聯](https://experienceleague.adobe.com/en/docs/workfront/using/home))中取得有關將核准程式與工作專案建立關聯的資訊。

**在以下環境中可用：**

* Adobe Workfront Classic
* 全新Adobe Workfront體驗

## 搜尋的新覆蓋頁面

為了讓使用者在新的Workfront體驗中更輕鬆地在搜尋頁面和先前的頁面之間來回導覽，我們新增了搜尋覆蓋頁面，該頁面部分涵蓋了畫面。

現在，當您按一下「搜尋」功能表中的「進階搜尋」或執行基本搜尋時，頁面幻燈片會從畫面右側開啟。

如需詳細資訊，請參閱[搜尋Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md)。

**在以下環境中可用：**

* 全新Adobe Workfront體驗

## 事件訂閱的更新

為了更方便讓使用者進行分級、疑難排解及解決問題，我們已修改行為，並將更多資料新增至事件訂閱API。 我們也進行了以下變更：

* 已移轉基礎傳訊技術
* 重新建立服務，減少複雜的相依性，進而提高擴充效率
* 改善監視和警報

若要深入瞭解，請參閱[常見問題集 — 活動訂閱](../../../wf-api/general/event-subs-faq.md)與[活動訂閱最佳實務](../../../wf-api/general/event-sub-best-practice.md)。
