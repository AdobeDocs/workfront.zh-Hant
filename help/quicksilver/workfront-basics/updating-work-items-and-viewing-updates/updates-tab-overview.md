---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新區段概觀
description: 「更新」區段會顯示最多200個過去90天內進行的最新更新。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# 更新區段概觀

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

對象的「更新」部分顯示用戶在跟蹤對象更改的對象或系統更新上所做的注釋。

## 「更新」區段的概觀

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

物件的「更新」區段會顯示最多200個過去90天內進行的最新更新。

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

「更新」區段顯示下列資訊：

* 用戶的評論和對這些評論的答復。
* 系統更新，這些是Workfront為記錄物件上的特定事件而建立的資訊性訊息。 例如，您可以利用系統更新擷取狀態、名稱或自訂欄位中的變更。 您的Workfront或群組管理員可以為您的物件啟用系統更新。 如需詳細資訊，請參閱 [配置系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

「更新」(Updates)部分將顯示以下對象：

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
     <li>反覆項目</li> 
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

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## 也出現在高排名對象上的更新

如下表所示，對某些對象的更新所做的答復也會出現在排名較高的對象的「更新」部分。

例如，將更新添加到任務時，該更新將出現在該任務的「更新」部分和包含該任務的項目的「更新」部分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>添加原始更新的對象</strong> </th> 
   <th> <p><strong>顯示原始更新的高級對象</strong> </p> </th> 
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
   <td>方案，Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>文件 </td> 
   <td>附加文檔的對象，項目 </td> 
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
   <td>迭代，團隊</td> 
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
>添加到系統更新的回復不會匯總到父對象。 只有子對象的直接回覆和添加到現有更新的回覆才會匯總到父對象。
>
>如需Adobe Workfront中物件階層的相關資訊，請參閱 [了解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## 「更新」一節的限制

### 使用者和團隊的限制

無法對團隊進行更新。 在以下對象上輸入的更新將填充團隊的「更新」(Updates)部分：

* 使用者
* 時程表
* 劇本
* 反覆項目

在使用者和團隊的「更新」區段中，您可以檢視過去90天內輸入的更新。

如果您想查看使用者或團隊上所進行的所有更新，超過90天的限制，您可以建立報表以取得附註。 報表不應有時間篩選器來顯示使用者或團隊所做的所有更新。 如需詳細資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 代表其他使用者輸入註解時的限制

Adobe Workfront管理員和群組管理員可以和其他使用者身分登入，並在Workfront中執行動作，例如輸入註解。 (如需詳細資訊，請參閱 [以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) 代表其他使用者提出的任何意見都會在意見中注明。

群組管理員可以代表其他人發表意見，但無法刪除該意見。 只有Adobe Workfront管理員可以刪除代表其他使用者發表的意見。

## 使用「日記帳分錄」報表查看工作項的系統更新

「日記帳分錄」報表從項目、任務和問題的「更新」區域顯示系統更新。

報表可讓您查看：

* 發生了多少個狀態更改
* 刪除任務或問題時
* 重要自訂欄位中的值在專案期間有何變更
* 專案期間有哪些重要日期變更
* 如果在項目過程中更改了優先順序
* 如果專案的擁有者已變更

如需詳細資訊，請參閱 [更新區域報告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
