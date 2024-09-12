---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect資料字典
description: 本頁包含有關Workfront Data Connect中資料結構和內容的資訊。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: c3e18716aa74ed91e21e542437a017586a58d0b3
workflow-type: tm+mt
source-wordcount: '4294'
ht-degree: 4%

---

# Workfront Data Connect資料字典

本頁包含有關Workfront Data Connect中資料結構和內容的資訊。

>[!NOTE]
>
>Data Connect中的資料每四小時會重新整理一次，因此最近的變更可能不會立即顯示。

## 表格型別

在「資料連線」中您可以運用許多表格型別，以提供最深入分析的方式檢視您的Workfront資料。

* **目前的資料表**

  「目前」表格所反映的資料與Workfront中的資料、每個物件及其目前狀態類似。 不過，它比Workfront內的延遲要低很多。

* **事件資料表**

  「事件」表格會追蹤Workfront中的每筆變更記錄：亦即，每次物件變更狀態時，系統都會建立記錄以顯示變更發生時間、變更人員及變更內容。 因此，此表格對時間點比較很有用。 此表格僅包含過去三年的記錄。

* **每日記錄表**

  「每日歷史記錄」表格提供「事件」表格的縮寫版本，顯示每個物件的每日狀態，而非每個個別事件發生時的狀態。 因此，此表可用於趨勢分析。

<!-- Custom table -->

## 實體關係圖

Workfront中的物件（以及您的Data Connect資料湖中的物件）不僅是由其個別值所定義，也是由其與其他物件的關係所定義。 下面的實體關係圖提供資料連線中物件關係的高階對應。 您可以使用下列連結來檢視和下載圖表：

