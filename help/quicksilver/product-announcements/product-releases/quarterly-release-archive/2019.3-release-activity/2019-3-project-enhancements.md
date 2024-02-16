---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3專案增強功能
description: 本頁說明2019.3版中專案增強功能的所有變更。 它在2019年8月19日當週的生產環境中可用。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 0%

---

# 2019.3專案增強功能

本頁說明2019.3版中專案增強功能的所有變更。 它在2019年8月19日當週的生產環境中可用。

如需2019.3年度所有變更的清單，請參閱 [2019.3版本活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## 變更自訂表單中欄位的顯示型別

現在您可以變更自訂表單中欄位的顯示型別。

例如，如果您已建立「核取方塊」欄位，則可將其變更為「下拉式清單」欄位或「選項按鈕」欄位。 這三種欄位顯示型別可以互換。

或者，如果您已建立「單行文字欄位」，您可以將其變更為「段落文字欄位」。 這兩種欄位顯示型別可以互換。

之前，若要變更自訂欄位的顯示型別，您必須建立新欄位並刪除舊欄位。 這需要傳輸資料，而這通常很耗時。

如需詳細資訊，請參閱 [建立或編輯自訂表單](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 在文章中 [建立或編輯自訂表單](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

>[!NOTE]
>
>預覽可用性： 2019年8月9日
>
>生產可用性： 2019年8月30日

## 建立休假行事曆和報告

您現在可以看到使用者的休假，以便進行更好的規劃和執行。 您也可以將新的休假報告和行事曆新增到您的儀表板，以即時檢視使用者可用性。

>[!NOTE]
>
>預覽可用性： 2019年8月9日
>
>生產可用性： 2019年8月30日

## 開啟篩選器現在會在問題清單中顯示更多結果

當您套用開啟篩選器至問題清單時，該清單包含下列問題：

* 處於「已關閉 — 未決核准」狀態
* 與解析物件相關聯

在此變更之前，套用「開啟」篩選器時，這些問題未包含在清單中。

## 在清單中內聯編輯資訊的新體驗

當您在新清單中內聯編輯資訊時，已編輯的列將會變暗，但資訊將保持可見。 在此變更之前，編輯的列顯示為灰色，且資訊不可見。

您可以在Workfront的下列區域找到新清單：

* 專案和任務清單
* 專案、任務和問題的小時索引標籤

## 更新專案、任務和問題時數標籤的清單

改善的清單檢視現在可在專案、任務和問題的小時索引標籤中使用。

在此增強功能之前，新清單僅套用至下列專案：

* 任務清單
* 專案清單

如需有關檢視清單中專案的資訊，請參閱 [開始使用Adobe Workfront中的清單](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## 編輯甘特圖而不啟用特殊編輯模式

現在當啟用或未啟用自動儲存時，您可以編輯工作清單甘特圖。 切換開啟時，您無法復原變更。 在這種情況下，您對專案進行的變更會自動儲存。

如需有關編輯工作清單甘特圖的資訊，請參閱 [更新工作清單甘特圖中的資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## 從Kanban面板中移除「問題」標籤

我們正在移除19.3生產版本中Kanban面板的問題索引標籤。 您仍然可以從Kanban展示板上的待辦專案存取「問題」子標籤。

## 從反複專案詳細資訊頁面移除檔案和問題標籤

>[!NOTE]
>
>2019.3版將在生產環境中進行此變更。 它不會在生產版本之前的預覽環境中進行。

我們將從敏捷疊代詳細資訊頁面中移除檔案和問題標籤：

* **檔案：** 儲存在檔案索引標籤中的所有檔案都必須在生產版本之前移動。 如果您無法移動檔案，您將無法再存取這些檔案。
* **問題：** 此標籤通常位於更多下拉式選單下方。 您仍然可以從疊代上的「工作專案」標籤存取「問題」子標籤。

## 考慮或忽略使用者在任務日期的休假

您現在可以決定是否允許任務之主要受指派人的休假排程來調整計畫日期。

您可以在系統層級、作為Workfront管理員或在專案層級、作為專案經理做出此決定。

在此變更之前，如果「任務限制」允許修改日期，則「主要受指派人」的休假一律會調整任務的計畫日期。

如需有關系統層級使用者休假設定的資訊，請參閱 [設定全系統專案偏好設定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

如需有關專案層級「使用者休假」設定的資訊，請參閱 [編輯專案](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>預覽可用性： 2019年7月22日
>
>生產可用性： 2019年8月9日

## 自訂條件

現在您可以進行下列操作，自訂您用於專案、任務和問題的條件，並更好地滿足組織的需求：

* 使用您自己的標籤和顏色建立自訂條件。
* 變更使用者在下拉式清單中選取條件的順序。
* 使用您建立的自訂條件，取代Workfront自動指派給工作專案的內建預設條件。
* 變更專案、任務和問題的內建預設條件的名稱和顏色。

此外，如果您有權編輯任務或問題，但您未獲得指派（可能是因為您正在監督它），您現在可以使用清單檢視中的條件欄變更其條件。

以前，無法自訂或變更條件，並且只有使用者可以變更任務或問題的條件（如果指派給它）。

如需詳細資訊，請參閱 [自訂條件](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>預覽可用性： 2019年7月4日
>
>生產可用性： 9月底或10月初

## 適用於團隊的新電子郵件通知

為團隊提供新的電子郵件事件通知。 當具有指派給團隊之任務的專案變為使用中狀態時，團隊成員會收到電子郵件通知。 此設定預設為關閉。

過去，團隊成員無法在他們參與的專案生效時收到通知。

如需詳細資訊，請參閱通知：關於我所在專案的資訊。

>[!NOTE]
>
>預覽可用性： 2019年7月4日
>
>生產可用性： 2019年7月18日

## 檔案更新現在會出現在關聯的物件和專案上

當您在檔案上加上註解時，您的更新現在會顯示在檔案及附加檔案的物件的「更新」標籤上。

如果物件是專案的一部分，您對檔案的註解也會出現在專案的「更新」標籤上。

以前，更新註釋只出現在檔案的「更新」標籤上。

如需詳細資訊，請參閱區段 [更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) 在文章中 [更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>預覽可用性： 2019年6月6日
>
>生產可用性： 2019年6月20日

## 將使用者指派給任務和問題時檢視其休假排程

當您將使用者指派給任務或問題時，如果所選使用者在任務或問題的計畫日期之間已排程任何時間的休假，您現在可以看到內嵌警告。

如需指派工作的相關資訊，請參閱 [指派任務](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

如需休假的詳細資訊，請參閱 [設定個人休假](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>預覽可用性： 2019年5月30日
>
>生產可用性： 2019年6月13日

## 新增代表自訂Forms中物件的欄位

我們已在自訂表單產生器中建立一個名為「自動提示」的新欄位型別。 此欄位可讓您將代表物件的欄位新增至自訂表單。 目前，使用者物件已啟用自動提示功能，未來將推出其他物件。

以前，管理員必須在自訂表單下拉式選單中手動將使用者維持為個別選項。

如需詳細資訊，請參閱 [建立或編輯自訂表單](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>預覽可用性： 2019年5月30日
>
>生產可用性： 2019年6月13日
>
>在生產版本發行日期之前，新的自訂欄位在Mobile、Outlook、MS Teams和原生Salesforce整合上不受支援。
>
>在生產環境中，現在支援Outlook和MS Teams。 自6月底或7月初起已支援Mobile；自6月起已支援Salesforce整合。

## 新請求「主旨」欄位已重新命名為「名稱」

>[!NOTE]
>
>此功能已移除，將不會包含在2019.3版中。

現在，當您向請求佇列提交新請求時，在新請求表單的「名稱」欄位中輸入請求名稱。

在此變更之前，您需在「主旨」欄位中輸入請求名稱。

如需建立請求的相關資訊，請參閱 [建立及提交Workfront請求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

