---
title: 22.1專案增強功能
description: 22.1專案增強功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# 22.1專案增強功能

本頁說明22.1版對預覽環境所做的所有專案增強功能。 這些增強功能將在生產環境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日當週。

如需22.1版本可用的所有變更清單，請參閱[22.1版本總覽](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md)。

## 變更複製或移動任務時前置任務的預設選項

為了將複製或移動任務時的手動步驟數減到最少，我們更新了預設與任務一起複製或移動的資訊。 現在，所有前置任務預設會隨任務一起複製或移動，因為預設會選取「所有前置任務」選項。

在此增強功能之前，在複製或移動任務時，預設會取消選取「所有前置任務」選項。

如需詳細資訊，請參閱文章：

* [複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## 更新了儀表板清單和報告上的工具列

四個儀表板頁面上的工具列現在具有符合其他Workfront清單（例如專案、任務和問題）的現代化外觀。 此直覺式工具列現在可讓您更輕鬆地新增、編輯、共用、複製和刪除控制面板。

具有已更新工具列的頁面為：

* 任務報告（顯示在控制面板中）
* 所有報告面板清單
* 我的儀表板清單
* 共用控制面板清單

如需詳細資訊，請參閱[建立和管理儀表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md)。

## 新增和編輯檔案的自訂表單摘要面板

您現在可以直接在檔案摘要面板中新增和編輯自訂表單。

透過這項變更，您也會在檔案「摘要」中看到新的外觀與風格。 有一個新的「概觀」區段，其中包含影像縮圖以及檔案詳細資訊。 您也可以在檔案詳細資訊區段中存回和取出檔案。

之前，您必須前往檔案詳細資訊中的自訂表單索引標籤，才能進行編輯或新增自訂表單。

如需詳細資訊，請參閱[檔案概述](../../../documents/managing-documents/summary-for-documents.md)的摘要。

## 複製一或多個任務時的新體驗

為了讓您使用Workfront與新的Adobe Workfront體驗一致，我們在複製任務時重新設計了介面。 目前可在作業層次復製作業，或在清單中復製作業或多個作業時使用此功能。

部分改善包括：

* 在複製任務之前必須更新的所有資訊都會顯示在一個連續的頁面上。
* Workfront會在選擇專案後，立即檢查您是否有目的地專案的存取權。 在此增強功能之前，在您確認複製後，會顯示一則警告訊息，指出您沒有正確的存取權，這會導致額外的步驟，且不允許複製。
* 能夠要求存取您要複製任務的專案，而不需要離開「複製任務」方塊。

如需詳細資訊，請參閱[複製和複製工作](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

## 從清單移動一或多個任務時的新體驗

為了在執行相同任務時提供一致的體驗，我們現在更新了從清單移動一個或多個任務的介面，以在任務層級移動任務時符合體驗。 （我們已更新在先前的「預覽」版本中，在任務層級移動任務的體驗。）

如需詳細資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

## 在任務層級移動任務時的新體驗

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了用於移動任務的介面。 目前可在任務層級移動任務時使用此功能。 在下一個版本中，我們將將此重新設計擴展為從清單中移動任務。

這個全新重新設計的介面部分改良包括：

* 移動前必須更新的所有資訊都會顯示在一個連續的頁面上。
* Workfront會在選擇專案後，立即檢查您是否有目的地專案的存取權。 在此增強功能之前，Workfront警告您確認移動後沒有正確的存取權，這會導致額外的步驟，且不允許移動。
* 能夠要求存取您要移動任務的專案，而不離開「移動任務」方塊。

如需詳細資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

## 在問題層級使用範本將問題轉換為專案時的新體驗

>[!NOTE]
>
>此功能已於2022年3月4日暫時從生產環境中移除。 它後來在2022年4月28日開始分階段發行。 推出已於2022年5月5日完成。 現在，預覽和生產版都可供所有客戶使用。 （如需此功能發行至生產環境的最新狀態更新，請參閱[22.3版本總覽](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)。）

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了介面，讓您從問題頁面使用範本時將其轉換為專案。

選取轉換問題後，您現在可以更輕鬆地立即存取我的最愛清單。

重新設計的介面與從範本建立專案時的體驗相符，我們最近也更新了範本。

如需詳細資訊，請參閱[在Adobe Workfront中將問題轉換為專案](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)。

## 使用清單、報告和儀表板的範本將問題轉換為專案

>[!NOTE]
>
>此功能已於2022年3月4日暫時從生產環境中移除。 它後來在2022年4月28日開始分階段發行。 推出已於2022年5月5日完成。 現在，預覽和生產版都可供所有客戶使用。 （如需此功能發行至生產環境的最新狀態更新，請參閱[22.3版本總覽](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)。）

為了提高您的工作效率，讓您更輕鬆地在快節奏環境中轉換問題，我們已新增使用清單、報告或儀表板中的範本將問題轉換為專案的功能。

在此增強功能之前，此功能僅當您從問題頁面轉換問題時存在。

如需詳細資訊，請參閱[在Adobe Workfront中將問題轉換為專案](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)。

## 在敏捷板上依使用者清單篩選，顯示具有最多指派的使用者先前

>[!NOTE]
>
>22.1版不含此功能。 已從預覽環境中移除。

現在，篩選器會先顯示具有最多指派的使用者，這樣他們就更容易找到而無需捲動清單。

先前，Kanban和Scrum面板上的依使用者清單篩選會依字母順序顯示。

如需詳細資訊，請參閱下列資訊

* [在Scrum展示板上依使用者篩選](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [在Kanban板上依使用者篩選](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## 限制將檔案新增至您共用的範本的能力

有時候，人們會將檔案新增至專案範本，以為他們要將檔案新增至專案。 現在您可以協助防止這種情況 — 當您以檢視存取權共用範本時，可以停用新的進階設定「新增檔案」。 這會停用收件者將檔案新增至範本的能力。

如需共用範本的指示，請參閱[共用專案範本](../../../manage-work/projects/create-and-manage-templates/share-project-template.md)。

如需有關新進階設定[新增檔案]的資訊，請參閱[共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)一節中的章節。

## 共用檔案資料夾

現在您可以從檔案區域共用檔案資料夾及其內容。 以前這是不可能的，您必須單獨共用資料夾中的每一份檔案。

如需詳細資訊，請參閱[共用檔案資料夾](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