[資料連線實體關係圖](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>實體關係圖表是進行中的工作，因此僅供參考，且可能會變更。

## 日期型別

有許多日期物件可提供特定事件發生時間的相關資訊。

* `DL_LOAD_TIMESTAMP`：此日期用於內部參考，並反映資料載入目前、事件或每日記錄表格的時間。 此日期不應用於資料分析，且計畫在Workfront資料湖的測試階段期間移除。
* `CALENDAR_DATE`：此日期僅出現在「每日歷史記錄」表格中。 此表格記錄了`CALENDAR_DATE`中指定的每個日期在11:59 UTC時的資料外觀。
* `BEGIN_EFFECTIVE_TIMESTAMP`：此日期同時存在於「事件」和「每日歷史記錄」表格中，且記錄記錄將記錄目前資料列中的值&#x200B;_變更為_&#x200B;的確切時間。
* `END_EFFECTIVE_TIMESTAMP`：此日期同時存在於「事件」和「每日歷史記錄」表格中，而且記錄記錄將目前資料列中的值&#x200B;_從_&#x200B;變更為其他資料列中的值的確切時間。 若要允許在`BEGIN_EFFECTIVE_TIMESTAMP`和`END_EFFECTIVE_TIMESTAMP`上的查詢之間進行，此值絕不為Null，即使沒有新值也是如此。 在記錄仍有效的情況下（亦即值未變更），`END_EFFECTIVE_TIMESTAMP`的值將為2300-01-01。

## 術語表

下表將Workfront中的物件名稱（及其在介面和API中的名稱）與其在Data Connect中的對等名稱建立關聯。

<table>
  <thead>
    <tr>
        <th>Workfront實體名稱</th>
        <th>介面參考</th>
        <th>API參考 | 標籤</th>
        <th>資料湖表格</th>
        <th>關係欄位</th>
        <th>關係表格與欄位</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>存取層級</td>
        <td>存取層級</td>
        <td>ACSLVL | 存取層級</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>不是關聯性；用於內部應用程式<br>USER_CURRENT | USERID<br>不是關聯性；用於內部應用程式<br>在OBJCODE欄位中識別的物件識別碼<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>存取規則</td>
        <td>共用</td>
        <td>ACSURL | 共用</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ACCESSOROBJCODE欄位中識別的物件識別碼<br>Self<br>ANCESTOROBJCODE欄位中識別的物件識別碼<br>USERS_CURRENT | USERID<br>在SECURITYOBJCODE欄位中識別的物件識別碼<br>不是關聯性；用於內部應用程式用途</td>
    </tr>
    <tr>
        <td>核准路徑</td>
        <td>核准路徑</td>
        <td>ARVPTH | 核准</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID （自身） <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | USERID<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>核准流程</td>
        <td>核准流程</td>
        <td>ARVPRC | 核准流程</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID （自身） <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>自我<br>使用者_目前 | USERID<br>USERS_CURRENT | USERID<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>核准步驟</td>
        <td>核准步驟</td>
        <td>ARVSTP | 核准階段</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID （自我） <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>核准者狀態</td>
        <td>核准者狀態</td>
        <td>封存 | 核准者狀態</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td>APPROVERSTATUSID （自身）<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>在APPROVABLEOBJCODE欄位中識別的物件識別碼<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | 使用者ID <br>使用者_目前 | USERID<br>USERS_CURRENT | 使用者ID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | 使用者ID<br>專案_目前 | PROJECTID<br>USERS_CURRENT | USERID<br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | 使用者ID</td>
    </tr>
    <tr>
        <td>指派</td>
        <td>指派</td>
        <td>指派 | 指定任務</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (SELF)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | 使用者ID<br>自我<br>類別_目前 | CATEGORYID<br>目前不支援的分類資料表<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>工作_目前 | TASKID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>等待核准</td>
        <td>等待核准</td>
        <td>AWAPVL | 等待核准</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID （自身） <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>目前不支援存取要求資料表<br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>專案_目前 | PROJECTID<br>角色_目前 | ROLEID<br>使用者_目前 | USERID<br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID<br>團隊_目前 | TEAMID<br>時程表_目前 | TIMESHEETID<br>使用者_目前 | 使用者ID</td>
    </tr>
    <tr>
        <td>基準線</td>
        <td>基準線</td>
        <td>BLIN | 基線</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID (SELF)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>專案_目前 | PROJECTID<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>基準線任務</td>
        <td>基準線任務</td>
        <td>BSTSK | 基準線任務</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>基準線_目前 | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>專案_目前 | PROJECTID<br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>計費率</td>
        <td>費率或覆寫率</td>
        <td>評等 | 收費率</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (SELF)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>指定任務_目前 | ASSIGNMENTID<br>目前不支援的分類資料表<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>目前不支援非人工資源類別資料表<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>在OBJCODE欄位<br>PROJECTS_CURRENT中識別的物件識別碼 | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>角色_目前 | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>不是關聯性；用於內部應用程式<br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | 使用者ID</td>
    </tr>
    <tr>
        <td>計費記錄</td>
        <td>計費記錄</td>
        <td>帳單 | 付費記錄</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID （本身）<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>CATEGORY_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>目前不支援的商業發票資料表<br>USERS_CURRENT | 使用者ID <br>專案_目前 | PROJECTID   <br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>預訂</td>
        <td>預訂</td>
        <td>預訂 | 預訂</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID (SELF)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>自我<br>使用者_目前 | USERID<br>USERS_CURRENT | USERID<br>目前不支援非人工資源類別資料表<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>在OBJOBJCODE欄位<br>PROJECTS_CURRENT中識別的物件識別碼 | PROJECTID <br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID     <br>範本_目前 | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>在TOPOBJCODE欄位中識別的物件識別碼</td>
    </tr>
    <tr>
        <td>類別</td>
        <td>自訂表單</td>
        <td>CTGY | 類別</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID （自身）<br>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>自我<br>使用者_目前 | 使用者ID<br>群組_目前 | GROUPID <br>USERS_CURRENT | 使用者ID <br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>類別參數</td>
        <td>自訂表單欄位</td>
        <td>CTGYPA | 類別引數</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID （自身）<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>Self<br>CATEGORY_CURRENT | 目前不支援CATEGORYID<br>引數群組表格<br>PARAMETERS_CURRENT | 引數    <br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>公司</td>
        <td>公司</td>
        <td>CMPY | 公司</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>Self<br>使用者_目前 | 使用者ID <br>群組_目前 | GROUPID<br>USERS_CURRENT | 使用者ID <br>RATECARD_CURRENT | RATECARDID<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>自訂季度</td>
        <td>自訂季度</td>
        <td>CSTQRT | 自訂季度</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID （自我） <br>SYSID</td>
        <td>Self<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>條件、優先順序、嚴重性、狀態</td>
        <td>系統 | 自訂列舉</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>*記錄型別是透過'enumClass'屬性識別。 下列是預期的型別：<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | 使用者ID<br>群組_目前 | GROUPID</td>
    </tr>
    <tr>
        <td>文件</td>
        <td>文件</td>
        <td>檔案 | 檔案</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASLEID eversionid<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>目前不支援檔案要求表格<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | 使用者ID<br>NOTE_CURRENT | NOTEID<br>根據DOCOBJCODE值<br>OPTASK_CURRENT的變數 | OPTASKID<br>USER_CURRENT | 使用者ID<br>PORTFOLIO_目前 | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | 目前不支援PROJECTID<br>發行版本資料表<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>根據TOPOBJCODE值<br>USER_CURRENT的變數 | 使用者ID</td>
    </tr>
    <tr>
        <td>文件核准</td>
        <td>文件核准</td>
        <td>DOCAPL | 檔案核准</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | 使用者識別碼<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>備註_目前 | NOTEID<br>USERS_CURRENT | 使用者ID <br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>文件資料夾</td>
        <td>文件資料夾</td>
        <td>DOCFLD | 檔案資料夾</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID （自身）<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>自我<br>使用者_目前 | 使用者ID<br>OPTASKS_CURRENT | OPTASKID<br>反複專案_目前 | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_目前 | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMID    <br>專案_目前 | PROJECTID <br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID     <br>範本_目前 | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | 使用者ID</td>
    </tr>
    <tr>
        <td>DocumentProvideMetadata</td>
        <td>檔案提供中繼資料</td>
        <td>檔案 | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID （自我） <br>SYSID</td>
        <td>Self<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>Documentprovider</td>
        <td>文件提供者</td>
        <td>DOCPROP | 檔案提供者</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID （自身）<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | 使用者ID    <br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>檔案提供者設定</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID （自身）<br>SYSID</td>
        <td>Self<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>檔案版本</td>
        <td>文件版本</td>
        <td>DOCV | 檔案版本</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSIDS<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFONWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | 目前不支援USERID<br>外部ID<br>校訂核准狀態表格<br>USER_CURRENT | USERID<br>目前不支援的校訂資料表<br>USER_CURRENT | 目前不支援USERID<br>校訂階段資料表</td>
    </tr>
    <tr>
        <td>匯率</td>
        <td>匯率</td>
        <td>運算式 | 匯率</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID （自身）<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>自我<br>專案_目前 | PROJECTID <br>不是關聯性；用於內部應用程式<br>TEMPLATES_CURRENT | 範本ID  </td>
    </tr>
    <tr>
        <td>費用</td>
        <td>費用</td>
        <td>費用 | 費用</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (SELF) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>類別_目前 | CATEGORYID<br>USERS_CURRENT | 使用者ID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | 使用者識別碼<br>物件識別碼（在OBJCODE欄位<br>PROJECTS_CURRENT中識別） | PROJECTID <br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>在TOPOBJCODE欄位中識別的物件識別碼</td>
    </tr>
    <tr>
        <td>費用類型</td>
        <td>費用類型</td>
        <td>EXPTYP | 費用型別</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>物件ID <br>SYSID  </td>
        <td>不是關聯性；用於內部應用程式<br>Self<br>在OBJCODE欄位中識別的物件識別碼<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>群組</td>
        <td>群組</td>
        <td>群組 | 群組</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | 使用者ID<br>類別_目前 | CATEGORYID<br>USER_CURRENT | 不支援USERID<br>Self<br>配置範本資料表<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>小時</td>
        <td>小時</td>
        <td>HOUR | 小時</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>ID taskid<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>類別_目前 | CATEGORYID<br>目前不支援分類資料表<br>不是關聯性；用於內部應用程式<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>不是Workfront關係；用於整合至外部系統<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | 使用者ID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | 使用者ID<br>PROJECT_CURRENT | PROJECTID<br>不是關聯性；用於內部應用程式<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>時程表_目前 | 時程表ID</td>
    </tr>
    <tr>
        <td>時數類型</td>
        <td>時數類型</td>
        <td>小時 | 小時型別</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>物件ID</td>
        <td>不是關聯性；用於內部應用程式<br>本身<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>反覆項目</td>
        <td>反覆項目</td>
        <td>ITRN | 反複專案</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORY_CURRENT | 類別ID<br>使用者_目前 | 使用者ID <br>自我<br>使用者_目前 | 使用者ID <br>使用者_目前 | 使用者ID <br>不是關聯性；用於內部應用程式<br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>日誌輸入項目</td>
        <td>日誌輸入項目</td>
        <td>JRNLE | 日誌專案</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID<br>PORTASIDPORTASID folioid<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>目前不支援稽核記錄表格<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>公司_目前 | 公司ID <br>DOCUMENTS_CURRENT | DOCUMENTID <br>目前不支援的檔案共用表格<br>USERS_CURRENT | 使用者ID<br>費用_目前 | EXPENSEID<br>HOURS_CURRENT | HOURID<br>目前不支援Initiative資料表<br>Self<br>在OBJCODE欄位中識別的物件識別碼<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_目前 | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>專案_目前 | PROJECTID <br>在SUBOBJCODE欄位中識別的物件識別碼<br>目前不支援訂閱資料表<br>不是關聯性；用於內部應用程式目的<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>時程表_目前 | TIMESHEETID<br>在TOPOBJCODE欄位<br>USERS_CURRENT中識別的物件識別碼 | 使用者ID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (SELF)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>外部ID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>里程碑</td>
        <td>里程碑</td>
        <td>英里 | 里程碑</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | 里程碑ID</td>
    </tr>
    <tr>
        <td>里程碑路徑</td>
        <td>里程碑路徑</td>
        <td>MPATH | 里程碑路徑</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | 使用者ID<br>本身</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>非勞動力資源</td>
        <td>NLBR | 非人工資源</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID <br>SYSID  </td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>Self<br>使用者_目前 | 使用者ID <br>群組_目前 | GROUPID<br>USERS_CURRENT | 使用者ID <br>目前不支援非人工資源類別資料表<br>不是關聯性；用於內部應用程式    </td>
    </tr>
    <tr>
        <td>非工作日</td>
        <td>排程例外狀況</td>
        <td>NONWKD | 非工作日</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID （自身）<br>物件ID <br>排程識別碼<br>SYSID <br>使用者ID  </td>
        <td>Self<br>在OBJCODE欄位<br>SCHEDULES_CURRENT中識別的物件識別碼 | SCHEDULEID <br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID  </td>
    </tr>
    <tr>
        <td>備註</td>
        <td>備註</td>
        <td>注意 | 注意</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHHOPTASKID<br>ATTACHHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTANDORSEMENTID<br>PARENTID<br>PARENTID tjournalentryid<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFACTIONID<br>PROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID 28}使用者ID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>變數，依據ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | 目前不支援USERID<br>稽核記錄資料表<br>COMPANIES_CURRENT | 公司ID <br>DOCUMENT_CURRENT | DOCUMENTID<br>不是Workfront關係；用於與外部系統整合<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>變數（依據NOTEOBJCODE<br>OPTASK_CURRENT） | OPTASKID<br>USER_CURRENT | USERID<br>目前不支援的簽署資料表<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_目前 | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>目前不支援校訂動作資料表<br>目前不支援校訂資料表<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>時程表_目前 | TIMESHEETID<br>變數，依據TOPOBJCODE<br>USER_CURRENT | 使用者ID</td>
    </tr>
    <tr>
        <td>物件整合</td>
        <td>物件整合</td>
        <td>物件 | 物件整合</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   （自我）<br>物件ID <br>SYSID  </td>
        <td>LINKEDOBJECTCODE欄位<br>Self<br>識別之物件的識別碼在OBJCODE欄位<br>識別之物件的識別碼不是關聯性；用於內部應用程式用途  </td>
    </tr>
    <tr>
        <td>物件類別</td>
        <td>物件類別</td>
        <td>物件 | 物件類別</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>Self<br>在OBJCODE欄位中識別的物件識別碼<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>Op 任務</td>
        <td>問題，請求</td>
        <td>OPTASK | 問題</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID RESOLVEOPTASKID<br>QUEUETOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | 使用者ID<br>類別_目前 | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | 使用者ID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | 目前不支援ITERATIONID<br>Kanban面板資料表<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | 使用者ID<br>PROJECT_CURRENT | PROJECTID<br>目前不支援佇列定義資料表<br>目前不支援佇列主題資料表<br>OPTASK_CURRENT | OPTASKID<br>專案_目前 | PROJECTID<br>TASK_CURRENT | TASKID<br>變數，依據RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>變數，依據SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | 使用者ID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>參數</td>
        <td>自訂欄位</td>
        <td>引數 | 引數</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID （自身）<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>目前不支援引數篩選資料表<br>Self<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>參數選項</td>
        <td>參數選項</td>
        <td>POPT | 引數選項</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID （本身） <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>本身<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>入口網站區段</td>
        <td>報告</td>
        <td>PTLSEC | 報告</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID （自身）<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID <br>UIFILTERS_CURRENT | 篩選<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | 使用者ID <br>使用者_目前 | 使用者識別碼<br>物件識別碼欄位<br>Self<br>PREFERENCES_CURRENT中識別的物件識別碼 | PREFERENCEID<br>USERS_CURRENT | 使用者ID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>目前不支援排程報告表格<br>不是關聯性；用於內部應用程式目的<br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>入口網站頁簽</td>
        <td>儀表板</td>
        <td>PTLTAB | 儀表板</td>
        <td>PORTALTABLES_CURRENT<br>PORTALTABLES_DAILY_HISTORY<br>PORTALTABLES_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID （自身）<br>SYSID<br>USERID</td>
        <td>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 不支援USERID <br>入口網站設定檔資料表<br>Self<br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID  </td>
    </tr>
    <tr>
        <td>入口網站頁籤區段</td>
        <td>儀表板區段</td>
        <td>PRTBSC | 入口網站頁簽區段</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (SELF)<br>SYSID</td>
        <td>行事曆入口網站區段目前不支援<br>外部區段表格目前不支援<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>在PORTALSECTIONOBJCODE欄位<br>PORTALTABS_CURRENT中識別的物件識別碼 | PORTALTABID<br>Self<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>報表最後檢視者</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID （自身）<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID （本身）<br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID  </td>
    </tr>
    <tr>
        <td>專案組合</td>
        <td>專案組合</td>
        <td>連線埠 | Portfolio</td>
        <td>Portfolio_CURRENT<br>PORTFOLIO_每日_歷史記錄<br>PORTFOLIO_事件<br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>目前不支援計分卡表格<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | 使用者ID<br>群組_目前 | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | 使用者ID<br>本身</td>
    </tr>
    <tr>
        <td>喜好設定</td>
        <td>檢視、篩選、分組、報告定義</td>
        <td>PROSET | 偏好設定</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID （自我） <br>SYSID  </td>
        <td>不是關聯性；用於內部應用程式<br>本身<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>方案</td>
        <td>方案</td>
        <td>PRGM | 計畫</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>USER_CURRENT | 使用者ID<br>群組_目前 | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | 使用者ID<br>PORTFOLIO_目前 | PORTFOLIOID<br>自行</td>
    </tr>
    <tr>
        <td>專案</td>
        <td>專案</td>
        <td>專案 | 專案</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTERDBYID<br>GROUPID<br>LASTCONDITIONNOTEID{12 {LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOOLID<br>SCHEDULEID 25}SPONSORID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID<br><br></td>
        <td>不是Workfront關係；用於與外部系統整合<br>目前不支援的計分卡表格<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>類別_目前 | 類別ID<br>公司_目前 | 公司ID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | 使用者ID<br>APPROVALSTEPS_CURRENT | 目前不支援APPROVALSTEPID<br>計分卡表格<br>USER_CURRENT | 使用者ID<br>群組_目前 | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>使用者_目前 | 目前不支援USERID<br>Pop帳戶資料表<br>PORTFOLIO_目前 | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | 目前不支援PROGRAMID<br>Self<br>佇列定義資料表<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | 使用者ID<br>TEAM_CURRENT | TEAMID<br>範本_目前 | 範本ID</td>
    </tr>
    <tr>
        <td>費率卡</td>
        <td>費率卡</td>
        <td>RTCRD |評等卡</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (SELF) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>類別ID<br>使用者_目前 | 使用者ID <br>使用者_目前 | 使用者ID    <br>Self<br>在SECURITYOBJCODE欄位中識別的物件識別碼<br>在SOURCEOBJCODE欄位中識別的物件識別碼<br>不是關聯性；用於內部應用程式用途  </td>
    </tr>
    <tr>
        <td>報告資料夾</td>
        <td>報告資料夾</td>
        <td>RPTFDR | 報告資料夾</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID （自身） <br>SYSID  </td>
        <td>自我<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>保留時間</td>
        <td>（個人）休假</td>
        <td>REVT | 休假</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID （自身） <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Self<br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | 使用者ID  </td>
    </tr>
    <tr>
        <td>資源集區</td>
        <td>資源集區</td>
        <td>RSPL | 資源集區</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID （自身）<br>SYSID  </td>
        <td>USERS_CURRENT | 使用者ID <br>使用者_目前 | USERID <br>Self<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>RTF 備註</td>
        <td>RTF 備註</td>
        <td>RHNOTE | RTF備註</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID （自身） <br>SYSID  </td>
        <td>自我<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>RTF引數值</td>
        <td>RTF引數值</td>
        <td>RCHVAL | RtfParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID （本身） <br>SYSID  </td>
        <td>目前不支援引數值資料表<br>本身<br>不是關聯性；用於內部應用程式  </td>
    </tr>
    <tr>
        <td>風險</td>
        <td>風險</td>
        <td>風險 | 風險</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGEERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID （自身）<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | 使用者ID <br>專案_目前 | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br>不是關聯性；用於內部應用程式<br>TEMPLATES_CURRENT | 範本ID</td>
    </tr>
    <tr>
        <td>風險類型</td>
        <td>風險類型</td>
        <td>RSKTYP | 風險型別</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>角色</td>
        <td>職務角色</td>
        <td>角色 | 工作角色</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | 不支援USERID<br>配置範本資料表<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>排程</td>
        <td>排程</td>
        <td>時程 | 排程</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | 使用者ID<br>群組_目前 | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>步驟核准者</td>
        <td>步驟核准者</td>
        <td>SPAPVR | 階段核准者</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>角色_目前 | ROLEID<br>Self<br>不是關聯性；用於內部應用程式<br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | 使用者ID</td>
    </tr>
    <tr>
        <td>任務</td>
        <td>任務</td>
        <td>任務 | 任務</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>ID{13 LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>類別_目前 | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | 使用者ID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | 使用者ID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>群組目前 | GROUPID<br>ITERATIONS_CURRENT | 目前不支援ITERATIONID<br>Kanban面板資料表<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | 目前不支援PROJECTID<br>遞回規則資料表<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>使用者_目前 | 使用者ID<br>自我<br>團隊目前 | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>前置任務</td>
        <td>前置任務</td>
        <td>前置任務 | 前置任務</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID （自我）<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Self<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID <br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>團隊</td>
        <td>團隊</td>
        <td>TEAMOB | 團隊</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | 使用者ID<br>群組_目前 | 不支援GROUPID<br>配置範本資料表<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | 使用者ID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>小組成員</td>
        <td>其他團隊、團隊成員</td>
        <td>TEAMMB | 團隊成員</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID （本身）<br>USERID</td>
        <td>不是關聯性；用於內部應用程式<br>TEAMS_CURRENT | TEAMID<br>自我<br>使用者_目前 | 使用者ID</td>
    </tr>
    <tr>
        <td>團隊成員角色</td>
        <td>小組成員角色</td>
        <td>團隊成員 | 團隊成員角色</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID （本身）<br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>團隊_目前 | TEAMID<br>自我<br>使用者_目前 | 使用者ID</td>
    </tr>
    <tr>
        <td>範本</td>
        <td>範本</td>
        <td>範本 | 範本</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br> TEAMID<br>TEMPLATEID （自助）</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>類別_目前 | CATEGORYID<br>公司_目前 | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | 使用者ID<br>群組_目前 | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>使用者_目前 | 使用者ID <br>RATECARD_CURRENT | RATECARDID<br>程式目前 | 目前不支援PROGRAMID<br>佇列定義資料表<br>SCHEDULES_CURRENT | SCHEDULEID <br>不是關聯性；用於內部應用程式<br>TEAMS_CURRENT | TEAMID<br>自行</td>
    </tr>
    <tr>
        <td>範本指派</td>
        <td>範本指派</td>
        <td>任務 | 範本指派</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (SELF)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | 使用者ID<br>類別_目前 | CATEGORYID<br>USERS_CURRENT | USERID<br>在OBJCODE欄位<br>ROLES_CURRENT中識別的物件識別碼 | ROLEID<br>不是關聯性；用於內部應用程式<br>TEAMS_CURRENT | TEAMID<br>目前不支援Team Timelineable資料表<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>範本任務</td>
        <td>範本任務</td>
        <td>TTSK | 範本任務</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMAMTIMELINEABLEID<br>TEMPLATEID<br>PLATEMID tetaskid（自身）<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | 使用者ID<br>類別_目前 | 類別ID<br>使用者_目前 | 使用者ID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>筆記_目前 | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>目前不支援週期性規則資料表<br>ROLES_CURRENT | ROLEID<br>不是關聯性；用於內部應用程式<br>TEAMS_CURRENT | 目前不支援TEAMID<br>團隊時間表<br>TEMPLATES_CURRENT | TEMPLATEID<br>本身</td>
    </tr>
    <tr>
        <td>範本任務前置任務</td>
        <td>範本前置任務</td>
        <td>已暫存 | 前置任務</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID （自身）<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Self<br>不是關聯性；用於內部應用程式用途</td>
    </tr>
    <tr>
        <td>時程表</td>
        <td>時程表</td>
        <td>表格 | 時間表</td>
        <td>時程表_目前<br>時程表_每日歷史記錄<br>時程表_事件</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | 使用者ID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | 使用者ID</td>
    </tr>
    <tr>
        <td>時程表設定檔</td>
        <td>時程表設定檔</td>
        <td>TSPRO | 週期性時程表</td>
        <td>時程表設定檔_目前<br>時程表設定檔_每日歷程記錄<br>時程表設定檔_事件</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (SELF)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | 使用者ID <br>群組_目前 | GROUPID<br>不是關聯性；用於內部應用程式<br>Self</td>
    </tr>
    <tr>
        <td>UI篩選器</td>
        <td>篩選器</td>
        <td>UIFT | 篩選</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (SELF)</td>
        <td>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID <br>使用者_目前 | 使用者ID <br>物件識別碼欄位<br>PREFERENCES_CURRENT | PREFERENCEID<br>不是關聯性；用於內部應用程式目的<br>Self</td>
    </tr>
    <tr>
        <td>UI群組依據</td>
        <td>分組</td>
        <td>UIGB | 分組</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID （自我）</td>
        <td>USERS_CURRENT | 使用者ID<br>群組_目前 | GROUPID <br>USERS_CURRENT | 使用者ID <br>不是關聯性；用於內部應用程式目的<br>自行</td>
    </tr>
    <tr>
        <td>UI範本</td>
        <td>版面配置範本</td>
        <td>UITMPL | 版面配置範本</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (SELF)</td>
        <td>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID <br>使用者_目前 | 使用者ID <br>物件識別碼欄位<br>PREFERENCES_CURRENT | PREFERENCEID<br>不是關聯性；用於內部應用程式目的<br>Self</td>
    </tr>
    <tr>
        <td>使用者介面檢視</td>
        <td>檢視</td>
        <td>UIVIEW | 檢視</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (SELF)</td>
        <td>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID <br>使用者_目前 | 使用者ID <br>物件識別碼欄位<br>PREFERENCES_CURRENT | PREFERENCEID<br>不是關聯性；用於內部應用程式目的<br>Self</td>
    </tr>
    <tr>
        <td>使用者</td>
        <td>使用者</td>
        <td>使用者 | 使用者</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>MANAGERID<br>PORTALPROFILPROFILID eid<br>PREFUIID<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID<br></td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>類別_目前 | CATEGORYID<br>公司_目前 | 公司ID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>不是關聯性；用於內部應用程式<br>USER_CURRENT | 使用者ID<br>群組_目前 | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | 使用者ID<br>NOTE_CURRENT | 不支援NOTEID<br>配置範本資料表<br>USER_CURRENT | 不支援USERID<br>入口網站設定檔資料表<br>不是關聯性；用於內部應用程式<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | 排程識別碼<br>時程表設定檔_目前 | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>不是關聯性；用於內部應用程式</td>
    </tr>
    <tr>
        <td>使用者委派</td>
        <td>使用者委派</td>
        <td>超級 | 使用者委派</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID （自行）</td>
        <td>USERS_CURRENT | USERID<br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID <br>本身</td>
    </tr>
    <tr>
        <td>使用者群組</td>
        <td>其他群組</td>
        <td>USRGPS | 使用者群組</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID (SELF)</td>
        <td>群組_目前 | GROUPID <br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID <br>本身</td>
    </tr>
    <tr>
        <td>使用者角色</td>
        <td>其他角色</td>
        <td>USROL | 使用者角色</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID （自行）</td>
        <td>ROLES_CURRENT | ROLEID <br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID    <br>使用者角色集_目前 | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | 使用者偏好設定</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID （自行）</td>
        <td>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID    <br>自己</td>
    </tr>
    <tr>
        <td>使用者角色集</td>
        <td>使用者角色集</td>
        <td>URSET | 使用者角色集</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID （自行）</td>
        <td>ROLES_CURRENT | ROLEID <br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID <br>本身</td>
    </tr>
    <tr>
        <td>使用者決策</td>
        <td>使用者決策</td>
        <td>USRDEC | 使用者決策</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID （自身）<br>SYSID <br>USERID  </td>
        <td>Self<br>不是關聯性；用於內部應用程式<br>USERS_CURRENT | 使用者ID </td>
    </tr>
    <tr>
        <td>工作專案</td>
        <td>工作項目</td>
        <td>WRKITM | 工作專案</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>使用者ID <br>工作專案ID （自行）</td>
        <td>指定任務_目前 | ASSIGNMENTID <br>在OBJOBJCODE欄位<br>OPTASK_CURRENT中識別的物件識別碼 | OPTASKID    <br>專案_目前 | PROJECTID <br>不是關聯性；用於內部應用程式<br>TASKS_CURRENT | TASKID    <br>位使用者_目前 | 使用者ID    <br>自己 </td>
    </tr>
  </tbody>
</table>
