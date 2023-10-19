---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新區段概觀
description: 物件的「更新」區段會顯示使用者對物件所做的註解，或追蹤物件變更的系統更新。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: bc7039bc4b8b257fc55e71e73f72327fdb417837
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 5%

---

# 更新區段概觀

<!--take "Beta" references out when we remove the beta-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。 </span>\
<span class="preview">如需快速發行版本的相關資訊，請參閱 [啟用或停用組織的快速發行](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<span class="preview">如需目前發行排程的詳細資訊，請參閱 [2023年第四季版本總覽](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>我們目前正在重新設計Adobe Workfront中的評論體驗。
>
>根據您存取評論體驗的環境和物件，您可能會在更新區段中看到不同的功能。
>
>如需有關新評論體驗及其可用性的詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>新註解體驗僅適用於「更新」區段，不適用於下列區域：
>
> * 首頁
> * 清單中的摘要面板
> * 時程表中的摘要面板

<!-- with October 26 release: add somewhere this:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old note, removed with August 2023: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the new commenting experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

The Updates section of an object displays comments that users make on the object or system updates that track changes to the object.

-->

## 「更新」區段的總覽

* 物件的「更新」區段會顯示最近90天內進行的最多200個更新。

  ![](assets/updates-tab-before-unified-experience-for-issues.png)

* 會針對下列物件顯示「更新」段落：

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td> 
      <ul> 
      <li>文件</li> 
      <li>目標</li> 
      <li>問題</li> 
      <li>疊代</li> 
      <li>專案</li> 
      <li>計劃</li> 
      <li>專案組合</li> 
      </ul> </td> 
    <td> 
      <ul> 
      <li>劇本*</li> 
      <li>任務</li> 
      <li>範本</li> 
      <li>範本任務</li> 
      <li>時程表</li> 
      <li>使用者</li>
      <li>展示板上的卡片</li>
      </ul> </td> 
    </tr> 
  </tbody> 
  </table>

  *劇本是任務。 所有與工作相關的資訊也可用於劇本。

根據您從哪個環境存取更新，更新區段中的資訊會有不同的組織方式。


### 目前更新區段的總覽

<!--October 26 - replace current with legacy-->

* 目前的「更新」段落顯示下列資訊：

   * **使用者更新**：使用者所做的評論和對這些評論的回覆。
   * **系統更新**：Workfront為記錄物件上的特定事件而建立的資訊訊息。 例如，您可以使用系統更新來擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 下列物件不會記錄系統更新：

   * 團隊
   * 範本
   * 範本任務

### 新評論體驗中「更新」區段的概觀

如需有關新註解體驗有哪些功能可用以及哪些物件的資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<span class="preview">![](assets/updates-tab-after-unified-experience-for-tasks.png)</span>

* 「更新」區段在新註解體驗的以下標籤中顯示資訊：

   * **註解**：顯示使用者所做的評論以及對這些評論的回覆。 如需有關更新新註解體驗中物件的資訊，請參閱 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).
   * **系統活動**：顯示系統更新，這些資訊性訊息是Workfront為記錄物件上的特定事件而建立的訊息。 例如，您可以使用系統更新來擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

      * 下列物件沒有「系統活動」標籤：

         * 團隊
         * 範本
         * 範本任務
         * 臨機卡

* 目前，您可以在下列物件上使用新的註解體驗來新增註解及回覆更新：


   * 專案
   * 任務（和劇本）
   * 問題
   * 文件
   * 目標

  >[!NOTE]
  >
  >您必須額外擁有授權才能存取Workfront目標。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * 展示板上的卡片

  >[!NOTE]
  >
  > 當您啟用卡片上的「註解」和「系統活動」區段時，您可以在「面板」區域中新增和檢視卡片的更新。 如需詳細資訊，請參閱 [新增臨機卡到展示板](../../agile/get-started-with-boards/add-card-to-board.md).


  <span class="preview">

   * 範本
   * 範本任務
   * 時程表
   * 使用者
   * 專案組合
   * 計劃

  >[!NOTE]
  >
  >    您無法顯示版序的新註解體驗。

  </span>

<!--hidden in August 2023 and replaced by the list above: 

  <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
      <tr> 
      <td> 
        <ul> 
        <li><p>Goals</p>
        <li>Cards in the Boards area*</li>
          This is the only experience for goals and cards.
        </li> 
        <li>Projects</li>
        </ul> </td> 
      <td> 
        <ul> 
        <li>Issues</li> 
        <li>Tasks</li>
        <li>Documents</li>
        </ul> </td> 
      </tr> 
    </tbody> 
    </table>

  *You can add and view updates to cards in the Board areas when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md). 
  -->

## 也會出現在較高排名物件上的更新

對特定物件更新所做的評論或回覆也會顯示在較高排名物件的「更新」區段中。

例如，當您將更新新增到任務時，該更新會出現在任務的「更新」區段以及包含任務的專案的「更新」區段中。

>[!NOTE]
>
>啟用新的註解體驗時，註解會顯示在下列排名較高的物件上：
>
>* 問題
>* 專案
>* 任務
>
>如需詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

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
   <td>使用者、團隊</td> 
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
   <td>目標</td> 
   <td>結果，活動</td> 
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

您無法在團隊的「更新」區段中新增註解。

<span class="preview">您可以對您在團隊中檢視的更新新增回覆。 回覆會顯示在專案團隊的「更新」區段，以及專案團隊所屬物件的「更新」區段中。 </span>

專案團隊的「更新」區段由在下列物件上輸入的更新來填入：

* 使用者
* 時程表
* 劇本
* 疊代

在適用於使用者和團隊的更新區段中，您可以檢視過去90天內輸入的更新。

如果您想要在90天限制之外檢視使用者或團隊進行的所有更新，您可以建立附註報表。 報告不應具有顯示使用者或團隊所有更新的時間篩選器。 如需詳細資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 代表其他使用者輸入評論時的限制

Adobe Workfront管理員和群組管理員可以其他使用者身份登入，並在Workfront中執行輸入註釋等動作。

如需詳細資訊，請參閱 [以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

以其他使用者身份登入並新增註解時，請考慮下列事項：

* 代表其他使用者所做的任何評論都會在評論中標示。

* 群組管理員可以代表其他人發表評論，但無法刪除該評論。 只有Adobe Workfront管理員可以刪除他們代表其他使用者所做的評論。

* Workfront或群組管理員只有在以使用者身分登出並以本身身分登入時，才能編輯他們代表其他使用者新增的評論。

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
