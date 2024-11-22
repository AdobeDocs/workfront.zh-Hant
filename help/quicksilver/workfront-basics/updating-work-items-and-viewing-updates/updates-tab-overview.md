---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新區段概觀
description: 物件的「更新」區段會顯示使用者對物件所做的註解，或追蹤物件變更的系統更新。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 6327e5625481ce7ff8d744bc6eb50d417cbb4413
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 4%

---


# 更新區段概觀

<!-- Audited: 1/2024 -->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

物件的「更新」區段會顯示使用者對物件所做的註解，或追蹤物件變更的系統更新。

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process.
-->

## 「更新」區段的總覽

物件的「更新」區段會顯示系統更新，以及使用者在過去90天內所做的最近200項更新。

![更新區段](assets/updates-tab-with-unified-experience-for-issues-all-tab.png)

<!--Info for April 11: Add the following right under the screen shot above:-->

下列物件有「更新」區段，您可以在其中新增註解或檢閱系統更新：

* 專案
* 任務
* 問題
* 計劃
* 專案組合
* 範本
* 範本任務
* 使用者
* 時程表
* 團隊
* 目標
* 疊代

下列物件有可以新增註釋及檢閱系統更新的區域：

* 展示板上的卡片
* Workfront Planning中的記錄

<!--info for April 11: remove all the information below, all the way down to the following section: -->

<!--
Depending on what objects you access the commenting experience for, you might find the following experience for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

  * Project
  * Task (this includes Stories)
  * Issue
  * Document

    >[!TIP]
    >
    >Use the New commenting option to display the new commenting experience (when you enable it) or the legacy commenting experience (when you disable it). The new commenting experience is the default. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

  * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations

    There is no option to enable the new commenting experience for iterations. For more information, see [Manage iteration comments](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md). 
-->

<!--Info for April 11: reword the section title below to: Overview of the Updates section; and remove the preview tags-->

### 更新區段標籤總覽

![更新區段](assets/updates-tab-after-unified-experience-for-tasks-all-tab.png)

「更新」區段會在下列標籤中顯示資訊：

* **註解**：顯示使用者所做的註解以及這些註解的回覆。 使用「註解」標籤來新增註解或回覆現有註解。 如需有關更新物件的資訊，請參閱[更新工作](../updating-work-items-and-viewing-updates/update-work.md)。
* **系統活動**：顯示系統更新，這些是Workfront建立的資訊訊息，用來在物件上記錄特定事件。 例如，狀態、名稱或自訂欄位的變更會透過系統更新擷取。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 對舊版評論體驗中系統活動記錄所做的任何回覆，都會以唯讀形式填入系統活動標籤中。 如需詳細資訊，請參閱[設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)。
* **全部（唯讀）**：在一個位置同時顯示使用者註解和系統活動註解。 這是僅供檢視的標籤。 您無法在[全部]索引標籤的現有註解中回覆註解或標籤其他使用者。 若要回覆特定註解，請使用「全部」標籤到「註解」標籤的連結。 如需有關更新物件的資訊，請參閱[更新工作](../updating-work-items-and-viewing-updates/update-work.md)。

  >[!NOTE]
  >
  >「註解」和「系統」活動標籤會即時更新。 您必須重新整理[全部]索引標籤才能檢視最近的更新。

### 不同物件「更新」區域的異同

不同物件的註釋和更新顯示方式有所不同。

* 以下物件在更新區段的所有三個索引標籤中具有類似的體驗：

   * 專案
   * 任務
   * 問題
   * 計劃
   * 專案組合
   * 使用者
   * 時程表

* 下列物件沒有「系統」活動標籤或「全部」標籤，且「註解」標籤中的體驗符合所有其他物件的體驗：

   * 團隊
   * 範本
   * 範本任務

* 下列物件沒有「系統」活動標籤或「全部」標籤，且「註解」標籤中的體驗與所有其他物件的體驗不同：

   * 疊代
   * 面板區域中的臨時卡片

     如需卡片更新的詳細資訊，請參閱[將臨機卡片新增到展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)。

