---
content-type: api
navigation-topic: api-navigation-topic
title: API 13版的新功能
description: Adobe Workfront已於2021年4月22日發行API 13版。 API 13版提供第12版的下列變更。
author: Becky
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# API 13版的新功能

Adobe Workfront已於2021年4月22日發行API 13版。 API 13版提供第12版的下列變更。

## 新增資源

未為API 13版新增資源。

## 已移除資源

未移除API 13版的資源。

## 修改的資源

已針對API 13版修改下列資源。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">客戶偏好設定</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">群組 </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">版面範本</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">Op 任務</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">專案</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">任務</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">團隊</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">時程表</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">時間表配置檔案</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">用戶委派</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

AccessLevel對象與用戶關聯，並描述了決定用戶可以訪問的AccessLevelPermissions集。

有關訪問級別的詳細資訊，請參見 [存取層級如何運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>說明</b> </p> <p>已新增驗證器MAX_LENGTH，其指定說明的長度不超過4000個字元。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

BreadCrumb物件代表Workfront工作項目的父/子階層中的元素。 階層連結會指出工作項目如何融入Portfolio、專案、專案和工作的更大結構中。

如需階層連結的詳細資訊，請參閱 [新Adobe Workfront體驗中的階層連結概觀](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>您可以在 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

BurndownEvent對象表示更改小版本的組合的對象。

有關燃耗的詳細資訊，請參見 [Burndown](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> <p>以下欄位刪除了標誌NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶偏好設定 {#customerpreferences}

CustomerPreferences物件代表客戶為其Workfront例項所設定的偏好設定集。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>名稱</p> <p style="font-weight: normal;">新增可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">密碼：aemAPIKey(config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain(config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled(config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost(config.general.aem.host)</li> 
       <li style="font-weight: normal;">timeshee:default.timese.restrict.timeset.edit.owners.admins(config.timeshite.restrict.timeset.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> <p>CustomerPreferences資源中新增了下列動作。</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>引用引數：</p> 
      <ul> 
       <li> <p>首選項（映射）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

DocumentVersion對象表示檔案的特定版本（如書面材料、影像或其他形式的資訊）。

有關文檔版本的詳細資訊，請參閱 [上傳新版本的檔案](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>AEM(Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>新增標幟NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 群組  {#group}

群組物件代表一組使用者和團隊。 團體往往代表部門結構。

如需群組的詳細資訊，請參閱 [Adobe Workfront中的群組與團隊比較](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>動作</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>此動作會傳回群組的父群組（指定群組為的子群組）陣列。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

JournalEntry對象可以設定為在修改這些欄位時記錄有關特定對象欄位的資訊。 將欄位設定為作為日記帳分錄對象的一部分進行記錄時，每次修改該欄位時都將建立相應的日記帳分錄。

JournalEntry資源添加了標誌REPOURABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> <p>以下欄位移除了標幟NOT_GROUPABLE:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>以下欄位已新增標幟NOT_FILTEABLE:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 版面範本 {#layouttemplate}

Adobe Workfront管理員或群組管理員可以建立範本，以自訂Adobe Workfront中的配置元素。 LayoutTemplate物件是Adobe Workfront Classic專屬的。

如需在新Adobe Workfront體驗中代表版面範本的物件，請參閱 [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>說明</b> </p> <p>已新增驗證器MAX_LENGTH，其指定說明的長度不超過4000個字元。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder對象表示從外部文檔提供程式(如Google驅動器或Dropbox)連結的資料夾。

如需連結資料夾的詳細資訊，請參閱 [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>AEM(Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任務 {#optask}

OpTask物件通常稱為「問題」。 問題是工作項，通常表示存在問題，無法完成任務或項目。 問題也可以是服務台請求。 變更訂單、請求和錯誤也是問題。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>搜尋欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 專案 {#project}

專案是Workfront內的工作項目，是Workfront協助人們工作的主要建置要素。 專案物件代表一組具有共同特定目標的工作。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ProofApproval {#proofapproval}

ProofApproval對象表示直接連接到校樣的批准。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> <p>ProofApproval資源已新增下列欄位。</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef對象表示「隊列」，該「項目」已發佈到「服務台」區域，允許用戶向其提交問題。

如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>已新增. 可能的值包括：</p> 
      <ul> 
       <li> <p>0（自訂表單後）</p> </li> 
       <li> <p>1（自訂表單前）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任務 {#task}

任務對象表示一個工作項，必須作為實現最終目標（完成項目）的步驟執行。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>搜尋欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 團隊 {#team}

Team對象是可分配給工作項的Users的集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已新增此欄位，且是布林參數，如果物件作用中，則值為true；如果物件不作用，則為false。 設定為「活動」(Active)的對象會顯示在下拉菜單和「預先輸入」(Type-ahead)欄位中，並可附加到其他對象。 未設定為「活動」的對象在要附加到其他對象的下拉菜單和預鍵入欄位中不可見。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>預設欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 時程表 {#timesheet}

工時單對象表示一個虛擬工時單卡，它允許用戶輸入實際工時，以處理任務、項目和間接費用工時類型。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>isAtterimedDisabled</b> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>已移除</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 時間表配置檔案 {#timesheetprofile}

工時單對象表示一個虛擬工時單卡，它允許用戶輸入實際工時，以處理任務、項目和間接費用工時類型。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>isAtterimedDisabled</b> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>預設欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>isAtterimedDisabled</b> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront管理員或群組管理員可以建立範本，以自訂Adobe Workfront中的配置元素。 LayoutTemplate物件是新Adobe Workfront體驗專屬的。

如需代表Adobe Workfront Classic版面範本的物件，請參閱 [版面範本](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>UITemplate資源中添加了以下操作。</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>引用引數：</p> 
      <ul> 
       <li> <p>overrideIfExists（布林值）</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>使用引數：</p> 
      <ul> 
       <li> <p>layoutTemplateIDs(string[])</p> </li> 
       <li> <p>overrideIfExists（布林值）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 用戶委派 {#userdelegation}

UserDelegation對象表示在特定時間段內將工作從一個用戶委派到另一個用戶的行為。

UserDelegation物件已新增標幟REPOURABLE。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> <p>以下欄位刪除了標誌NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預設欄位</td> 
   <td> <p>新增下列欄位：</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 工作  {#work}

Work對象是Task和OpTask都繼承的公共介面，並且兩者之間共用公共代碼。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>搜尋欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
