---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新區段概觀
description: 物件的「更新」區段會顯示使用者對物件所做的註解，或是追蹤物件變更的系統更新。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 7c458a41cd5376b746c93e9ed8e4f379a0ed1f4b
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 4%

---

# 更新區段概觀

<!--take "Beta" references out when we remove the beta-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在「預覽」環境中可用。</span>

>[!NOTE]
>
>我們目前正在重新設計Adobe Workfront中的評論體驗。
>
>如需有關新評論體驗的詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>您可以存取下列物件的新體驗：
> * 問題， <span class="preview">專案、任務和檔案</span>.
   >
   >     當您啟用註解Beta版體驗時，即可使用此功能。
   >
   >     此功能僅適用於「更新」區段，不適用於以下區域：
   >
   >     * 首頁
   >     * 清單中的摘要面板
   >     * 時程表中的摘要面板
>
> * 目標

   >
   >   新的註解體驗是目標的預設值。 您必須有其他授權才能存取Workfront目標。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    如需有關對目標發表註解的資訊，請參閱 [在Adobe Workfront目標中管理目標註解](../../workfront-goals/goal-management/manage-goal-comments.md).


物件的「更新」區段會顯示使用者對物件所做的註解，或是追蹤物件變更的系統更新。

## 更新區段概觀

根據您從哪個環境存取更新，更新區段中的資訊會有不同的組織方式。

### 目前更新區段的總覽

物件的「更新」區段會顯示過去90天內進行的最近200項更新。

![](assets/updates-tab-before-unified-experience-for-issues.png)

目前的「更新」段落顯示下列資訊：

* 使用者所做的評論和對這些評論的回覆。
* 系統更新，這是Workfront建立的資訊性訊息，用來記錄物件上的特定事件。 例如，您可以使用系統更新來擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

會針對下列物件顯示「更新」段落：

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
     <li>劇本</li> 
     <li>任務</li> 
     <li>範本</li> 
     <li>範本任務</li> 
     <li>時程表</li> 
     <li>使用者</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Beta版評論體驗中「更新」區段的概觀

![](assets/updates-tab-after-unified-experience-for-issues.png)

「更新」區段會在新評論體驗的下列標籤中顯示資訊：

* **註解**：顯示使用者所做的評論和對這些評論的回覆。 如需有關更新新註解體驗中物件的資訊，請參閱 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).
* **系統活動**：顯示系統更新，這些資訊性訊息是Workfront為記錄物件上的特定事件而建立的訊息。 例如，您可以使用系統更新來擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

目前，您可以使用以下物件的測試版註解體驗來新增註解並回覆更新：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><p>目標</p>
     <p>這是目標的預設體驗</p>
     </li> 
     <li><span class="preview">專案</span></li>
     </ul> </td> 
   <td> 
    <ul> 
     <li>問題</li> 
     <li><span class="preview">任務</span></li>
     <li><span class="preview">文件</span></li>
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 也會出現在較高層級物件上的更新

對特定物件更新所做的評論或回覆也會顯示在較高等級物件的「更新」區段中。

例如，當您將更新新增到任務時，該更新會出現在任務的更新區段和包含任務的專案的更新區段中。

>[!NOTE]
>
>啟用新的註解Beta版體驗時，註解會顯示在下列較高等級的物件上：
>
>* 問題
>* <span class="preview">專案</span>
>* <span class="preview">任務</span>
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
> 無法在新註解Beta版體驗中回覆系統更新。 如需詳細資訊，請參閱 [新的評論體驗](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

## 「更新」區段的限制

團隊的「更新」區段以及代表其他使用者輸入更新時，有一些限制。

### 使用者和團隊的限制

您無法更新團隊。 團隊的「更新」區段由在下列物件上輸入的更新填入：

* 使用者
* 時程表
* 劇本
* 疊代

在適用於使用者和團隊的更新區段，您可以檢視在過去90天內輸入的更新。

如果您想要在90天上限之外檢視使用者或團隊進行的所有更新，您可以建立報表以記錄附註。 報告不應有顯示使用者或團隊所有更新的時間篩選器。 如需詳細資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 代表其他使用者輸入評論時的限制

Adobe Workfront管理員和群組管理員可以其他使用者身分登入，並在Workfront中執行動作，例如輸入註解。 (如需詳細資訊，請參閱 [以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) 代表其他使用者所做的任何評論都會顯示在評論上。

群組管理員可以代表其他人發表評論，但無法刪除該評論。 只有Adobe Workfront管理員可以刪除他們代表其他使用者所做的評論。

## 使用分錄報表檢視工作專案的系統更新

「日誌專案」報表會從專案、任務和問題的「更新」區域顯示系統更新。

報表可讓您檢視：

* 已發生多少個狀態變更
* 刪除任務或問題時
* 重要自訂欄位中的值在專案過程中如何變更
* 專案過程中變更了哪些重要日期
* 如果優先順序在專案過程中改變
* 如果專案所有者變更

如需詳細資訊，請參閱 [報告更新區域](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
