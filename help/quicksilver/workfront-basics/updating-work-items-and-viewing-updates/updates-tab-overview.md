---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新區段概觀
description: 物件的「更新」區段會顯示使用者對物件所做的註解，或追蹤物件變更的系統更新。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 9babe17ad862925440e555f881bf753fb443b67d
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 3%

---


# 更新區段概觀

<!-- Audited: 1/2024 -->

<!--take "legacy" and "new commenting" and "production" or "preview" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md) ).</span> -->


<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽」環境中供所有客戶使用，或在「生產」環境中供啟用快速發行的客戶使用。 </span>

<span class="preview">如需快速發行版本的相關資訊，請參閱 [啟用或停用組織的快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">如需目前發行排程的詳細資訊，請參閱 [2024年第二季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

<!--info for April 11: take out the Important box-->

>[!IMPORTANT]
>
>我們目前正在重新設計Adobe Workfront中的評論體驗。
>
>根據您存取註釋體驗的物件，您可能會在「更新」區段中看到下列功能：
>* 新體驗
>* 舊版體驗
>* 全新和舊版體驗
>
>如需有關新評論體驗及其可用性的詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
><Span class="preview"> 舊版評論體驗已從預覽環境中的專案、任務、問題和檔案中移除。 </span>
>
>新註解體驗僅適用於Workfront物件的「更新」區段，當您從以下區域存取更新時，無法使用：
>
> * 首頁
> * 清單中的摘要面板
> * 時程表中的摘要面板
> * 工作負載平衡器中的摘要面板
>
><span class="preview">新的評論體驗可在「預覽」環境中的清單、時程表和工作負載平衡器中的「摘要」面板中取得，並可在已選擇快速發行流程的客戶的「生產」環境中取得。

## 「更新」區段的總覽

物件的「更新」區段會顯示系統更新，以及使用者在過去90天內所做的最近200項更新。

<div class="preview">

![更新區段](assets/updates-tab-with-unified-experience-for-issues-all-tab.png)

</div>

<!--Info for April 11: Add the following right under the screen shot above:

The following objects have an Updates section where you can add comments or review system updates: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations
-->

<!--remove all the information below, all the way down to the following section: -->

根據您存取評論體驗的物件，您可能會在「更新」區段找到下列體驗：

* 下列物件的新舊註解體驗：

   * 專案
   * 工作（包括劇本）
   * 問題
   * 文件

     >[!TIP]
     >
     >使用新註解選項來顯示新的註解體驗（當您啟用時）或舊版註解體驗（當您停用時）。 預設為新的註解體驗。 如需詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* 僅限下列物件的新註解體驗。 沒有選項可啟用這些物件的舊版註解體驗：

   * 目標

     >[!NOTE]
     >
     >您必須額外取得Adobe Workfront目標授權才能存取此Workfront區域。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * 展示板上的卡片
   * 團隊
   * 範本
   * 範本任務
   * 時程表
   * 方案
   * 專案組合
   * 使用者

* 僅限下列物件的舊版註解體驗：

   * 疊代

     沒有選項可啟用反複專案的新註解體驗。 如需詳細資訊，請參閱 [管理反複專案註解](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md).

<!--Info for April 11: reword the section title below to: Overview of the Updates section; and remove the preview tags-->

### 新評論體驗中「更新」區段的概觀

<div class="preview">

![更新區段](assets/updates-tab-after-unified-experience-for-tasks-all-tab.png)

</div>

<!--info for April 11: remove the NOTE below-->

>[!NOTE]
>
>新的註解體驗不適用於反複專案。

* 「更新」區段在新註解體驗的以下標籤中顯示資訊：

   * **註解**：顯示使用者所做的評論以及對這些評論的回覆。 使用「註解」標籤來新增註解或回覆現有註解。 如需有關更新新註解體驗中物件的資訊，請參閱 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).
   * **系統活動**：顯示系統更新，這些資訊性訊息是Workfront為記錄物件上的特定事件而建立的訊息。 例如，狀態、名稱或自訂欄位的變更會透過系統更新擷取。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 <span class="preview">對舊版評論體驗中系統活動記錄所做的任何回覆，都會以唯讀形式填入系統活動標籤中。</span> 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).
   * <span class="preview">**全部（唯讀）**：在一個位置同時顯示使用者註解和系統活動註解。 這是僅供檢視的標籤。 您無法在[全部]索引標籤的現有註解中回覆註解或標籤其他使用者。 若要回覆特定註解，請使用「全部」標籤到「註解」標籤的連結。 如需有關更新新註解體驗中物件的資訊，請參閱 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).</span>

* 下列物件沒有「系統活動」標籤 <span class="preview">或「全部」標籤：</span>

   * 團隊
   * 範本
   * 範本任務
   * 臨機卡

* 下列物件沒有 <span class="preview">所有標籤：</span>

   * 目標

<!-- info for April 11: hide the entire section below: -->

### 舊版更新區段概觀

![](assets/updates-tab-before-unified-experience-for-tasks.png)

舊版更新區段會顯示下列資訊：

* **使用者更新**：使用者所做的評論和對這些評論的回覆。
* **系統更新**：Workfront為記錄物件上的特定事件而建立的資訊訊息。 例如，您可以使用系統更新來擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

下列物件不會記錄系統更新：

* 團隊
* 範本
* 範本任務
* 疊代


## 也會出現在較高排名物件上的更新

某些物件的註解、回覆或系統更新也會顯示在較高等級物件的「更新」區段中。

例如，當您將更新新增到任務時，該更新會出現在任務的「更新」區段以及包含任務的專案的「更新」區段中。

下表顯示其註解也顯示在其較高等級物件上的物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已新增原始更新的物件</strong> </th> 
   <th> <p><strong>也會顯示原始更新的較高等級物件</strong> </p> </th> 
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

>[!NOTE]
>
>新增至系統更新的回覆不會彙總至父物件。 只有子物件的直接回覆和新增至現有更新的回覆會向上彙整至父物件。
>
>如需Adobe Workfront中物件階層的相關資訊，請參閱 [瞭解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> 無法在新評論體驗中回覆系統更新。 如需詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## 更新區段的限制

更新團隊的部分，以及代表其他使用者輸入更新時，有一些限制。

### 使用者和團隊的限制

檢視使用者和團隊的更新時，請考量下列事項：

* 您無法在團隊的「更新」區段中新增註解。

* 您可以對您在團隊中檢視的更新新增回覆。 回覆會顯示在專案團隊的「更新」區段，以及專案團隊所屬物件的「更新」區段中。

* 專案團隊的「更新」區段由在下列物件上輸入的更新來填入：

   * 使用者
   * 時間表*
   * 劇本
   * 反複專案*

  *這些不適用於新的評論體驗。

* 在適用於使用者和團隊的更新區段中，您可以檢視過去90天內輸入的更新。

  如果您想要在90天限制之外檢視使用者或團隊進行的所有更新，您可以建立附註報表。 報告不應具有顯示使用者或團隊所有更新的時間篩選器。 如需詳細資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 代表其他使用者輸入評論時的限制

Adobe Workfront管理員和群組管理員可以其他使用者身份登入，並在Workfront中執行輸入註釋等動作。

如需詳細資訊，請參閱 [以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

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

如需詳細資訊，請參閱 [更新區域報告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
