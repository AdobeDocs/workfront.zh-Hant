---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 處理它並完成按鈕總覽
description: 當您被指派到任務或問題時，您可以使用內容按鈕，該按鈕會根據您對工作專案的參與來變更名稱和功能。
author: Lisa and Alina
feature: Get Started with Workfront
role: User
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: f5632af0fb87739fc41c4e2f41dc8ebab0f8be8b
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# 處理它並完成按鈕總覽

當您被指派到任務或問題時，您可以使用內容按鈕，該按鈕會根據您對工作專案的參與來變更名稱和功能。

使用內容按鈕來接受或完成工作專案，您可以讓Adobe Workfront更新專案上的多個欄位，而無需自行手動更新。

具有下列條件的使用者可看見處理它和完成按鈕：

* 標準授權（新），或計畫或工作授權（目前）
* 有限制的編輯存取權或任務或問題的較高許可權

## 處理它和完成按鈕名稱

根據您從哪個Workfront區域存取您的任務或問題，處理它或完成按鈕可以變更名稱，如以下案例所述：

* 當任務或問題首次指派給您且狀態為新建時，按鈕顯示為其上的工作。

  ![](assets/nwe-work-on-it-button.png)

  >[!TIP]
  >
  >您可以使用開始按鈕取代處理它按鈕。 如需有關將[處理它]按鈕取代為[開始]按鈕的資訊，請參閱[將[處理它]按鈕取代為[開始]按鈕](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)。

* 在您按一下「處理它接受」後，按鈕會依據您在Workfront中存取任務或問題的位置而變更為「標示為完成」或「完成」 。 有關您可以在何處存取「處理它」按鈕的資訊，請參閱本文中的[尋找處理它並完成按鈕](#locate-the-work-on-it-and-done-button)小節。

  ![](assets/nwe-mark-as-done-button-350x122.png)

* 如果您不是唯一指派給任務或問題的人，並且您正從「首頁」區域的「工作清單」存取您的工作專案，則按鈕會變更為「完成我的零件」。

  ![](assets/home-left-done-with-my-part-button-350x184.png)

## 找到處理它的工作並完成按鈕 {#locate-the-work-on-it-and-done-button}

您可以在Workfront的下列區域中找到「處理它並完成」按鈕：

* 首頁區域，在工作清單或詳細資訊面板中

  如需有關在首頁區域將專案標示為完成的資訊，請參閱[在首頁區域將專案標示為完成](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md)。

* 在任務或問題的標題中

  如需物件標頭的詳細資訊，請參閱[新物件標頭](../../workfront-basics/the-new-workfront-experience/new-object-headers.md)。

* 在任務或問題清單或工作負載平衡器中的摘要面板

  如需有關使用「摘要」面板的資訊，請參閱[摘要概觀](../../workfront-basics/the-new-workfront-experience/summary-overview.md)。

## 按一下「處理它並完成」按鈕時自動更新的欄位概觀

使用它的工作和完成按鈕的好處是，您可以允許Workfront自動更新有關指派給您的工作專案的資訊。

* [處理它按鈕](#work-on-it-button)
* [開始按鈕](#start-button)
* [完成按鈕](#the-done-button)

### 處理它按鈕 {#work-on-it-button}

當您按一下「處理它」時，也會更新下列專案：

* 工作分派狀態更新從「已請求」到「正在處理」

  >[!TIP]
  >
  >「工作分派狀態」欄位僅會顯示在報告和清單中。 如需[工作分派狀態]欄位的相關資訊，請參閱[Adobe Workfront術語辭彙表](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

* 認可日期

  如需認可日期的相關資訊，請參閱[認可日期概觀](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

### 開始按鈕 {#start-button}

如果您有編輯團隊的存取權，您可以將其上的工作按鈕取代為團隊的開始按鈕。 當以該團隊作為其主團隊的使用者按一下他們被指派給的專案上的「開始」按鈕，其工作專案上的其他欄位會自動更新。 有關將[處理它]按鈕取代為[開始]按鈕的資訊，請參閱[將[處理它]按鈕取代為[開始]按鈕](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)。

除了按一下處理它按鈕時更新的欄位外，當您按一下開始按鈕時，以下欄位會自動更新任務或問題：

* 狀態
* 實際開始日期

  如需實際開始日期的相關資訊，請參閱[專案實際開始日期的總覽](../../manage-work/projects/planning-a-project/project-actual-start-date.md)。

* 實際完成日期，如果「開始」按鈕與等同於「完成」或「已關閉」的狀態相關聯。

  如需實際完成日期的相關資訊，請參閱[專案實際完成日期概觀](../../manage-work/projects/planning-a-project/project-actual-completion-date.md)。

>[!NOTE]
>
>按一下「復原」按鈕會將工作專案恢復為原始狀態，並刪除「實際開始日期」。
>
>「復原」按鈕在下列區域無法使用：
>
>* 團隊請求
>* 任務標題
>

### 完成按鈕 {#the-done-button}

如果您有權編輯團隊，您可以設定團隊的「完成」按鈕，以在您將專案標籤為完成時更新任務或問題狀態。 當使用者以該團隊作為他們的主團隊按一下他們的專案上的完成按鈕，以下欄位將自動更新任務或問題：

* 狀態
* 從工作到完成的指派狀態更新
* 實際完成日期

如需有關為團隊設定「完成」按鈕的資訊，請參閱下列文章：

* [設定任務的[完成]按鈕](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [設定問題的完成按鈕](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
