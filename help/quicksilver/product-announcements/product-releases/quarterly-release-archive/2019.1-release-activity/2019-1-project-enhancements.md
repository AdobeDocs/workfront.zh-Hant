---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1專案增強功能
description: 本頁說明2019.1版包含的所有專案增強功能。 此功能目前可在預覽環境中使用。 它可以在的生產環境中使用。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# 2019.1專案增強功能

本頁說明2019.1版包含的所有專案增強功能。 此功能目前可在預覽環境中使用。 它可以在的生產環境中使用。

>[!IMPORTANT]
>
>本頁所述的功能在生產環境使用之前可能會有所變更。

如需2019.1年進行的所有變更清單，請參閱「2019.1版本活動概覽」。

管理員的&#x200B;****

* [從資源回收筒還原範本](#restore-templates-from-the-recycle-bin)
* [顯示首頁](#show-timestamps-for-date-fields-in-home)中日期欄位的時間戳記
* [專案偏好設定下可用的所有期間型別](#all-duration-types-available-under-project-preferences)

**所有使用者**

* [敏捷改善](#agile-improvements)
* [從清單新增任務和問題至反複專案](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [甘特圖匯出的新紙張大小](#new-paper-sizes-for-gantt-chart-export)
* [在編輯模式中移除對甘特圖對話方塊的存取權](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [檢視計畫或Portfolio中專案清單甘特圖中的任務資訊](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [存取範本上的工作清單甘特圖](#access-the-task-list-gantt-chart-on-templates)
* [已重新命名甘特圖上的專案檢視](#renamed-the-project-view-on-the-gantt-chart)
* [工作清單甘特圖中的假設分析藍本](#what-if-scenarios-in-the-task-list-gantt-chart)
* [工作清單改善](#task-list-improvements)
* [以全熒幕顯示清單](#display-lists-in-full-screen)
* [其他區域的新清單](#new-lists-in-additional-areas)
* [以XLSX格式傳送傳遞的報告](#send-a-delivered-report-in-xlsx-format)
* [匯出稽核記錄](#export-audit-logs)

## 從資源回收筒還原範本 {#restore-templates-from-the-recycle-bin}

Workfront管理員現在可以從資源回收筒還原範本。 如同其他已刪除的專案，您最多可以在刪除範本後30天內將其還原。

如需詳細資訊，請參閱「還原已刪除的專案」。

## 在首頁顯示日期欄位的時間戳記 {#show-timestamps-for-date-fields-in-home}

作為Workfront管理員，您現在可以選擇使用版面配置範本在「工作清單」和「行事曆」中顯示或隱藏到期日的時間戳記。 依預設，範本和非範本使用者都能看見時間戳記。

如需詳細資訊，請參閱「建立和管理版面範本」一文中的「自訂首頁區域」。

## 專案偏好設定下可用的所有期間型別 {#all-duration-types-available-under-project-preferences}

在「設定>專案偏好設定」中設定預設任務和問題期間型別時，您可以使用以下任一選項：

簡單

投入比導向

已計算的任務指派

已計算的工作

以前，如果您將「簡單」或「投入比導向」設定為預設期間型別，則無法選擇「計算的任務指派」和「計算的工時」。

如需設定任務和問題期間型別預設值的詳細資訊，請參閱「任務和問題偏好設定」

## 敏捷功能改進 {#agile-improvements}

敏捷工具現在提供下列改良功能：

Kanban

從任何任務清單或報告將任務和問題新增到Kanban面板。

之前，您只能從待處理專案新增任務至Kanban面板。 您無法新增問題。

依團隊中的個別使用者篩選Kanban面板。

如需詳細資訊，請參閱使用Kanban面板。

檢視及管理Kanban待處理專案上的問題。

如需詳細資訊，請參閱使用Kanban面板。

之前，您無法在Kanban展示板上新增或管理問題。

Scrum

依團隊中的個別使用者篩選反複專案劇本面板。

如需詳細資訊，請參閱「使用Scrum敏捷故事板」。

之前，您無法在Kanban或Scrum面板上依使用者篩選。

## 從清單新增任務和問題至反複專案 {#add-tasks-and-issues-from-a-list-to-an-iteration}

您現在可以使用任務或問題清單、報告或儀表板來將劇本新增到疊代。 您也可以在一個疊代中為多個團隊指派劇本。

以前，您只能從任務或問題詳細資訊頁面將內文新增到疊代，並且您只能將內文新增到團隊建立的疊代。

如需詳細資訊，請參閱「建立和管理敏捷反複專案」。

## 以XLSX格式傳送傳遞的報表 {#send-a-delivered-report-in-xlsx-format}

除了目前的所有其他格式外，您現在可以排程報表以MS Excel (.xlsx)格式傳送。

之前，您只能傳送以下格式的報表：

HTML

PDF

MS Excel (.xls)

TSV

如需排程報表傳送的相關資訊，請參閱設定報表傳送。

## 任務清單改善 {#task-list-improvements}

[更新已從]移除的18.3 Beta 4

在18.3 Beta 4版本中短暫移除後，重新設計的工作清單已重新啟用。 我們也在工作清單中引進了以下附加功能，這些功能不是原始版本的一部分：

內聯編輯一項任務時，將滑鼠右鍵功能表取代為其他圖示。

內聯編輯數個任務時，在滑鼠右鍵功能表中可用的選項現在已移至任務清單頂端的圖示。

依預設，工作清單會顯示2000個工作。

當Workfront重新計算時間表時，日期正在更新的任務旁邊的問號已替換為灰色區域。

如需有關編輯內嵌任務的資訊，請參閱複製和複製任務及透過連結任務建立前置任務關係。

如需重新計算專案時間表的相關資訊，請參閱重新計算專案的時間表。

## 以全熒幕顯示清單 {#display-lists-in-full-screen}

當專案或工作清單大於熒幕大小時，現在當您捲動時，清單會自動顯示在整個瀏覽器視窗中。 這樣會增加您一次看到的資訊量，並可讓您更輕鬆地管理清單。

您可以全熒幕顯示下列清單：

下列標籤和子標籤中的專案清單：

我參與的專案

我擁有的專案

所有專案

Portfolio中的專案索引標籤

計畫中的專案索引標籤

以下標籤中的工作清單：

專案中的任務標籤

任務中的子任務標籤

如需有關在清單中顯示物件的資訊，請參閱檢視清單中的專案。

## 其他區域的新清單 {#new-lists-in-additional-areas}

我們已在下列方面改善專案和工作清單的效能與外觀：

「專案」區域中的「Portfolio」和「方案」標籤

任務層級的子任務標籤

在此增強功能之前，新清單僅適用於下列區域：

專案區域中的專案標籤

專案層級的任務標籤

如需有關在清單中顯示物件的資訊，請參閱檢視清單中的專案。

## 在方案或Portfolio的專案清單甘特圖中檢視任務資訊 {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

您現在可以在方案或Portfolio的專案清單甘特圖中，檢視專案工作的相關資訊。

之前，您只能在專案索引標籤的專案清單甘特圖中，檢視關於任務的資訊。

如需詳細資訊，請參閱檢視甘特圖中的資訊。

## 工作清單甘特圖中的假設分析案例 {#what-if-scenarios-in-the-task-list-gantt-chart}

當專案中的任務以甘特圖的編輯模式顯示時，您現在可以對它們執行下列動作：

新增任務

移除任務

內聯編輯任務

複製任務

重新排列任務

修改子任務

雖然您可以看到變更如何影響專案的時間表，但不會立即儲存。 您可以儲存它們以永久更新專案時間表，也可以取消它們。

之前，您無法預覽甘特圖中的任務清單變更。

如需有關編輯甘特圖中的工作的資訊，請參閱更新工作清單甘特圖中的資訊。

## 存取範本上的工作清單甘特圖 {#access-the-task-list-gantt-chart-on-templates}

您現在可以存取專案範本中的「工作清單甘特圖」 。

之前，您無法檢視範本中工作清單上的甘特圖。

如需詳細資訊，請參閱「甘特圖快速入門」。

## 甘特圖轉存的新紙張大小 {#new-paper-sizes-for-gantt-chart-export}

您現在可以在A1和A2紙張大小上列印甘特圖。

之前，您只能匯出至Letter、Legal、Ledger、A3 （僅適用於某些語言）及A4。

如需詳細資訊，請參閱「將甘特圖匯出至PDF」。

## 已重新命名甘特圖上的專案檢視 {#renamed-the-project-view-on-the-gantt-chart}

我們將甘特圖上的「專案」檢視選項重新命名為「適合所有」。 檢視選項仍像之前一樣運作。 新名稱旨在更能說明您選取選項時檢視的內容。

如需詳細資訊，請參閱檢視甘特圖中的資訊。

## 在編輯模式中移除對甘特圖對話方塊的存取權 {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

當甘特圖處於編輯模式時，您無法再存取「進階工作總攬」對話方塊。 您只能在任務清單甘特圖處於編輯模式時進行內嵌編輯。

之前，您可以在甘特圖處於編輯模式時存取「進階工作總攬」對話方塊，但是它儲存了在甘特圖和關閉的編輯模式中所做的變更。

如需有關編輯「工作清單甘特圖」的詳細資訊，請參閱「更新工作清單甘特圖中的資訊」。

## 匯出稽核記錄 {#export-audit-logs}

您現在可以將稽核記錄專案匯出至CSV檔案。 您一次最多可以將50,000個稽核記錄專案匯出至CSV檔案。

如需詳細資訊，請參閱管理稽核記錄。
