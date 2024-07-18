---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta最終發行活動
description: 本頁說明2018.1 Beta最終版本預覽環境中最近可用的所有變更。 預覽環境已於2018年1月31日提供此功能。 它將在2018年3月的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 2018.1 Beta最終發行活動

本頁說明2018.1 Beta最終版本預覽環境中最近可用的所有變更。 預覽環境已於2018年1月31日提供此功能。 它將在2018年3月的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.1年度所有變更的清單，請參閱  [2018.1發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta最終版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;****

* [設定資源可用性與使用者配置，以根據使用者排程進行計算](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**所有使用者**

* [行動裝置增強功能](#mobile-enhancements)
* [Jira整合](#jira-integration)
* [更新至校訂檢視器名稱](#update-to-proofing-viewer-names)
* 從校訂生產環境同步到預覽時[變更為同步化步調](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [在資源規劃工具中達到2,000個料號限制時顯示警告訊息](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## 行動裝置增強功能 {#mobile-enhancements}

以下功能將於2018年3月初推出，供行動應用程式商店使用：

* 全新導覽：行動應用程式首頁經過重新設計。
* 行動首頁：我們行動應用程式也更新了新首頁功能。

iOS和Android平台均支援新功能。

## Jira整合 {#jira-integration}

您現在可以透過安裝和設定適用於Jira的Workfront附加元件將Jira問題連結至Workfront任務或問題。 透過這項整合，您的專案經理可以繼續在Workfront中工作，而您的開發工程師可以繼續在Jira中工作，同時他們的個別專案會透過Workfront與Jira的整合建立連結。

您可以透過這項整合來設定下列專案：

* 為Workfront指派建立觸發器，以在發生Jira問題時自動建立。
* 手動將Jira問題連結至先前已建立的Workfront任務或問題。
* 指定當其中一個應用程式中的其中一個專案更新後，應在連結專案上同步的欄位。

Workfront附加元件將適用於Jira的內部部署和隨選版本。 此附加元件免費且將於2018年3月初在Atlassian Marketplace中可供下載。

如需有關適用於Jira的Workfront附加元件的詳細資訊，包括下載連結，請參閱[搭配Jira使用Workfront。](https://support.workfront.com/hc/en-us/sections/115001130053)

## 校訂檢視器名稱的更新 {#update-to-proofing-viewer-names}

在整個Workfront系統中，HTML5型校訂檢視器和Flash型校訂檢視器的名稱已重新命名。 先前和更新的名稱如下： 

| **先前名稱** | **已更新名稱** |
|---|---|
| HTML5校訂檢視器 | 新校訂檢視器 |
| Flash校訂檢視器 | 舊版校訂檢視器 |

{style="table-layout:auto"}

 如需有關使用新校訂檢視器的詳細資訊，請參閱[在校訂檢視器中檢閱校訂。](https://support.workfront.com/hc/en-us/sections/115000275214)

## 設定資源可用性與使用者配置，以根據使用者排程進行計算 {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

Workfront管理員現在可以決定Workfront如何計算系統層級的資源可用性和使用者配置（考量時數及FTE可用性）。 Workfront管理員可設定要使用預設排程或使用者的排程來計算資源使用狀態和使用者配置。

此設定在排程資源時，會影響使用者在下列情況下的可用性：

* 允許Workfront自動指派資源時，如「在排程區域中手動指派未指派的任務和問題」所述。

* 顯示配置指標時，如「在排程區域中管理使用者配置」中所述。

如需詳細資訊，請參閱設定Workfront計算排程區域的資源時數和FTE可用性的方式。

>[!NOTE]
>
>已棄用資源排程工具，並已從Workfront的23.1版本中移除。 如需有關使用工作負載平衡器排程資源的資訊，請參閱[工作負載平衡器概覽](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。


## 從校訂生產環境同步至預覽時變更為同步化步調 {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>此變更將於2018年2月11日生效。

Workfront Proof生產環境中的資料現在每週都會同步至Workfront Proof預覽環境。

在此變更前，資料會每月從Workfront Proof生產環境同步到預覽環境，而來自Workfront生產環境的資料每週會同步到Workfront預覽環境。 在Workfront預覽環境中使用校訂功能時，這種差異會導致一些同步處理錯誤。 

如需詳細資訊，請參閱[預覽Sandbox測試環境 — Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md)。 

## 在資源規劃工具中達到2,000個料號限制時顯示警告訊息 {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

由於我們目前正在研究更永久的解決方案以改進資源規劃工具中的效能，我們針對您可以套用至資源規劃工具的每個檢視引入了2,000個專案的限制：

* 「使用者檢視」只會顯示2,000個指派
* 「專案檢視」只會顯示2,000個專案
* 「角色檢視」只會顯示2,000個角色

當資源規劃工具嘗試載入超過2,000個專案時，會顯示通知，提醒您只能顯示2,000個專案。

如需這些限制及其如何影響資源規劃工具的詳細資訊，請參閱[資源規劃工具顯示限制](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
