---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1專案增強功能
description: 本頁說明2020.1版專案的所有增強功能。 這些增強功能目前可在「預覽」環境中取得，並將於2020年3月底或4月初在「生產」環境中取得。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 2020.1專案增強功能

本頁說明2020.1版專案的所有增強功能。 這些增強功能目前可在「預覽」環境中取得，並將於2020年3月底或4月初在「生產」環境中取得。

如需2020.1版所有可用變更的清單，請參閱 [2020.1版本總覽](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## 更輕鬆檢視在更新中被標籤的訪客

現在更容易檢視哪些使用者在更新中被標籤。 標籤的使用者名稱顯示為藍色，並連結至使用者設定檔。

已標籤的使用者也會列在註解方塊下。

在此增強功能之前，先前標籤的使用者未出現在「通知」方塊中。

如需詳細資訊，請參閱 [標籤其他人的更新](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## 在更新註解或回覆中包含並識別引號文字

當您輸入註解時，可以將註解的一部分標示為引號文字，以便將其與您自己的註解區分開來。 使用HTML編輯器中的Block Quote按鈕。

如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## 在更新註解或回覆中引用之前的註解

當您在更新對話串中註解時，您可以快速將先前註解的文字加入對話串中。 在您要報價的註解旁的「更多」功能表中，尋找「報價回覆」選項。

如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 其他風險資訊

為了協助您更清楚瞭解專案的風險，您現在可以看到風險輸入的人和時間以及專案上的更新時間。 您可以在風險檢視中及透過公用Workfront API存取此資訊。 這些欄位將隨API版本11提供，該版本隨2020.1生產環境發行。

如需Workfront的風險相關資訊，請參閱 [建立及編輯專案的風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## 新增至「基準線」與「基準線作業」的其他欄位

為了協助您更清楚瞭解專案的財務進度，您現在可以在「比較基準」或「比較基準任務」報表中包含其他成本與收入資訊。 其他財務資訊不會新增至您目前儲存的基準線，但會新增至新的基準線。

如需有關可從「比較基準」和「比較基準任務」物件存取的專案與任務財務欄位的資訊，請參閱 [專案基準線中包含的專案財務](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## 「已關閉未決核准」狀態的問題會視為未完成

Workfront處理「完成 — 未決核准」狀態中問題的方式已變更。 現在，這些問題會被視為未完成，在核准解決之前，專案不能標籤為完成。

在此變更之前，處於「已關閉 — 未決核准」狀態的問題被視為已關閉。

在此變更前已設定為「已關閉 — 未決核准」狀態的所有問題，其行為方式將與先前相同，即視為已完成，並允許專案完成。 進行此變更後，置於此狀態的所有問題都將被視為未完成。

如需有關專案狀態的資訊，請參閱 [存取系統專案狀態清單](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

