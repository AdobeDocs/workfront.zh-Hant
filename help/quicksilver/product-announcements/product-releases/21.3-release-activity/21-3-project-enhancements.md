---
title: 21.3專案增強功能
description: 21.3專案增強功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3專案增強功能

本頁面說明在「預覽」環境中21.3版所做的所有專案增強功能。 這些增強功能已於2021年7月21日當周在生產環境中推出。

如需21.3版所有可用變更的清單，請參閱 [21.3版本概觀](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## 將範本與群組關聯

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

為了幫助您簡化項目建立流程，並幫助您更輕鬆地確定哪些組擁有哪些項目模板，並報告這些組，我們添加了將組分配給項目模板的能力。

將組分配給項目模板時，從模板建立的所有項目都會自動與模板的組關聯。 如需詳細資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

此外，如果模板與您的組關聯，則可以將組批准流程附加到模板及其模板任務。 如需詳細資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 更輕鬆編輯「詳細資料」區段中的欄位

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

下列改良功能可讓您更輕鬆地編輯任何物件之「詳細資訊」區段中的資訊：

* 將滑鼠游標暫留在欄位上時，其周圍的灰色輪廓表示該欄位可編輯。
* 您可以按一下欄位一次來編輯欄位。

在此增強功能之前，不清楚哪些欄位是可編輯的，您必須連按兩下才能編輯欄位。

## 在計算切換日期時考慮跨項目前置任務

隨著Adobe Workfront計算任務切換日期方式的新改善，現在已考慮跨專案相依性。

以前，僅基於同一項目中任務的前置任務來計算切換日期。

現在，為了確保始終具有跨項目前置任務的準確切換日期，必須重新計算後續任務項目的時間表。 在重新計算時間線之後，考慮任務的跨項目依賴關係來計算任務的切換日期。

有關切換日期的詳細資訊，請參閱 [任務切換日期概述](../../../manage-work/tasks/task-information/handoff-task-date.md).

## 從Scrum展示板新增現有動態和問題

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

您現在可以直接從Scrum展示板新增現有的文章或問題。 這可讓您更輕鬆地將現有動態新增至目前的迭代，而不需前往積壓頁面。

如需詳細資訊，請參閱 [從Scrum展示板新增動態和問題](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 從Scrum展示板新增動態和問題

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

您現在可以直接從Scrum展示板建立新動態或期刊。 這可讓您更輕鬆地將新動態快速新增至目前的迭代。

如需詳細資訊，請參閱 [從Scrum展示板新增動態和問題](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 從看板板中刪除文章或問題

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

您現在可以從看板板中直接刪除文章或發放，方法是按一下文章或發放卡上的「更多」表徵圖，然後選擇「刪除」。 刪除文章或問題時，它將移到資源回收筒30天，並且只能由系統管理員恢復。

如需詳細資訊，請參閱 [從看板板中刪除動態或問題](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## 敏捷卡片頁首和文章板更新

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

在看板和清單板上，現在提供了以下增強功能：

* 動態卡片和展示板欄的寬度固定，因此如果您調整瀏覽器視窗大小，卡片大小不會變更。
* 「動態」欄已重新命名為「父動態」。
* 每張卡片頂端都有標籤，可將其識別為父貼文、子工作（與父貼文關聯）、文章（未與父貼文關聯）或問題。
* 背景底紋以視覺化方式分隔欄。

如需詳細資訊，請參閱 [反覆項目概觀](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## 將項目、任務和問題首選項分組

如我們先前所傳達的，我們已針對專案、任務和問題偏好設定推出群組層級的自訂，分階段進行，直到2021年6月24日。 現在轉出已完成，並可在生產環境中供所有客戶使用。

如需詳細資訊，請參閱下列文章：

* [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## 允許外部用戶批准文檔

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

您現在可以使用外部電子郵件地址，將核准者指派給新Workfront體驗中的檔案。

過去，您只能在Workfront Classic中透過電子郵件地址新增外部使用者。

如需詳細資訊，請參閱 [請求文檔批准](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 從產品組合或方案的「詳細資訊」部分導出資訊

>[!NOTE]
>
>此功能已於2021年5月20日發佈至「預覽」環境。 它將於2021年6月3日發行至生產環境。

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

您現在可以從產品組合和程式的詳細資訊區段，匯出為.pdf檔案資訊。 在此增強功能之前，您只能從專案、工作和問題，從「詳細資訊」區段匯出資訊。

如需從物件匯出自訂表單的相關資訊，請參閱 [匯出自訂表單和物件詳細資訊](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## 在物件的標題中新增計畫完成日期時間戳記

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

為方便存取、方便且準確，我們已新增選項，以在專案、工作或問題標題的「計畫完成日期」中選取時間戳記。

在此增強功能之前，當您更新物件的「計畫完成日期」時，Workfront會選取午夜作為預設時間。 現在，您可以自訂時間和完成日期。

如需新Workfront體驗中物件標題的相關資訊，請參閱 [新物件標題](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## 將自訂表單新增至物件，而不需加以編輯

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

我們讓您將自訂表單新增至物件更輕鬆，讓其他人可填寫，或您稍後可填寫。 新增表單時，表單不再自動進入編輯模式。 您只需將空白表單儲存至物件即可。

以前，當您將自訂表單新增至物件時，頁面會進入編輯模式，您必須先完成表單上的任何必要欄位，才能將其儲存至物件。 當表單是要讓其他使用者填寫，或您尚不知道要在表單的必要欄位中加入什麼時，這會很不方便。

如需將自訂表單新增至物件的詳細資訊，請參閱 [將自訂表單新增至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

