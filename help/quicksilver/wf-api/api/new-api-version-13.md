---
content-type: api
navigation-topic: api-navigation-topic
title: API 13版的新增功能
description: Adobe Workfront於2021年4月22日發行API第13版。 API版本13具有下列版本12的變更。
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# API 13版的新增功能

Adobe Workfront於2021年4月22日發行API第13版。 API版本13具有下列版本12的變更。

## 新增的資源

沒有為API版本13新增資源。

## 已移除的資源

未移除API版本13的資源。

## 已修改的資源

已針對API版本13修改下列資源。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">存取層級</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">待執行工作事件</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">客戶喜好設定</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">檔案版本</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">群組 </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">日誌專案</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
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
     <li> <p><a href="#timesheetprofile" class="MCXref xref">週期性時程表</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UIT範本</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegation</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 存取層級 {#accesslevel}

AccessLevel物件與使用者相關聯，並描述決定使用者可存取內容的AccessLevelPermissions集合。

如需存取層級的詳細資訊，請參閱 [存取層級的運作方式](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>說明</b> </p> <p>新增驗證器MAX_LENGTH，指定說明長度不得超過4000個字元。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

BreadCrumb物件代表Workfront工作專案之父/子階層中的元素。 階層連結可指出工作專案如何融入Portfolio、專案、專案和任務的較大結構。

如需階層連結的詳細資訊，請參閱 [新Adobe Workfront體驗中的階層連結概觀](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>物件代碼</b> </p> <p>物件程式碼可在以下位置找到： <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API總管</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 待執行工作事件 {#burndownevent}

BurndownEvent物件代表變更版序的下拉清單的物件。

如需待執行工作的詳細資訊，請參閱 [待執行工作](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> <p>下列欄位已移除標幟NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶喜好設定 {#customerpreferences}

CustomerPreferences物件代表客戶已針對其Workfront例項設定的偏好設定集。

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
       <li style="font-weight: normal;">密碼：aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> 密碼：aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">密碼：aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">密碼：aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">時程表：default.timesheet.restrict.timesheet.edit.owners.admins (config.timesheet.restrict.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> <p>下列動作已新增至CustomerPreferences資源。</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>採用引數：</p> 
      <ul> 
       <li> <p>偏好設定（對應）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 檔案版本 {#documentversion}

DocumentVersion物件代表檔案的特定版本（例如書面材料、影像或其他形式的資訊）。

如需檔案版本的詳細資訊，請參閱 [上傳檔案的新版本](../../documents/managing-documents/upload-new-document-version.md).

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
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>已新增旗標NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 群組  {#group}

群組物件代表一組使用者和團隊。 群組通常代表部門結構。

如需群組的詳細資訊，請參閱 [Adobe Workfront中的群組與團隊](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>動作</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>此動作會傳回群組父群組（指定群組為其子群組的群組）的陣列。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 日誌專案 {#journalentry}

JournalEntry物件可設定為每次修改特定物件欄位時，記錄這些欄位的相關資訊。 當欄位設定為記錄為日誌專案物件的一部分時，每次修改該欄位時都會建立對應的日誌專案。

JournalEntry資源已新增標幟REPORTABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> <p>下列欄位已移除標幟NOT_GROUPABLE：</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>物件代碼</b> </p> </li> 
    </ul> <p>下列欄位新增了旗標NOT_FILTERABLE：</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>Subobjid</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>Topobjid</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Adobe Workfront管理員或群組管理員可建立範本，以自訂Adobe Workfront中的版面配置元素。 LayoutTemplate物件特定於Adobe Workfront Classic。

如需代表新Adobe Workfront體驗中版面配置範本的物件，請參閱 [UIT範本](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>說明</b> </p> <p>新增驗證器MAX_LENGTH，指定說明長度不得超過4000個字元。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder物件代表連結自外部檔案提供者(例如Google Drive或Dropbox)的資料夾。

如需連結資料夾的詳細資訊，請參閱 [從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

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
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任務 {#optask}

OpTask物件通常稱為「問題」。 問題指工作專案，通常表示發生問題而無法完成任務或專案。 問題也可以是服務檯請求。 變更單、請求和錯誤也是問題。

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

專案是Workfront內的工作專案，也是Workfront協助人們完成工作的主要建置組塊。 Project物件代表具有共同特定目標的一組任務。

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

ProofApproval物件代表直接連線至校訂的核准。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> <p>下列欄位已新增到ProofApproval資源。</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>決定日期</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef物件代表佇列，這是已發佈至服務檯區域的專案，可讓使用者向其提交問題。

如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>檔案位置</b> </p> <p>已新增. 可能的值包括：</p> 
      <ul> 
       <li> <p>0 （在自訂表格之後）</p> </li> 
       <li> <p>1 （在自訂表單前）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任務 {#task}

Task物件代表作為達成最終目標（完成專案）的步驟而必須執行的工作專案。

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

Team物件是可指派至工作專案的「使用者」集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">此欄位已新增，且是布林引數，如果物件為作用中，則值為true，否則為false。 設定為「作用中」的物件會出現在下拉式選單和預先輸入欄位中，並可附加到其他物件。 未設定為「作用中」的物件在下拉式選單和要附加至其他物件的預先輸入欄位中不可見。  </p> </li> 
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

時程表物件代表虛擬時程表，可讓使用者輸入任務、專案和管理費用時數型別的實際工作時數。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>物件代碼</b> </p> <p>已移除</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 週期性時程表 {#timesheetprofile}

時程表物件代表虛擬時程表，可讓使用者輸入任務、專案和管理費用時數型別的實際工作時數。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>預設欄位</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UIT範本 {#uitemplate}

Adobe Workfront管理員或群組管理員可建立範本，以自訂Adobe Workfront中的版面配置元素。 UITemplate物件是新Adobe Workfront體驗專屬的物件。

如需在Adobe Workfront Classic中代表版面範本的物件，請參閱 [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>下列動作已新增至UITemplate資源。</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>採用引數：</p> 
      <ul> 
       <li> <p>overrideIfExists （布林值）</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>採用引數：</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists （布林值）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

UserDelegation物件代表在特定期間內將工作從一名使用者委派給另一使用者的行為。

UserDelegation物件已新增標幟REPORTABLE。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> <p>下列欄位已移除標幟NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預設欄位</td> 
   <td> <p>已新增下列欄位：</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 工作  {#work}

Work物件是Task和OpTask都繼承的公用介面，並在兩者之間共用公用程式碼。

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