* 下列物件有「系統」活動標籤，沒有「全部」標籤：

   * 面板區域中的已連線卡片

     如需詳細資訊，請參閱[使用主機板上的連線卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

* 下列物件具有「歷史記錄」標籤，可取代「系統」活動標籤：

   * Workfront Planning中的記錄

     如需詳細資訊，請參閱[歷程記錄區段總覽](/help/quicksilver/planning/records/history-section-overview.md)。

* 下列物件沒有「全部」標籤，「註解」標籤中的體驗符合大多數物件的體驗：

   * 目標

     如需有關目標更新的詳細資訊，請參閱[管理目標註解](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md)。

<!-- info for April 11: hide the entire section below: -->

<!--
### Overview of the legacy Updates section 

![](assets/updates-tab-before-unified-experience-for-tasks.png)

The legacy Updates section shows the following information:

* **User updates**: Comments made by users and replies to those comments. 
* **System updates**: Informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your objects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

The following objects don't record system updates:

* Team
* Template
* Template Task
* Iterations
-->

## 也會出現在較高等級物件上的更新

某些物件的註解、回覆或系統更新也會出現在較高層級物件的「更新」區段中。

例如，當您將更新新增到任務時，該更新會出現在任務的「更新」區段以及包含任務的專案的「更新」區段中。

下表顯示其註解也顯示在其較高等級物件上的物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已新增原始更新的物件</strong> </th> 
   <th> <p><strong>原始更新也出現的較高等級的物件</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>問題</td> 
   <td>專案</td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>專案</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>計畫，Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>文件 </td> 
   <td>附加檔案的物件，專案 </td> 
  </tr> 
 </tr> 
  <tr data-mc-conditions=""> 
   <td>校樣 </td> 
   <td>文件 </td> 
  </tr>

<tr> 
   <td>方案</td> 
   <td>專案組合</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>團隊</td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td><p>使用者、團隊</p>
   <p><b>附註</b></p>
   <p>時程表註解會顯示在發表註解之使用者的「更新」區段及其主團隊的「更新」區段。</p>
   </td> 
  </tr> 
  <tr> 
   <td>範本任務</td> 
   <td>範本</td> 
  </tr> 
  <tr> 
   <td>本文</td> 
   <td>反複專案，團隊</td> 
  </tr> 
  <tr> 
   <td>反覆項目</td> 
   <td>團隊</td> 
  </tr>

<tr> 
   <td>結果</td> 
   <td>目標</td> 
  </tr> 
  <tr> 
   <td>活動</td> 
   <td>目標</td> 
  </tr> 
 </tbody> 
</table>

<!--info for April 11: hide the note below-->

<!--
>[!NOTE]
>
>Replies added to system updates do not roll up to the parent object. Only direct replies on a child object and replies added to existing updates roll up to parent objects.
>
>For information about the object hierarchy in Adobe Workfront, see [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> It is not possible to reply to system updates in the new commenting experience. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
-->


## 更新區段的限制

更新團隊的部分，以及代表其他使用者輸入更新時，有一些限制。

### 使用者和團隊的限制

檢視使用者和團隊的更新時，請考量下列事項：

* 您無法在團隊的「更新」區段中新增註解。

* 專案團隊的「更新」區段由在下列物件上輸入的更新來填入：

   * 使用者
   * 劇本
   * 時程表
   * 疊代

* 您可以對您在團隊中檢視的更新新增回覆。 回覆會顯示在專案團隊的「更新」區段，以及專案團隊所屬物件的「更新」區段中。

* 在適用於使用者和團隊的更新區段中，您可以檢視過去90天內輸入的更新。

  如果您想要在90天限制之外檢視使用者或團隊進行的所有更新，您可以建立附註報表。 報告不應具有顯示使用者或團隊所有更新的時間篩選器。 如需詳細資訊，請參閱[建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

### 代表其他使用者輸入評論時的限制

Adobe Workfront管理員和群組管理員可以其他使用者身份登入，並在Workfront中執行輸入註釋等動作。

如需詳細資訊，請參閱[以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)。

以其他使用者身分登入並新增註解時，請考慮下列事項：

* 代表其他使用者所做的任何評論都會在評論中標示。

* 群組管理員可以代表其他人發表評論，但無法刪除該評論。 只有Adobe Workfront管理員可以刪除他們代表其他使用者所做的評論。

* Workfront或群組管理員只有在以使用者身分登出並以本身身分登入時，才能編輯他們代表其他使用者新增的評論。 他們無法代表其他使用者刪除評論。

## 使用分錄報表檢視工作專案的系統更新

「日誌專案」報表會從專案、任務和問題的更新區域顯示系統更新。

報表可讓您檢視：

* 已發生的狀態變更數量
* 刪除任務或問題時
* 重要自訂欄位中的值在專案過程中如何變更
* 專案過程中變更了哪些重要日期
* 如果優先順序在專案過程中改變
* 如果專案所有者已變更

如需詳細資訊，請參閱[更新區域報告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)。
