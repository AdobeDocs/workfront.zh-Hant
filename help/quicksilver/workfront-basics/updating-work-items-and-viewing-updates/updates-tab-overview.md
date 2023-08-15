---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新區段概觀
description: 物件的「更新」區段會顯示使用者對物件所做的註解，或追蹤物件變更的系統更新。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: d93d42322d62ff5eb927ca13febcb763cbec3f13
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 4%

---

# 更新區段概觀

<!--take "Beta" references out when we remove the beta-->

<!--after August 17: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/enable-fast-release-process.html?lang=en ). </span>  
<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>-->

<!--replace the note below with this at August 17: 
>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>Depending on what environment and what objects you access the commenting experience from, you might see different functionality in the Updates section. 
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>The new commenting experience is available only for the Updates section, and it is not available for the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets

-->

<!-- with October 26 release: add somewhere this:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

>[!NOTE]
>
>我們目前正在重新設計Adobe Workfront中的評論體驗。
>
>如需有關新註解體驗的詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>您可以存取下列物件的新體驗：
> * 問題、專案、任務和檔案。
>
>     當您啟用新的評論體驗時，這是可用的。
>
>     此功能僅適用於「更新」區段，不適用於下列區域：
>
>     * 首頁
>     * 清單中的摘要面板
>     * 時程表中的摘要面板
>
> * 面板區域中的目標、卡片
>
>   新的評論體驗是目標和卡的唯一體驗。 您必須額外擁有授權才能存取Workfront目標。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     當您啟用卡片上的「註解」和「系統活動」區段時，您可以在「面板」區域中新增和檢視卡片的更新。 如需詳細資訊，請參閱 [新增臨機卡到展示板](../../agile/get-started-with-boards/add-card-to-board.md).

物件的「更新」區段會顯示使用者對物件所做的註解，或追蹤物件變更的系統更新。

## 「更新」區段的總覽

根據您從哪個環境存取更新，更新區段中的資訊會有不同的組織方式。

### 目前更新區段的總覽

<!--October 26 - replace current with legacy-->

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
      </ul> </td> 
    </tr> 
  </tbody> 
  </table>

  *劇本是任務。 所有與工作相關的資訊也可用於劇本。

* 目前的「更新」段落顯示下列資訊：

   * **使用者更新**：使用者所做的評論和對這些評論的回覆。
   * **系統更新**：Workfront為記錄物件上的特定事件而建立的資訊訊息。 例如，您可以使用系統更新來擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 下列物件不會記錄系統更新：

   * 團隊
   * 範本
   * 範本任務

### 新評論體驗中「更新」區段的概觀

如需有關新註解體驗有哪些功能可用以及哪些物件的資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--update screen shot and maybe save it under a new name??? with the August 17 release-->

![](assets/updates-tab-after-unified-experience-for-issues.png)

* 「更新」區段在新註解體驗的以下標籤中顯示資訊：

   * **註解**：顯示使用者所做的評論以及對這些評論的回覆。 如需有關更新新註解體驗中物件的資訊，請參閱 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).
   * **系統活動**：顯示系統更新，這些資訊性訊息是Workfront為記錄物件上的特定事件而建立的訊息。 例如，您可以使用系統更新來擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 目前，您可以在下列物件上使用新的註解體驗來新增註解及回覆更新：

<!--replace the table with this list on August 17: 

    * Projects
    * Tasks (and stories)
    * Issues
    * Documents

    <span class="preview">
    
    * Templates
    * Template Tasks
    * Timesheets
    * Users
    * Portfolios
    * Programs
    
    >[!NOTE]
    >
    >    You cannot display the new commenting experience for iterations. 

    </span>
  
  -->

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
      <tr> 
      <td> 
        <ul> 
        <li><p>目標</p>
        <li>看板區域中的卡片*</li>
          這是唯一的目標和卡片體驗。
        </li> 
        <li>專案</li>
        </ul> </td> 
      <td> 
        <ul> 
        <li>問題</li> 
        <li>任務</li>
        <li>文件</li>
        </ul> </td> 
      </tr> 
    </tbody> 
    </table>

*當您啟用資訊卡上的「註解」和「系統活動」區段時，您可以在「展示板」區域新增和檢視資訊卡的更新。 如需詳細資訊，請參閱 [新增臨機卡到展示板](../../agile/get-started-with-boards/add-card-to-board.md).

<!--enable this when we release the new update stream to ALL other objects and only if Anna's bug was fixed to include this: 

* The following objects don't have a System Activity tab:

  * Team
  * Template
  * Template Task
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

您無法更新團隊。 專案團隊的「更新」區段由在下列物件上輸入的更新來填入：

* 使用者
* 時程表
* 劇本
* 疊代

在適用於使用者和團隊的更新區段中，您可以檢視過去90天內輸入的更新。

如果您想要在90天限制之外檢視使用者或團隊進行的所有更新，您可以建立附註報表。 報告不應具有顯示使用者或團隊所有更新的時間篩選器。 如需詳細資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 代表其他使用者輸入評論時的限制

Adobe Workfront管理員和群組管理員可以其他使用者身份登入，並在Workfront中執行輸入註釋等動作。

如需詳細資訊，請參閱 [以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

代表其他使用者所做的任何評論都會在評論中標示。

<!--might need to update this note when the new commenting experience will be the only experience; also - how will this affect the areas that will keep the old experience, like Iterations?-->

>[!NOTE]
>
>使用新的註解體驗時，註解會新增為以其他使用者身分登入的使用者，而不會顯示他們代表其他人新增註解。
>
>例如，如果Workfront管理員以其他使用者身份登入，則與評論相關聯的使用者是Workfront管理員。 如需詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


群組管理員可以代表其他人發表評論，但無法刪除該評論。 只有Adobe Workfront管理員可以刪除他們代表其他使用者所做的評論。

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
