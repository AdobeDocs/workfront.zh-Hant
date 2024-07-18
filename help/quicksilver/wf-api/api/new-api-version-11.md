---
content-type: api
navigation-topic: api-navigation-topic
title: API 11版的新增功能
description: ReportableBudgedHour已新增至Adobe Workfront API作為報表的資源。 它具有BudgetedHour中不存在的參考欄位、核心欄位和預設欄位。
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3573'
ht-degree: 2%

---

# API 11版的新增功能

* [已新增資源](#added-resources)
* [已移除資源](#removed-resources)
* [已修改的資源](#modified-resources)

## 新增的資源 {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetedHour](#reportablebudgetedhour)

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
     <li style="font-weight: bold;">存取子ID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">存取子</li> 
     <li style="font-weight: bold;">客戶</li> 
     <li style="font-weight: bold;">使用者  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">物件代碼</li> 
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
     <li style="font-weight: bold;">物件ID</li> 
     <li style="font-weight: bold;">物件代碼  </li> 
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
     <li style="font-weight: bold;">物件代碼</li> 
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
     <li style="font-weight: bold;">licenseType</li> 
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
     <li style="font-weight: bold;">其他規則</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">物件代碼</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReportableBudgetedHour {#reportablebudgetedhour}

ReportableBudgedHour已新增至Adobe Workfront API作為報表的資源。 它具有BudgetedHour中不存在的參考欄位、核心欄位和預設欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>配置日期是您在「資源規劃工具」中編列時數預算的一週的第一天（星期日）。</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>預算時數是資源管理員預算專案上資源需要完成的工作的時數</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>指派給特定可報告預算時數物件的唯一Workfront ID。</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>指派給特定專案的唯一Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>指派給特定工作角色的唯一Workfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>指派給特定使用者的唯一Workfront ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">專案</p> <p>ReportableBudgetedHour相關聯的專案。</p> </li> 
     <li> <p style="font-weight: bold;">角色</p> <p>與ReportableBudgetedHour相關聯的工作角色。</p> </li> 
     <li> <p style="font-weight: bold;">使用者</p> <p>ReportableBudgetedHour相關聯的使用者。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">名稱</li> 
     <li style="font-weight: bold;">物件代碼</li> 
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
   <td>營運</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">計數</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">報告 </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 已移除的資源 {#removed-resources}

未移除API v11的資源。

## 已修改的資源 {#modified-resources}

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
     <li><a href="#accessrule" class="MCXref xref">存取規則</a> </li> 
     <li><a href="#approval" class="MCXref xref">核准</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">核准路徑</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">工作分派</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">基準線任務</a> </li> 
     <li><a href="#category" class="MCXref xref">類別</a> </li> 
     <li><a href="#company" class="MCXref xref">公司</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">客戶</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">客戶喜好設定</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">檔案</a> </li> 
     <li><a href="#iteration" class="MCXref xref">反複專案</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">配置範本</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">里程碑路徑</a> </li> 
     <li><a href="#note" class="MCXref xref">附註</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">引數</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">程式</a> </li> 
     <li><a href="#project" class="MCXref xref">專案</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">校訂核准</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">保留時間</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">風險</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">排程報告</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">任務</a> </li> 
     <li><a href="#team" class="MCXref xref">團隊</a> </li> 
     <li><a href="#template" class="MCXref xref">範本</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">範本指派</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">範本任務</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">時程表</a> </li> 
     <li><a href="#update" class="MCXref xref">更新</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">使用者附註</a> </li> 
     <li><a href="#work" class="MCXref xref">工作</a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions物件代表一組許可權。 然後可以將這組許可權與存取層級相關聯。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>下列欄位新增了可能的值BUDGETING_INFORMATION。 這允許具有許可權的使用者編輯規劃工具中的優先順序和預算時數。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

如果使用者無權存取Workfront中他們需要的物件，他們可以請求存取該物件。 AccessRequest物件代表此要求。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">動作</p> <p>已新增可能的值BUDGETING_INFORMATION。 這允許具有許可權的使用者編輯規劃工具中的優先順序和預算時數。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 存取規則 {#accessrule}

AccessRule物件代表自訂存取層級中的規則集，可決定使用者如何共用他們建立的專案。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>下列欄位新增了可能的值BUDGETING_INFORMATION。 這允許具有許可權的使用者編輯規劃工具中的優先順序和預算時數。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 核准 {#approval}

指定的工作專案，例如工作、檔案或時程表，可能需要主管或其他使用者登出該工作專案。 Approval物件代表在工作專案上簽核的動作。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接欄位<p style="font-weight: normal;">下列欄位新增了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定相關物件上的日期不能設定在1900年之前或2200年之後。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintdate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">下列欄位已新增到公用API，以透明方式計算EAC （預估完成成本）。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">「已執行工作之預算成本(BCWP)」也稱為「盈餘值」，是一種專案績效量度，代表計算此量度時實際完成之任務量的預算成本。 若為作業，BCWP =實際完成百分比x作業預算。 對於專案，BCWP = SUM（所有父系和個別任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「已排程工作之預算成本(BCWS)」也稱為計畫值，是專案效能量度，代表計算此量度時應該完成之任務量的預算成本。 若為工作，BCWS =計畫完成百分比x工作預算。 對於專案，BCWS = SUM（所有父系和個別任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">下列欄位新增了可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">工作單位</li>
    </ul><p style="font-weight: normal;">下列欄位已新增標幟CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">專案淨值</li>
    </ul><p style="font-weight: normal;">下列欄位已從核准物件中移除。</p>
    <ul>
     <li style="font-weight: bold;">保留時間ID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">下列欄位已新增至核准物件。</p>
    <ul>
     <li style="font-weight: bold;">storyPoint</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>保留時間</p> <p style="font-weight: normal;">已從核准物件移除  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">已新增至「核准」物件。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

ApprovalPath物件是核准流程中的分支。 「核准路徑」是以與「核准流程」相關聯之物件的狀態為基礎。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">新增可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

ApprovalProcess物件是可與專案、任務或問題相關聯的多步驟核准。

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

### 指派 {#assignment}

工作指派物件代表工作專案與指派處理該工作專案的使用者、專案團隊或群組之間的連線。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>工作單位 </p> <p style="font-weight: normal;">新增可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 基準線任務 {#baselinetask}

基準線是專案在指定時間的效能快照。 這類檔案會儲存專案的關鍵資訊，例如關鍵日期、進度、成本和收入值。 當您建立基準線時，也會擷取該基準線之基準線工作上的工作資訊。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">新增可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 類別 {#category}

類別物件是自訂表單。 您可以建立此物件的報表，也可以在其他物件報表中顯示它。

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

### 公司 {#company}

Company物件代表由人員集合組成的組織。 公司與使用者或專案相關聯。

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
   <td> <p>下列查詢已新增到CustomEnum物件</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">任務條件</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶 {#customer}

Customer物件代表使用Workfront例項的組織。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumType</p> <p style="font-weight: normal;">新增可能的值： </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ （專案狀態）</li> 
       <li style="font-weight: normal;">CONDITION_TASK （工作條件）</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK （問題條件）  </li> 
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
   <td> <p style="font-weight: normal;">下列動作已新增至Customer物件</p> 
    <ul> 
     <li style="font-weight: bold;">Goalenabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 客戶喜好設定 {#customerpreferences}

CustomerPreferences物件代表客戶已針對其Workfront例項設定的偏好設定集。

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
       <li style="font-weight: normal;">password：password.eauthPolicy （密碼複雜性要求）</li> 
       <li style="font-weight: normal;"> password：password.minimumLength （最小密碼長度）</li> 
       <li style="font-weight: normal;">密碼：mobileSessionTimeout （行動工作階段逾時）</li> 
       <li style="font-weight: normal;"> project.mgmt：default.project.usertimeoff （使用者休假）</li> 
       <li style="font-weight: normal;">時程表：default.timesheet.manualrole （手動控制角色）</li> 
       <li style="font-weight: normal;">proof：defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof：defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole)  </li> 
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

Document物件代表檔案（例如書面材料、影像或其他形式的資訊）。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td> <p>下列動作已新增至Document物件。</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 反覆項目 {#iteration}

反複專案物件代表單一敏捷反複專案。 反複專案是用來規劃和完成敏捷內文的離散時段。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>下列欄位已新增至版序物件。</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">完成點數</li> 
     <li style="font-weight: bold;">總點數  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 版面配置範本 {#layout-template}

「版面配置範本」物件代表版面配置元素的特定排列，例如主功能表、導覽面板或「首頁」區域。 版面配置範本可以指派給使用者、團隊、群組或工作角色。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">此欄位已新增，是一個布林引數，如果「版面配置範本」設定為在工作清單和行事曆中顯示到期日的時間戳記，則值為true；如果設定為隱藏時間戳記，則值為false。  </p> </li> 
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

里程碑是任務的標籤，表示它是專案中的關鍵點。 通常用於表示重大事件，例如專案某個階段或一組關鍵活動的完成。 MilestonePath物件是里程碑的集合。

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

### 備註 {#note}

Note物件是在Workfront物件上所做的註解或更新。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>下列欄位已新增至Note物件。</p> 
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

OpTask物件通常稱為「問題」。 問題指工作專案，通常表示發生問題而無法完成任務或專案。 問題也可以是服務檯請求。 變更單、請求和錯誤也是問題。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接欄位<p style="font-weight: normal;">下列欄位新增了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定相關物件上的日期不能設定在1900年之前或2200年之後。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">下列欄位已新增至OpTask。</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">Kanban展示板物件的唯一Workfront ID。</p></li>
     <li style="font-weight: bold;"><p>percentcomplete</p><p style="font-weight: normal;">完成百分比是將傳回問題完成數量的引數（百分比）。</p></li>
     <li style="font-weight: bold;">storyPoint</li>
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
     <li style="font-weight: bold;"> <p>percentcomplete</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> <p>下列動作已新增至OpTask物件</p> 
    <ul> 
     <li style="font-weight: bold;">bulkmove</li> 
     <li style="font-weight: bold;">copyissue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 參數 {#parameter}

Parameter物件是自訂欄位。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>顯示型別</p> <p style="font-weight: normal;">新增可能的值TYAH （自動提示）。</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">此欄位已新增，並參考參考參考物件的物件程式碼。 您可以在<a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>中找到所有物件的物件程式碼。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 專案組合 {#portfolio}

Portfolio物件是競爭相同資源（通常是金錢或人力）的專案集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>說明</p> <p style="font-weight: normal;">新增驗證器MAX_LENGTH，指定說明長度不得超過4000個字元。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 方案 {#program}

計畫物件是投資組合的子集，其中類似的專案可以分組在一起。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>說明</p> <p style="font-weight: normal;">新增驗證器MAX_LENGTH，指定說明長度不得超過4000個字元。</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">此欄位已新增，且是布林引數，如果物件為作用中，則值為true，否則為false。 設定為「作用中」的物件會出現在下拉式選單和預先輸入欄位中，並可附加到其他物件。 未設定為「作用中」的物件在下拉式選單和要附加至其他物件的預先輸入欄位中不可見。  </p> </li> 
     <li style="font-weight: bold;"> <p>名稱 </p> <p style="font-weight: normal;">新增驗證器MAX_LENGTH，指定名稱長度不得超過255個字元。  </p> </li> 
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

專案是Workfront內的工作專案，也是Workfront協助人們完成工作的主要建置組塊。 Project物件代表具有共同特定目標的一組任務。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接欄位<p style="font-weight: normal;">下列欄位新增了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定相關物件上的日期不能設定在1900年之前或2200年之後。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">下列欄位已新增到公用API，以透明方式計算EAC （預估完成成本）。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">「已執行工作之預算成本(BCWP)」也稱為「盈餘值」，是一種專案績效量度，代表計算此量度時實際完成之任務量的預算成本。 若為作業，BCWP =實際完成百分比x作業預算。 對於專案，BCWP = SUM（所有父系和個別任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「已排程工作之預算成本(BCWS)」也稱為計畫值，是專案效能量度，代表計算此量度時應該完成之任務量的預算成本。 若為工作，BCWS =計畫完成百分比x工作預算。 對於專案，BCWS = SUM（所有父系和個別任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">下列欄位已新增標幟CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">專案淨值</li>
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

ProofApproval物件代表直接連線至校訂的核准。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isWaitingDecision</p> <p style="font-weight: normal;">此欄位已新增，並且是布林引數，如果校訂正在等待決定，則值為true，否則為false。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef物件代表佇列，這是已發佈至服務檯區域的專案，可讓使用者向其提交問題。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>下列欄位新增了可能的值BUDGETING_INFORMATION。 這允許具有許可權的使用者編輯規劃工具中的優先順序和預算時數。</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### 保留時間 {#reservedtime}

ReservedTime物件代表在使用者個人時間中指定的天數，表示使用者將無法工作。

ReservedTime資源已新增旗標REPORTABLE。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>下列欄位已移除標幟NOT_GROUPABLE。</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefId</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>下列欄位已從ReservedTime物件中移除。</p> 
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
   <td>營運</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>編輯</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

ResourcePlannerFilter物件是一組規則，可決定要在資源規劃工具中顯示哪些專案。

ResourcePlannerFilter資源已新增SHARABLE標幟。 物件沒有其他變更。

### 風險 {#risk}

風險物件代表可能阻止專案按時完成或在預算內完成的事件。 在計畫階段中會為專案新增風險，以在核准任何工作之前識別潛在障礙。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p>下列欄位已新增至Risk物件：</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredById</p> <p style="font-weight: normal;">最初建立物件的使用者識別碼。</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>使用者在Workfront中提交物件的日期。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>上次更新日期引數會傳回對物件進行上次更新的日期，</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>上次更新者ID是將傳回上次更新物件之使用者的使用者ID的引數。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> <p style="font-weight: normal;">下列參考欄位已新增至RIsk物件。</p> 
    <ul> 
     <li style="font-weight: bold;">輸入者</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 排程報告 {#scheduledreport}

ScheduledReport物件代表已設定為排程傳送的報表。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">已新增下列可能值：</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScorecardQuestion {#scorecardquestion}

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，而他們的答案可讓經理瞭解專案與產品組合目標的對齊程度。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>顯示型別</p> <p style="font-weight: normal;">新增可能的值TYAH （自動提示）  </p> </li> 
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
   <td colspan="2">直接欄位<p style="font-weight: normal;">下列欄位新增了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定相關物件上的日期不能設定在1900年之前或2200年之後。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintdate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">下列欄位已新增到公用API，以透明方式計算EAC （預估完成成本）。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">「已執行工作之預算成本(BCWP)」也稱為「盈餘值」，是一種專案績效量度，代表計算此量度時實際完成之任務量的預算成本。 若為作業，BCWP =實際完成百分比x作業預算。 對於專案，BCWP = SUM（所有父系和個別任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「已排程工作之預算成本(BCWS)」也稱為計畫值，是專案效能量度，代表計算此量度時應該完成之任務量的預算成本。 若為工作，BCWS =計畫完成百分比x工作預算。 對於專案，BCWS = SUM（所有父系和個別任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">下列欄位新增了可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">工作單位</li>
    </ul><p style="font-weight: normal;">下列欄位已從Task物件中移除。</p>
    <ul>
     <li style="font-weight: bold;">保留時間ID</li>
    </ul><p style="font-weight: normal;">下列欄位已新增至Task物件。</p>
    <ul>
     <li style="font-weight: bold;">storyPoint</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>保留時間</p> <p style="font-weight: normal;">已移除  </p> </li> 
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

Team物件是可指派至工作專案的「使用者」集合。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">此欄位已新增至Team物件。 敏捷估計型別決定如何估計劇本的工作負載。 如果以時數來預估，這是新增到劇本的計畫時數。 如果以點為單位進行預估，則每個點都會根據點的設定方式（預設為8小時），將數個計畫時數新增到劇本中。 「敏捷估算型別」可能的值包括：</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS （劇本點）</li> 
       <li style="font-weight: normal;">HOURS (Hours)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS （以小時表示點）  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 範本 {#template}

Template物件代表專案的模式。 可以從範本建立專案以節省時間。 範本包含團隊和任務，在使用範本時將會複製到專案。

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
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>所有優先順序</p> <p style="font-weight: normal;">已新增</p> </li> 
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

### 範本指派 {#templateassignment}

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
     <li style="font-weight: bold;"> <p>工作單位</p> <p style="font-weight: normal;">新增可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 範本任務 {#templatetask}

TemplateTask物件代表屬於Template一部分的Task。 範本任務會成為使用範本之專案中的任務。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p style="font-weight: normal;">下列欄位新增了可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">工作單位</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>集合欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>所有優先順序</p> <p style="font-weight: normal;">已新增</p> </li> 
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
   <td>核心欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>物件代碼</p> <p style="font-weight: normal;">已移除</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新 {#update}

Workfront中的工作專案可以更新，以隨時通知使用者目前的狀態。 Update物件代表其中一項更新。 更新可由使用者輸入，或由Workfront系統建立。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">新增可能的值referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata)  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>查詢</td> 
   <td> <p style="font-weight: normal;">下列查詢已新增到Update物件。</p> 
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
   <td> <p style="font-weight: normal;">下列動作已新增至User物件。</p> 
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

### 使用者附註 {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td> <p style="font-weight: normal;">下列動作已新增至User物件。</p> 
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

Work物件是Task和OpTask都繼承的公用介面，並在兩者之間共用公用程式碼。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接欄位<p style="font-weight: normal;">下列欄位新增了驗證器AT_DATE_BEFORE_YEAR和AT_DATE_AFTER_YEAR。 這些驗證器指定相關物件上的日期不能設定在1900年之前或2200年之後。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintdate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">下列欄位已新增到公用API，以透明方式計算EAC （預估完成成本）。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">「已執行工作之預算成本(BCWP)」也稱為「盈餘值」，是一種專案績效量度，代表計算此量度時實際完成之任務量的預算成本。 若為作業，BCWP =實際完成百分比x作業預算。 對於專案，BCWP = SUM（所有父系和個別任務的BCWP值）。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">「已排程工作之預算成本(BCWS)」也稱為計畫值，是專案效能量度，代表計算此量度時應該完成之任務量的預算成本。 若為工作，BCWS =計畫完成百分比x工作預算。 對於專案，BCWS = SUM（所有父系和個別任務的BCWS值）。</p></li>
    </ul><p style="font-weight: normal;">下列欄位新增了可能的值ET。 此值代表經過的月時間單位，不考慮週末或假日。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">工作單位</li>
    </ul><p style="font-weight: normal;">下列欄位已從工作物件中移除。</p>
    <ul>
     <li style="font-weight: bold;">保留時間ID</li>
    </ul><p style="font-weight: normal;">下列欄位已新增至Work物件。</p>
    <ul>
     <li style="font-weight: bold;">storyPoint</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>保留時間</p> <p style="font-weight: normal;">已移除  </p> </li> 
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
