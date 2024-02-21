---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2專案增強功能
description: 本頁說明2020.2版對生產環境所做的所有專案增強功能。 這些增強功能已在2020年5月11日當週的生產環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 2020.2專案增強功能

本頁說明2020.2版對生產環境所做的所有專案增強功能。 這些增強功能已在2020年5月11日當週的生產環境中推出。

如需2020.2版所有可用變更的清單，請參閱 [2020.2版本總覽](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## 對於Workfront管理員：當新專案的專案狀態為隱藏或未鎖定時，新增故障保護

在「設定」中，您可以設定偏好設定，以確保建立專案時，每個新專案都具有特定狀態。 這很重要，因為專案總是需要狀態才能在Workfront中正常運作，即使專案是全新專案。

為了確保新專案總是有狀態，即使管理員隱藏或解鎖為新專案設定的狀態，系統現在會將「狀態」清單中的第一個狀態指派給所有新專案，直到您再次為新專案設定新狀態為止。

如需有關設定所有新專案狀態偏好設定的資訊，請參閱 [設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (或如果您使用Adobe Workfront Classic，請參閱 [設定專案偏好設定](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298))。

**適用於下列環境：**

* Adobe Workfront Classic
* 全新Adobe Workfront體驗

## Workfront管理員：改良專案偏好設定中的設計

設定專案偏好設定的體驗現在更直覺且易於使用：

* 標題比選項標籤大，可以更快找到您要找的內容。
* 將線條和額外的空格分隔每個區段，讓您更輕鬆地專注於正在執行的動作。
* 如果您輸入無效數字給選項，例如「每工作日一般時數」，警告訊息會立即出現，而不是在您按一下「儲存」後出現。
* 選項標籤會比對Workfront中其他位置的對應介面文字，例如詳細資訊區域和報表。

如需「專案偏好設定」區域的詳細資訊，請參閱 [設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (或如果您使用Adobe Workfront Classic，請參閱 [設定專案偏好設定](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298))。

**適用於下列環境：**

* Adobe Workfront Classic
* 全新Adobe Workfront體驗

## 選定的篩選器、檢視和分組保留在報告清單中

現在，即使使用者登出並返回Workfront，也會選取套用至特定報告的最後一個篩選、檢視或分組。

先前，當使用者將篩選、檢視或分組套用至報告清單，然後導覽離開該頁面後，預設的篩選、檢視或分組會在使用者下次導覽至該同一報告時顯示。

**適用於下列環境：**

* 全新Adobe Workfront體驗
* Adobe Workfront Classic

## 當任務符合專案的時間表時，將任務移動並複製到另一個專案會保留任務限制

當您將任務複製或移動到其他專案時，Workfront處理任務的特定日期任務限制的方式已得到改進。 特定日期的工作限制範例包括「必須開始於」、「必須完成於」、「固定日期」、「開始不得晚於」等。

例如，當您將具有「必須開始於」限制的任務移動或複製到其「計劃開始日期」早於任務的「開始日期」的另一個專案時，任務會在複製或移動後保留該限制。 當您將具有必須開始日期限制的任務移動或複製到其計劃開始日期在任務開始日期之後的專案時，任務限制會儘快變更為。

在此變更之前，任務限制一律會儘快變更為。

有關移動任務的資訊，請參閱， [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md) (或如果您使用Adobe Workfront Classic，請參閱 [移動任務](https://one.workfront.com/s/article/Moving-Tasks-2081996259))。

如需有關複製工作的資訊，請參閱 [複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (或如果您使用Adobe Workfront Classic，請參閱 [複製和複製任務](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605))。

如需所有任務限制的概觀，請參閱 [任務限制總覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (或如果您使用Adobe Workfront Classic，請參閱 [任務限制總覽](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848))。

**適用於下列環境：**

* Adobe Workfront Classic
* 全新Adobe Workfront體驗

## 在詳細資訊標籤或工作清單中進行變更時防止資料遺失

為了防止當您在手動儲存變更時，在專案層級更新物件或任務清單中任務的詳細資訊頁面上的資訊時遺失資料，現在會顯示警告訊息，在您嘗試編輯標題中的資訊之前，通知您尚未儲存變更。 在儲存變更之前，只允許訂閱物件或將物件加入您的最愛。

如需有關編輯清單中工作的資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**適用於下列環境：**

* 全新Adobe Workfront體驗

