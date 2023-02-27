---
content-type: api
navigation-topic: api-navigation-topic
title: API 14版的新功能
description: Adobe Workfront於2021年9月9日發行API 14版。 API 14版提供第14版的下列變更。
author: Becky
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# API 14版的新功能

Adobe Workfront於2021年9月9日發行API 14版。 API 14版提供第14版的下列變更。

## 新增資源

未為API 14版新增資源。

## 已移除資源

未移除API 14版的資源。

## 修改的資源

已針對API 14版修改下列資源。

* [帳單記錄（帳單）](#billingrecord-bill)
* [類別(CTGY)](#category-ctgy)
* [CustomEnum(CSTEM)](#customenum-cstem)
* [客戶(CUST)](#customer-cust)
* [客戶偏好設定(CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion(DOCV)](#documentversion-docv)
* [組（組）](#group-group)
* [NoteTag(NTAG)](#notetag-ntag)
* [項目(PROJ)](#project-proj)
* [QueueDef(QUED)](#queuedef-qued)
* [資源分配(RSALLO)](#resource-allocation-rsallo)
* [角色（角色）](#role-role)
* [範本(TMPL)](#template-tmpl)
* [工時單(TSHET)](#timesheet-tshet)

### 帳單記錄（帳單） {#billingrecord-bill}

BillingRecord對象記錄可以開單的收入、小時數或費用。 此資訊可用於在外部會計系統中建立發票。

有關帳單記錄的詳細資訊，請參閱 [建立計費記錄](../../manage-work/projects/project-finances/create-billing-records.md).

BillingRecord對象已添加標籤 **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>已新增. 類別是自訂表單。 已新增此參數，以支援將自訂Forms新增至BillingRecord物件的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">參考欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>類別</b> </p> <p>已新增. 類別是自訂表單。 已新增此參數，以支援將自訂表單新增至BillingRecord物件的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">集合欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>已新增. 這表示與BillingRecord對象關聯的類別（自定義表單）的集合。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>已新增. 此動作會重新計算自訂表單欄位中的運算式。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 類別(CTGY) {#category-ctgy}

類別物件是自訂表單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p> 帳單（帳單記錄）</p> </li> 
      </ul> <p>已新增此值，以支援將自訂表單新增至BillingRecord物件的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrezendInPendingApprovalStatus</b> </p> <p>此動作會採用objID和objCode參數，並傳回布林值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum(CSTEM) {#customenum-cstem}

CustomEnum物件有助於將狀態代碼轉換為人類看得懂的文字。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">查詢</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>已新增. 此查詢支援為組和子組建立和管理狀態的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">管理組狀態</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶(CUST) {#customer-cust}

客戶物件代表使用Workfront例項的組織。

這是內部物件。

### 客戶偏好設定(CUSTPR) {#customerpreferences-custpr}

CustomerPreferences物件代表客戶為其Workfront例項所設定的偏好設定集。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>名稱</b> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>允許使用者在更新中新增影像（更新：images.toggle）</p> </li> 
      </ul> <p>此參數支援將影像添加到工作項更新中的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion(DOCV) {#documentversion-docv}

DocumentVersion對象表示檔案的特定版本（如書面材料、影像或其他形式的資訊）。

有關文檔版本的詳細資訊，請參閱 [上傳新版本的檔案](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>已新增. 如果版本與校樣相關聯，此欄位會記錄Workfront Proof上次回呼的日期和時間。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 組（組） {#group-group}

群組物件代表一組使用者和團隊。 團體往往代表部門結構。

如需群組的詳細資訊，請參閱 [Adobe Workfront中的群組與團隊比較](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubroms</b> </p> <p>已新增. 此動作會取用groupIDs陣列，並將這些群組新增為指定群組的子群組。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag(NTAG) {#notetag-ntag}

NoteTag對象表示在工作項目的更新中對用戶或團隊進行標籤的行為。

如需更新中標籤的詳細資訊，請參閱 [在更新時標籤其他人](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">作業</td> 
   <td> <p>NoteTag對象中添加了以下操作：</p> 
    <ul> 
     <li> <p><b>計數</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>報表</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 項目(PROJ) {#project-proj}

專案是Workfront內的工作項目，是Workfront協助人們工作的主要建置要素。 專案物件代表一組具有共同特定目標的工作。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>已新增.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef(QUED) {#queuedef-qued}

QueueDef對象表示「隊列」，該項目已發佈到「幫助台」區域，允許用戶向其提交問題。

如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>已新增. 此動作可透過透過請求佇列和主題群組的路徑，支援尋找請求。</p> <p>如需依路徑搜尋請求佇列的詳細資訊，請參閱 <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">在Workfront網頁應用程式中建立請求並產生草稿</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">建立及提交Adobe Workfront請求</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 資源分配(RSALLO) {#resource-allocation-rsallo}

資源分配對象表示指定項目所需資源的估計值。 此對象僅用於舊式資源規劃器。 對於新資源規劃器中的相應欄位，請使用預算小時數(BGHR)。

資源分配對象刪除了標籤 **可報告**.

### 角色（角色） {#role-role}

角色對象（作業角色）表示用戶可能填寫的功能能力或技能集，如設計人員或產品經理。

有關作業角色的資訊，請參閱 [工作角色概觀](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已新增. 如果物件為「作用中」，則此為布林值參數，如果物件為「false」，則值為true。 設定為「活動」(Active)的對象會顯示在下拉菜單和「預先輸入」(Type-ahead)欄位中，並可附加到其他對象。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預設欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 範本(TMPL) {#template-tmpl}

範本物件代表專案的模式。 可從範本建立專案，以節省時間。 範本包含團隊和任務，這些團隊和任務將複製到從範本建立的任何專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">已新增. 已新增此欄位，以支援將群組與範本建立關聯的功能。</p> <p style="font-weight: normal;">如需詳細資訊，請參閱 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">編輯專案範本</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">已新增. 已新增此欄位，以支援將群組與範本建立關聯的功能。</p> <p style="font-weight: normal;">如需詳細資訊，請參閱 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">編輯專案範本</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
