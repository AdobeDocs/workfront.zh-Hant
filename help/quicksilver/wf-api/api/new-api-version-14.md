---
content-type: api
navigation-topic: api-navigation-topic
title: API 14版的新增功能
description: Adobe Workfront於2021年9月9日發行API第14版。 API版本14具有下列版本14的變更。
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# API 14版的新增功能

Adobe Workfront於2021年9月9日發行API第14版。 API版本14具有下列版本14的變更。

## 新增的資源

沒有為API版本14新增資源。

## 已移除的資源

未移除API版本14的資源。

## 已修改的資源

已針對API版本14修改下列資源。

* [記帳記錄(BILL)](#billingrecord-bill)
* [類別(CTGY)](#category-ctgy)
* [自訂列舉(CSTEM)](#customenum-cstem)
* [客戶（客戶）](#customer-cust)
* [客戶偏好設定(CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [群組（群組）](#group-group)
* [附註標籤(NTAG)](#notetag-ntag)
* [專案（專案）](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [資源配置(RSALLO)](#resource-allocation-rsallo)
* [角色(ROLE)](#role-role)
* [範本(TMPL)](#template-tmpl)
* [時程表(TSHET)](#timesheet-tshet)

### 記帳記錄(BILL) {#billingrecord-bill}

BillingRecord物件會記錄可記帳的收入、時數或費用。 此資訊可用於在外部會計系統中建立商業發票。

如需付費記錄的詳細資訊，請參閱 [建立付費記錄](../../manage-work/projects/project-finances/create-billing-records.md).

BillingRecord物件已新增標幟 **DATA_EXTENDIABLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>已新增. 類別是自訂表單。 新增此引數是為了支援新增自訂Forms至BillingRecord物件的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">參考欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>類別</b> </p> <p>已新增. 類別是自訂表單。 新增此引數是為了支援新增自訂表單至BillingRecord物件的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">集合欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>物件類別</b> </p> <p>已新增. 這代表與BillingRecord物件關聯的類別（自訂表單）集合。</p> </li> 
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
       <li> <p> 帳單（記帳記錄）</p> </li> 
      </ul> <p>新增此值是為了支援新增自訂表單到BillingRecord物件的功能。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>此動作會採用引數objID和objCode，並傳回布林值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 自訂列舉(CSTEM) {#customenum-cstem}

CustomEnum物件可協助將狀態代碼轉換為人類看得懂的文字。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">查詢</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>已新增. 此查詢支援建立和管理群組和子群組的狀態的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">管理群組狀態</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶（客戶） {#customer-cust}

Customer物件代表使用Workfront例項的組織。

這是內部物件。

### 客戶偏好設定(CUSTPR) {#customerpreferences-custpr}

CustomerPreferences物件代表客戶已針對其Workfront例項設定的偏好設定集。

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
       <li> <p>允許使用者在更新中新增影像(updates：images.toggle)</p> </li> 
      </ul> <p>此引數支援將影像新增至工作專案更新的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

DocumentVersion物件代表檔案的特定版本（例如書面材料、影像或其他形式的資訊）。

如需檔案版本的詳細資訊，請參閱 [上傳檔案的新版本](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>已新增. 如果版本與校訂相關聯，此欄位會記錄來自Workfront Proof的上次回撥日期和時間。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 群組（群組） {#group-group}

群組物件代表一組使用者和團隊。 群組通常代表部門結構。

如需群組的詳細資訊，請參閱 [Adobe Workfront中的群組與團隊](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>已新增. 這個動作會採用一個groupID陣列，並將這些群組新增為指定群組的子群組。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 附註標籤(NTAG) {#notetag-ntag}

NoteTag物件代表在工作專案的更新中標籤使用者或團隊的動作。

如需有關在更新中標籤的詳細資訊，請參閱 [標籤其他人的更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">作業</td> 
   <td> <p>下列作業已新增至NoteTag物件：</p> 
    <ul> 
     <li> <p><b>計數</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>報告</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 專案（專案） {#project-proj}

專案是Workfront內的工作專案，也是Workfront協助人們完成工作的主要建置組塊。 Project物件代表具有共同特定目標的一組任務。

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

### QueueDef (QUED) {#queuedef-qued}

QueueDef物件代表佇列，這是已發佈至服務檯區域的專案，可讓使用者向其提交問題。

如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>已新增. 此動作支援透過請求佇列和主題群組的路徑來尋找請求的功能。</p> <p>如需依路徑搜尋請求佇列的詳細資訊，請參閱 <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">在Workfront網頁應用程式中建立請求並產生草稿</a> 在 <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">建立及提交Adobe Workfront請求</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 資源配置(RSALLO) {#resource-allocation-rsallo}

Resource Allocation物件代表指定專案所需的資源預估值。 此物件僅用於舊版資源規劃工具。 對於新資源規劃工具中的對應欄位，請使用預算時數(BGHR)。

資源配置物件已移除標幟 **可報告**.

### 角色(ROLE) {#role-role}

角色物件（工作角色）代表使用者可能填入的功能容量或技能集，例如設計師或產品經理。

有關工作角色的資訊，請參閱 [工作角色總覽](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已新增. 如果物件為「作用中」，則此為布林值引數；如果物件為「非作用中」，則此值為false。 設定為「作用中」的物件會出現在下拉式選單和預先輸入欄位中，並可附加到其他物件。</p> </li> 
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

Template物件代表專案的模式。 可以從範本建立專案以節省時間。 範本包含專案團隊和任務，這些專案將會複製到從範本建立的任何專案中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">已新增. 新增此欄位以支援將群組與範本建立關聯的能力。</p> <p style="font-weight: normal;">如需詳細資訊，請參閱 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">編輯專案範本</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">已新增. 新增此欄位以支援將群組與範本建立關聯的能力。</p> <p style="font-weight: normal;">如需詳細資訊，請參閱 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">編輯專案範本</a>.</p> </li> 
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
