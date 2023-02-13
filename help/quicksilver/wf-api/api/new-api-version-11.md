---
content-type: api
navigation-topic: api-navigation-topic
title: API 11版的新功能
description: Adobe Workfront API已新增ReportBudgedHour作為報表資源。 它提供DekededHour中不存在的參考欄位、核心欄位和預設欄位。
author: John
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 2%

---

# API 11版的新功能

* [新增資源](#added-resources)
* [移除的資源](#removed-resources)
* [修改的資源](#modified-resources)

## 新增資源 {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableDekededHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">訪問器</li> 
     <li style="font-weight: bold;">客戶</li> 
     <li style="font-weight: bold;">使用者  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">客戶  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">客戶  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReportableDekededHour {#reportablebudgetedhour}

Adobe Workfront API已新增ReportBudgedHour作為報表資源。 它提供DekededHour中不存在的參考欄位、核心欄位和預設欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>分配日期是在資源計畫員中為小時數編製預算的一週的第一天（星期日）。</p> </li> 
     <li> <p style="font-weight: bold;">預算小時數 </p> <p>預算小時數是資源需要在項目上完成的工作的資源管理器預算的小時數</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>指派給特定可報告預算小時物件的唯一Workfront ID。</p> </li> 
     <li style="font-weight: bold;">planedDekededHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>指派給特定專案的不重複Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>指派給特定工作角色的不重複Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>指派給特定使用者的不重複Workfront ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">專案</p> <p>與ReportableDekededHour關聯的項目。</p> </li> 
     <li> <p style="font-weight: bold;">角色</p> <p>與RepourableDekededHour關聯的職務職責。</p> </li> 
     <li> <p style="font-weight: bold;">使用者</p> <p>與ReportableDekededHour關聯的用戶。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">名稱</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>預設欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">名稱</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">計數</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">報表 </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 移除的資源 {#removed-resources}

未移除API v11的資源。

## 修改的資源 {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">核准</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">指派</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">基線任務</a> </li> 
     <li><a href="#category" class="MCXref xref">類別</a> </li> 
     <li><a href="#company" class="MCXref xref">公司</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">客戶</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">客戶偏好設定</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">文件</a> </li> 
     <li><a href="#iteration" class="MCXref xref">反覆項目</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">配置範本</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">里程碑路徑</a> </li> 
     <li><a href="#note" class="MCXref xref">備註</a> </li> 
     <li><a href="#optask" class="MCXref xref">Op 任務</a> </li> 
     <li><a href="#parameter" class="MCXref xref">參數</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">專案組合</a> </li> 
     <li><a href="#program" class="MCXref xref">方案</a> </li> 
     <li><a href="#project" class="MCXref xref">專案</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">風險</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">排程報表</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">任務</a> </li> 
     <li><a href="#team" class="MCXref xref">團隊</a> </li> 
     <li><a href="#template" class="MCXref xref">範本</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">模板分配</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">模板任務</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">時程表</a> </li> 
     <li><a href="#update" class="MCXref xref">更新「</a>」 </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">工作 </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions對象表示一組權限。 然後，這組權限便可與存取層級相關聯。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>以下欄位添加了可能的值BUDGETING_INFORMATION。 這可讓有權編輯計畫員中的優先順序和預算小時數的用戶。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

如果使用者沒有必要存取Workfront中物件的權限，可以要求存取該物件。 AccessRequest物件代表此請求。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">動作</p> <p>新增可能的值BUDGETING_INFORMATION。 這可讓有權編輯計畫員中的優先順序和預算小時數的用戶。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

AccessRule對象表示自定義訪問級別中的規則集，該規則確定用戶如何共用他們建立的項目。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>以下欄位添加了可能的值BUDGETING_INFORMATION。 這可讓有權編輯計畫員中的優先順序和預算小時數的用戶。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 核准 {#approval}

給定的工作項（如任務、文檔或時間表）可能要求主管或其他用戶簽出該工作項。 Approval對象表示簽出工作項的操作。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接欄位<p style="font-weight: normal;">以下欄位添加了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定，不能在1900年之前或2200年之後設定關聯對象的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">plandedStartDate</li>
    </ul><p style="font-weight: normal;">為了在計算EAC時透明度（完成時估計），已將下列欄位新增至公用API。</p>
    <ul>
     <li><p style="font-weight: bold;">bcw</p><p style="font-weight: normal;">「已掙值」(Reaked Value)也稱為「已執行工作的預算成本」(BCWP)，它是一個項目績效度量，表示在計算此度量時實際完成的任務金額的預算成本。 對於任務，BCWP =實際完成百分比x任務預算。 對於項目，BCWP = SUM（所有父任務和單個任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「計畫值」也稱為「已計畫的工作成本」(BCWS)，它是一個項目績效度量，表示在計算此度量時應完成的任務量的預算成本。 對於任務，BCWS =計畫完成百分比x任務預算。 對於項目，BCWS = SUM（所有父任務和單個任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下欄位添加了可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">標幟CURRENCY的欄位如下</p>
    <ul>
     <li style="font-weight: bold;">projectDekededCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">下列欄位已從核准物件中移除。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">已將下列欄位新增至核准物件。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">從核准物件中移除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">新增至核准物件。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

ApprovalPath對象是批准流程中的分支。 審批路徑基於與審批流程關聯的對象的狀態。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">新增可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

ApprovalProcess對象是多步驟審批，可與項目、任務或問題關聯。

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

### 指派 {#assignment}

分配對象表示工作項與被分配用於處理該工作項的用戶、團隊或組之間的連接。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">新增可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 基線任務 {#baselinetask}

基線是項目效能在給定時刻的快照。 它們會儲存專案的關鍵資訊，例如關鍵日期、進度、成本和收入值。 建立基線時，也會根據該基線的基線任務捕獲任務資訊。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">新增可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 類別 {#category}

類別物件是自訂表單。 您可以建立此物件的報表，也可以在其他物件報表中顯示。

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

### 公司 {#company}

公司物件代表由人員集合組成的組織。 公司與使用者或專案相關聯。

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

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td> <p style="font-weight: normal;">下列動作已新增至CustomEnum物件</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查詢</td> 
   <td> <p>已將下列查詢新增至CustomEnum物件</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶 {#customer}

客戶物件代表使用Workfront例項的組織。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">新增可能的值： </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ（項目條件）</li> 
       <li style="font-weight: normal;">CONDITION_TASK（任務條件）</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK（問題條件）  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>動作</td> 
   <td> <p style="font-weight: normal;">已將下列動作新增至客戶物件</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶偏好設定 {#customerpreferences}

CustomerPreferences物件代表客戶為其Workfront例項所設定的偏好設定集。

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>名稱</p> <p style="font-weight: normal;">新增可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy（密碼複雜性要求）</li> 
       <li style="font-weight: normal;"> password:password.minimumLength（最小密碼長度）</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout（行動工作階段逾時）</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff（用戶超時）</li> 
       <li style="font-weight: normal;">時間表：default.timesheet.manualrole（手動控制角色）</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole(config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole(config.proofhq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 文件 {#document}

文檔對象表示檔案（如書面材料、影像或其他形式的資訊）。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td> <p>已將下列操作添加到文檔對象中。</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofPtaigs</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 反覆項目 {#iteration}

小版本對象表示單個敏捷小版本。 反覆項目是用於計畫和完成敏捷故事的離散時間段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>已將下列欄位添加到小版本對象中。</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">點已完成</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 配置範本 {#layout-template}

「佈局模板」(Layout Template)對象表示佈局元素的特定排列，如主菜單、導航面板或「首頁」區域。 版面範本可指派給使用者、團隊、群組或工作角色。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">已新增此欄位，如果「配置範本」設定為在「工作清單」和「日曆」中顯示到期日的時間戳，則此欄位是布林值參數，如果設定為隱藏時間戳，則此參數的值為true；如果設定為隱藏時間戳，則此參數為false。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>預設欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 里程碑路徑 {#milestonepath}

里程碑是任務指示上的標籤，表示它是項目中的關鍵點。 通常用於表示重大事件，例如項目的某一階段或一組關鍵活動的完成。 MilestonePath對象是里程碑的集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已新增此欄位，且是布林參數，如果物件作用中，則值為true；如果物件不作用，則為false。 設定為「活動」的對象會顯示在下拉菜單和「預先輸入」欄位中，並可附加到其他對象。 未設定為「活動」的對象在要附加到其他對象的下拉菜單和預鍵入欄位中不可見。  </p> </li> 
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

### 備註 {#note}

Note物件是對Workfront物件所做的註解或更新。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>已將下列欄位新增至Note物件。</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>贊</p> <p style="font-weight: normal;">已新增</p> </li> 
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
   <td colspan="2">直接欄位<p style="font-weight: normal;">以下欄位添加了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定，不能在1900年之前或2200年之後設定關聯對象的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">plandedStartDate</li>
    </ul><p style="font-weight: normal;">OpTask新增了下列欄位。</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">看板板對象的唯一Workfront ID。</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">「完成百分比」是一個參數，將以百分比傳回已完成的問題量。</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">工作  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>搜尋欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>工作</p> <p style="font-weight: normal;">已移除</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>預設欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> <p>OpTask對象中添加了以下操作</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 參數 {#parameter}

參數物件是自訂欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">新增可能的值TYAH(Typeahead)。</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">已新增此欄位，並參照所參考物件的物件程式碼。 可在 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 專案組合 {#portfolio}

Portfolio物件是專案的集合，這些專案會爭奪相同的資源，通常是金錢或人員來完成。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>說明</p> <p style="font-weight: normal;">已新增驗證器MAX_LENGTH，其指定說明的長度不超過4000個字元。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 方案 {#program}

Program對象是產品組合中的子集，可在其中將類似項目分組。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>說明</p> <p style="font-weight: normal;">已新增驗證器MAX_LENGTH，其指定說明的長度不超過4000個字元。</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">已新增此欄位，且是布林參數，如果物件作用中，則值為true；如果物件不作用，則為false。 設定為「活動」(Active)的對象會顯示在下拉菜單和「預先輸入」(Type-ahead)欄位中，並可附加到其他對象。 未設定為「活動」的對象在要附加到其他對象的下拉菜單和預鍵入欄位中不可見。  </p> </li> 
     <li style="font-weight: bold;"> <p>名稱 </p> <p style="font-weight: normal;">已新增驗證器MAX_LENGTH，其指定名稱的長度不超過255個字元。  </p> </li> 
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

### 專案 {#project}

專案是Workfront內的工作項目，是Workfront協助人們工作的主要建置要素。 專案物件代表一組具有共同特定目標的工作。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接欄位<p style="font-weight: normal;">以下欄位添加了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定，不能在1900年之前或2200年之後設定關聯對象的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">plandedStartDate</li>
    </ul><p style="font-weight: normal;">為了在計算EAC時透明度（完成時估計），已將下列欄位新增至公用API。</p>
    <ul>
     <li><p style="font-weight: bold;">bcw</p><p style="font-weight: normal;">「已掙值」(Reaked Value)也稱為「已執行工作的預算成本」(BCWP)，它是一個項目績效度量，表示在計算此度量時實際完成的任務金額的預算成本。 對於任務，BCWP =實際完成百分比x任務預算。 對於項目，BCWP = SUM（所有父任務和單個任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「計畫值」也稱為「已計畫的工作成本」(BCWS)，它是一個項目績效度量，表示在計算此度量時應完成的任務量的預算成本。 對於任務，BCWS =計畫完成百分比x任務預算。 對於項目，BCWS = SUM（所有父任務和單個任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">標幟CURRENCY的欄位如下</p>
    <ul>
     <li style="font-weight: bold;">projectDekededCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">下列欄位已從專案物件中移除。</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已新增</p> </li> 
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
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitingDecision</p> <p style="font-weight: normal;">此欄位已新增，且是布林參數，若校樣正在等待決策，則值為true；若非，則為false。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef對象表示「隊列」，該「項目」已發佈到「服務台」區域，允許用戶向其提交問題。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>以下欄位添加了可能的值BUDGETING_INFORMATION。 這可讓有權編輯計畫員中的優先順序和預算小時數的用戶。</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

ReservedTime對象表示在用戶的個人時間上指定的天數，表示用戶將無法工作。

ReservedTime資源已添加標誌REPOURABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>以下欄位刪除了標誌NOT_GROUPABLE。</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>已從ReservedTime對象中刪除以下欄位。</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>任務</p> <p style="font-weight: normal;">已移除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>作業</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>編輯</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

ResourcePlannerFilter對象是一組規則，它確定將在Oracle Resource Planner中顯示哪些物料。

ResourcePlannerFilter資源添加了標誌SHARABLE。 物件沒有其他變更。

### 風險 {#risk}

風險對象表示可能阻止項目按時或在預算內完成的事件。 在規劃階段的項目中增加風險，以便在批准任何工作之前找出潛在障礙。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>Risk對象中添加了以下欄位：</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">最初建立對象的用戶ID。</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Workfront中的使用者提交物件的日期。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>上次更新日期參數將返回對對象進行上次更新的日期，</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID是一個參數，將返回更新對象的上次用戶的用戶的用戶ID。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> <p style="font-weight: normal;">RIsk對象中添加了以下引用欄位。</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 排程報表 {#scheduledreport}

ScheduledReport對象表示已配置為計畫傳送的報告。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">新增下列可能值：</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，他們的答案使經理能夠了解項目與產品組合目標的一致程度。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">新增可能的值TYAH(Typeahead)  </p> </li> 
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
   <td colspan="2">直接欄位<p style="font-weight: normal;">以下欄位添加了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定，不能在1900年之前或2200年之後設定關聯對象的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">plandedStartDate</li>
    </ul><p style="font-weight: normal;">為了在計算EAC時透明度（完成時估計），已將下列欄位新增至公用API。</p>
    <ul>
     <li><p style="font-weight: bold;">bcw</p><p style="font-weight: normal;">「已掙值」(Reaked Value)也稱為「已執行工作的預算成本」(BCWP)，它是一個項目績效度量，表示在計算此度量時實際完成的任務金額的預算成本。 對於任務，BCWP =實際完成百分比x任務預算。 對於項目，BCWP = SUM（所有父任務和單個任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「計畫值」也稱為「已計畫的工作成本」(BCWS)，它是一個項目績效度量，表示在計算此度量時應完成的任務量的預算成本。 對於任務，BCWS =計畫完成百分比x任務預算。 對於項目，BCWS = SUM（所有父任務和單個任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下欄位添加了可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">已從Task對象中刪除以下欄位。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Task對象中添加了以下欄位。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">已移除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已新增</p> </li> 
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
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">此欄位已添加到Team對象中。 「敏捷估計類型」可決定如何估計動態的工作負載。 如果以小時計算，則此為新增至文章的「計畫小時數」。 如果以點數預估，則每個點會根據點的設定方式，在動態中新增數個「計畫小時」（預設為8小時）。 敏捷估計類型的可能值為：</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS(Story Points)</li> 
       <li style="font-weight: normal;">小時（小時）</li> 
       <li style="font-weight: normal;">LEGACY_POINTS（小時作為點）  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 範本 {#template}

範本物件代表專案的模式。 您可以從範本建立專案，以節省時間。 模板包含「團隊」和「任務」，當使用「模板」時，這些「任務」將被複製到項目。

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
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriiress</p> <p style="font-weight: normal;">已新增</p> </li> 
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

### 模板分配 {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">新增可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 模板任務 {#templatetask}

TemplateTask對象表示屬於模板的Task。 在使用模板的項目中，模板任務變為任務。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p style="font-weight: normal;">以下欄位添加了可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriiress</p> <p style="font-weight: normal;">已新增</p> </li> 
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
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">已移除</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新 {#update}

Workfront中的工作項目可以更新，讓使用者隨時了解目前狀態。 更新對象表示其中一個更新。 使用者可輸入更新，或由Workfront系統建立。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">新增可能的值referenceObjectCustomData(enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查詢</td> 
   <td> <p style="font-weight: normal;">以下查詢已添加到更新對象。</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> <p style="font-weight: normal;">將下列動作新增至User物件。</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查詢</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td> <p style="font-weight: normal;">將下列動作新增至User物件。</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledgeMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledgedAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查詢</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">已新增</p> </li> 
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
   <td colspan="2">直接欄位<p style="font-weight: normal;">以下欄位添加了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定，不能在1900年之前或2200年之後設定關聯對象的日期。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">planedCompletionDate</li>
     <li style="font-weight: bold;">plandedStartDate</li>
    </ul><p style="font-weight: normal;">為了在計算EAC時透明度（完成時估計），已將下列欄位新增至公用API。</p>
    <ul>
     <li><p style="font-weight: bold;">bcw</p><p style="font-weight: normal;">「已掙值」(Reaked Value)也稱為「已執行工作的預算成本」(BCWP)，它是一個項目績效度量，表示在計算此度量時實際完成的任務金額的預算成本。 對於任務，BCWP =實際完成百分比x任務預算。 對於項目，BCWP = SUM（所有父任務和單個任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「計畫值」也稱為「已計畫的工作成本」(BCWS)，它是一個項目績效度量，表示在計算此度量時應完成的任務量的預算成本。 對於任務，BCWS =計畫完成百分比x任務預算。 對於項目，BCWS = SUM（所有父任務和單個任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">以下欄位添加了可能的值ET。 此值表示「已用月」的時間單位，它指的是與週末或節假日無關的月份。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">已從Work對象中刪除以下欄位。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">已將以下欄位添加到Work對象中。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">已移除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
