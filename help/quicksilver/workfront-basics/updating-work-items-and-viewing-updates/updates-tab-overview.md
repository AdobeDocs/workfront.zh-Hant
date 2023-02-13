---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新標籤概觀
description: 「更新」標籤會顯示過去90天內最近進行的200次更新。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 799a2f3463ee98d57b13edfda8a0c93629439ea3
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 6%

---

# 更新標籤概觀

「更新」標籤會顯示過去90天內最近進行的200次更新。 您可以回覆下列物件的更新：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>專案</li> 
     <li>專案組合</li> 
     <li>計劃</li> 
     <li>範本</li> 
     <li>範本任務</li> 
     <li>任務</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>問題</li> 
     <li>反覆項目</li> 
     <li>劇本</li> 
     <li>使用者</li> 
     <li>文件</li> 
     <li>時程表</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 也出現在高排名對象上的更新

如下表所示，對某些對象的更新所做的答復也會出現在排名較高對象的「更新」(Updates)頁簽上。

例如，將更新添加到任務時，該更新將顯示在該任務的「更新」頁簽上以及包含該任務的項目的「更新」頁簽上。

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
 </tbody> 
</table>

>[!NOTE]
>
>添加到系統更新的回復不會匯總到父對象。 只有子對象的直接回覆和添加到現有更新的回覆才會匯總到父對象。

如需Adobe Workfront中物件階層的相關資訊，請參閱 [了解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 「更新」標籤的限制

### 使用者和團隊的限制

無法對團隊進行更新。 在以下對象上輸入的更新將填充團隊的「更新」(Updates)頁簽：

* 使用者
* 時程表
* 劇本
* 反覆項目

在使用者和團隊的「更新」標籤中，您可以檢視過去90天內輸入的更新。

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
