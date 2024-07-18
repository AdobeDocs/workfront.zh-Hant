---
title: 21.3專案增強功能
description: 21.3專案增強功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3專案增強功能

本頁說明21.3版對預覽環境所做的所有專案增強功能。 這些增強功能已在2021年7月21日當週的生產環境中推出。

如需21.3版本可用的所有變更清單，請參閱[21.3版本總覽](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md)。

## 建立範本與群組的關聯

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

為了協助您簡化專案建立流程，以及協助您更輕鬆地識別和報告哪些群組擁有哪些專案範本，我們新增了將群組指派給專案範本的功能。

將群組指派給專案範本時，從範本建立的所有專案都會自動與範本的群組建立關聯。 如需詳細資訊，請參閱[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

此外，如果範本與您的群組相關聯，則您可以將群組核准流程附加至範本及其範本任務。 如需詳細資訊，請參閱[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

## 更輕鬆地編輯詳細資訊區段中的欄位

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

下列改良功能可讓您更輕鬆地編輯任何物件「詳細資訊」區段中的資訊：

* 將滑鼠懸停在欄位上時，該欄位周圍會出現灰色外框，表示該欄位是可編輯的。
* 您可以按一下欄位來編輯欄位。

在此增強功能之前，不清楚哪些欄位可編輯，您必須按兩下才能編輯欄位。

## 計算移交日期時考慮跨專案前置任務

隨著Adobe Workfront計算任務移交日期的方式出現新的改進，跨專案相依性現在已納入考量。

以前，移交日期僅根據相同專案中任務的前置任務計算。

現在，為了確保您一律擁有跨專案前置任務之任務的準確移交日期，您必須重新計算後續任務之專案的時間表。 重新計算時間表後，任務的移交日期會考慮任務的跨專案相依性。

如需移交日期的詳細資訊，請參閱[工作移交日期概觀](../../../manage-work/tasks/task-information/handoff-task-date.md)。

## 從Scrum展示板新增現有劇本和問題

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

您現在可以直接從Scrum展示板新增現有劇本或問題。 這可讓您更輕鬆地新增現有內文到您目前的反複專案，而不需要移至待處理頁面。

如需詳細資訊，請參閱[從Scrum展示板新增劇本和問題](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md)。

## 從Scrum展示板新增劇本和問題

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

您現在可以直接從Scrum展示板建立新劇本或問題。 這可讓您更輕鬆地將新劇本快速新增至您目前的反複專案。

如需詳細資訊，請參閱[從Scrum展示板新增劇本和問題](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md)。

## 從Kanban面板中刪除本文或問題

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

您現在可以直接從Kanban面板刪除內文或問題，方法是按一下內文或問題卡上的「更多」圖示並選取「刪除」。 當您刪除內文或問題時，內文或問題會移至資源回收筒並保留30天，且只有系統管理員才能復原。

如需詳細資訊，請參閱[從Kanban面板刪除劇本或問題](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)。

## 敏捷卡片標題和故事板更新

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

Kanban和Scrum展示板上現在提供下列增強功能：

* 內文卡片和板欄的寬度固定，因此如果您調整瀏覽器視窗大小，卡片大小不會變更。
* 「劇本」欄已重新命名為「父級劇本」。
* 每個卡片在頂端都有標籤，可將其識別為父內文、子任務（與父內文相關聯）、內文（與父項無關）或問題。
* 背景陰影會以視覺化方式分隔欄。

如需詳細資訊，請參閱[反複專案總覽](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md)。

## 群組專案、任務和問題偏好設定

如同我們先前所溝通，我們在截至2021年6月24日的階段中推出專案、任務和問題偏好設定的群組層級自訂。 現在推出已完成，並可在生產環境中供所有客戶使用。

如需詳細資訊，請參閱下列文章：

* [設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## 允許外部使用者核准檔案

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

您現在可以使用外部電子郵件地址，將核准者指派給新Workfront體驗中的檔案。

之前，您只能在Workfront Classic中依電子郵件地址新增外部使用者。

如需詳細資訊，請參閱[要求檔案核准](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)。

## 從投資組合或方案的詳細資訊區段匯出資訊

>[!NOTE]
>
>此功能已於2021年5月20日發佈到預覽環境。 它將於2021年6月3日發佈到生產環境。

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

您現在可以從Portfolio和Programs的Details區段匯出至.pdf檔案資訊。 在此增強功能之前，您只能從專案、任務和問題匯出詳細資訊區段的資訊。

如需從物件匯出自訂表單的相關資訊，請參閱[匯出自訂表單和物件詳細資料](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)。

## 在物件標頭中新增規劃完成日期時間戳記

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

為方便存取、方便及準確，我們新增了選項，以在專案、任務或問題標題的計畫完成日期中選取時間戳記。

在此增強功能之前，當您更新物件的規劃完成日期時，Workfront會選取午夜作為預設時間。 現在，您可以自訂時間以及完成日期。

如需有關新Workfront體驗中物件標頭的資訊，請參閱[新物件標頭](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)。

## 新增自訂表單至物件而不編輯它

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

我們更輕鬆地新增自訂表格，讓其他人可以填寫（或您稍後再填寫）該表格。 新增表單時，表單不再自動進入編輯模式。 您只需將空白表單儲存至物件即可。

之前，當您新增自訂表單至物件時，頁面會進入編輯模式，您必須先完成表單上的任何必填欄位，才能將其儲存至物件。 當表單要由其他使用者填寫，或您不知道在表單上要輸入什麼內容時，這會造成不便。

如需將自訂表單新增至物件的相關資訊，請參閱[將自訂表單新增至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

