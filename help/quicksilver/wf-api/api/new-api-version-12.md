---
content-type: api
navigation-topic: api-navigation-topic
title: API 12版的新功能
description: Workfront已於2020年11月12日發行API 12版。 API 12版提供第11版的下列變更
author: John
feature: Workfront API
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# API 12版的新功能

Workfront已於2020年11月12日發行API 12版。 API 12版提供第11版的下列變更

## 新增資源

下列為Workfront API 12版中的新資源。

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

BreadCrumb物件代表Adobe Workfront工作項目的父/子階層中的元素。 階層連結會指出工作項目如何融入Portfolio、專案、專案和工作的更大結構中。

如需Workfront中階層連結的詳細資訊，請參閱 [新Adobe Workfront體驗中的階層連結概觀](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

RTF欄位現在可用於更多物件。 RichTextParameterValue物件已新增至Workfront以支援此可用性。

如需詳細資訊，請參閱 [Adobe Workfront API中的RTF欄位](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## 移除的資源

未移除API 12版的資源。

## 修改的資源

已針對Workfront API 12版修改下列資源。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">公告附件</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">核准</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">日曆節</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">公司</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">客戶</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">客戶偏好設定</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">文件</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">群組 </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">Op 任務</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">參數</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">專案組合</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">方案</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">排程報表</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">任務</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">團隊</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">模板任務</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">時程表</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">使用者</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

AccessLevel對象與用戶關聯，並描述了決定用戶可以訪問的AccessLevelPermissions集。

有關訪問級別的詳細資訊，請參見 [存取層級如何運作](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions對象表示訪問、建立或修改Workfront對象的特定權限。 然後，這些權限便可與存取層級相關聯。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> <p>具有包含此權限的訪問級別的用戶可以更新工作負載平衡器中的計畫小時數。</p> <p>如需詳細資訊，請參閱 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">在管理用戶分配時更新任務計畫小時數</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器中管理用戶分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此權限的存取層級的使用者可將欄位新增至自訂表單。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此權限的訪問級別的用戶可以在系統範圍內與刪除訪問共用自定義欄位。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定義欄位和小工具的共用</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">動作</p> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> <p>具有包含此權限的訪問級別的用戶可以更新工作負載平衡器中的計畫小時數。</p> <p>如需詳細資訊，請參閱 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">在管理用戶分配時更新任務計畫小時數</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器中管理用戶分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此權限的存取層級的使用者可將欄位新增至自訂表單。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此權限的訪問級別的用戶可以在系統範圍內與刪除訪問共用自定義欄位。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定義欄位和小工具的共用</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> <p>具有包含此權限的訪問級別的用戶可以更新工作負載平衡器中的計畫小時數。</p> <p>如需詳細資訊，請參閱 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">在管理用戶分配時更新任務計畫小時數</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器中管理用戶分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此權限的存取層級的使用者可將欄位新增至自訂表單。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此權限的訪問級別的用戶可以在系統範圍內與刪除訪問共用自定義欄位。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定義欄位和小工具的共用</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

ActivityLog物件是指定Workfront校樣帳戶中發生之所有活動的完整清單。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>作業</p> </td> 
   <td> <p>已從ActivityLog對象中刪除以下操作：</p> 
    <ul> 
     <li> <p><strong>新增</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 公告附件 {#announcementattachment}

AnnotingAttachment物件代表已附加至Workfront公告的檔案。

有關公告附件的詳細資訊，請參閱 [傳送公告](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>qdoc(enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides(enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet(enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>移除下列標幟：</p> 
      <ul> 
       <li> <p>動態，</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>新增下列標幟</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>動態，</p> </li> 
       <li> <p>只讀(_O)</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>已新增此欄位，並代表使用者每天完成工作所需的小量、中量或大量工作。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>如需Workfront中「工作成果」的詳細資訊，請參閱 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作成果概觀</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 日曆節 {#calendarsection}

日曆部分是日曆報告。

如需日曆報表的詳細資訊，請參閱 [日曆報表概觀](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p style="font-weight: normal;">CalendarSection物件新增了下列欄位，以支援在日曆報表中使用自訂日期的新功能。 </p> <p style="font-weight: normal;">如需詳細資訊，請參閱 <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">在日曆報表中使用自訂日期欄位</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 公司 {#company}

公司物件代表由人員集合組成的組織。

如需公司的詳細資訊，請參閱 [建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">與公司相關聯之群組的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">公司關聯的群組。 將公司與群組關聯可讓群組管理員將群組存取權和權限延伸至公司。</p> </li> 
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
  <tr> 
   <td>動作</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">此動作會採用CustomerProductTypeEnum引數並傳回布林值，指出該客戶是否擁有該產品的帳戶。 </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled（啟用更新流中的Zoom整合）</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled(config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">已新增</p> </li> 
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
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">移除可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP(Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> <p>已將下列操作添加到文檔對象中。</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">此動作會採用documentVersonID引數（字串），並傳回指出審核者決定的地圖。</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">此動作會採用下列引數：</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID（字串）</p> </li> 
       <li> <p>reviewerDecision（字串）</p> </li> 
       <li> <p>註解（字串）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 群組  {#group}

群組物件代表一組使用者和團隊。 團體往往代表部門結構。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">指派給組的業務主管ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>業務領導者</p> <p style="font-weight: normal;">指派給組的業務主管。 業務領導者是為群組做出業務決策的人。</p> <p style="font-weight: normal;">有關業務領導者的詳細資訊，請參閱 <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">業務領導者概觀</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>此動作會採用下列引數：</p> 
      <ul> 
       <li> <p>userIDs(string[])</p> </li> 
       <li> <p>roleIDs(string[])</p> </li> 
       <li> <p>teamID（字串）</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>此動作會採用下列引數：</p> 
      <ul> 
       <li> <p>newMemberIDs(string[])</p> </li> 
       <li> <p>removedMemberDs(string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">移除可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP(Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任務 {#optask}

OpTask物件通常稱為「問題」。 問題是工作項，通常表示存在問題，無法完成任務或項目。 問題也可以是服務台請求。 變更訂單、請求和錯誤也是問題。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>訂單指明任務或事件在敏捷積壓工作中的位置。</p> <p>此欄位已移除下列標幟：
       <ul>
        <li>動態，</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>這些操作添加了參數狀態以支援新的「開始」按鈕功能，當用戶按一下該按鈕指示他們已開始處理該項時，該功能將更改工作項的狀態。</p> <p>如需詳細資訊，請參閱 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 參數 {#parameter}

參數物件是自訂欄位。

參數資源已新增標幟SHARABLE。

如需自訂欄位的詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>RTF(RTF)</p> <p>如需詳細資訊，請參閱 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API中的RTF欄位</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>RTF（帶格式的文本欄位）</p> <p>如需詳細資訊，請參閱 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API中的RTF欄位</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>標籤</strong> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">集合欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預設欄位</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>標籤</strong> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 專案組合 {#portfolio}

Portfolio物件是專案的集合，這些專案會爭奪相同的資源，通常是金錢或人員來完成。

如需產品組合的詳細資訊，請參閱 [PortfolioAdobe Workfront概觀](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">與產品組合關聯的組ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">與產品組合關聯的組。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 方案 {#program}

方案物件是產品組合內的專案子集，可將類似專案分組。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">程式關聯的組的ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">與方案關聯的組。 </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>已新增下列possibleValues:</p> 
      <ul> 
       <li> <p>PLANINED_HOURS_CONTOULING </p> <p>具有包含此權限的訪問級別的用戶可以更新工作負載平衡器中的計畫小時數。</p> <p>如需詳細資訊，請參閱 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">在管理用戶分配時更新任務計畫小時數</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器中管理用戶分配</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS。 </p> <p>具有包含此權限的存取層級的使用者可將欄位新增至自訂表單。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>具有包含此權限的訪問級別的用戶可以在系統範圍內與刪除訪問共用自定義欄位。</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定義欄位和小工具的共用</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>已新增下列possibleValues:</p> 
       <ul> 
        <li> <p>PLANINED_HOURS_CONTOULING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS。 </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 排程報表 {#scheduledreport}

ScheduledReport對象表示已配置為計畫傳送的報告。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>格式</strong> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>qdoc(enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides(enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet(enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，他們的答案使經理能夠了解項目與產品組合目標的一致程度。

如需計分卡問題的詳細資訊，請參閱 [建立計分卡](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">新增可能的值RICH（含格式的文字欄位） </p> <p style="font-weight: normal;">如需詳細資訊，請參閱 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API中的RTF欄位</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任務 {#task}

任務對象表示一個工作項，必須作為實現最終目標（完成項目）的步驟執行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>已新增此欄位，並代表使用者每天完成工作所需的小量、中量或大量工作。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>如需Workfront中「工作成果」的詳細資訊，請參閱 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作成果概觀</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>這些操作添加了參數狀態以支援新的「開始」按鈕功能，當用戶按一下該按鈕指示他們已開始處理該項時，該功能將更改工作項的狀態。</p> <p>如需詳細資訊，請參閱 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 團隊 {#team}

Team對象是可分配給工作項的Users的集合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> <p>已將下列欄位新增至團隊資源：</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>此欄位表示看板板上已完成卡的保留天數。</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此欄位將團隊與群組關聯。 這會將團隊識別為群組的一部分，並讓群組管理員可管理團隊。</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>這是布林參數，指示團隊的「工作」(Work on It)按鈕是否已配置為「開始」(Start)按鈕。 當團隊成員按一下「開始」按鈕開始處理工作項時，項目的狀態將從「新建」更改為在團隊設定中配置的狀態。</p> </li> 
     <li> <p>以下欄位允許您為單個工作項的「開始」按鈕指定自定義狀態。</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>有關「開始」按鈕的詳細資訊，請參閱 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">參考欄位</td> 
   <td> <p>已將下列欄位新增至團隊資源：</p> 
    <ul> 
     <li> <p><strong>群組</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 模板任務 {#templatetask}

TemplateTask對象表示屬於模板的Task。 在使用模板的項目中，模板任務變為任務。

有關模板任務的詳細資訊，請參閱 [編輯模板任務](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>已新增此欄位，並代表使用者每天完成工作所需的小量、中量或大量工作。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>如需Workfront中「工作成果」的詳細資訊，請參閱 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作成果概觀</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 時程表 {#timesheet}

工時單對象表示一個虛擬工時單卡，它允許用戶輸入實際工時，以處理任務、項目和間接費用工時類型。

有關工時單的詳細資訊，請參閱 [工時單概觀](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">核心欄位</td> 
   <td> <p>從時間表資源中刪除了以下欄位：</p> 
    <ul> 
     <li> <p><strong>物件代碼</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>新增下列可能值：</p> 
      <ul> 
       <li> <p>initiativeAdd(enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit(enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">有關計畫的詳細資訊，請參閱 <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">方案計畫器中的方案概覽</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 使用者 {#user}

使用者物件代表擁有Workfront中可登入並與系統互動之帳戶的人員。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> <p>已將下列欄位新增至使用者資源：</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>這代表使用者停用的日期和時間。</p> <p>如需已停用使用者的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>此欄位顯示使用者對Workfront目標的存取權。 可能的值包括：</p> 
      <ul> 
       <li> <p>無權存取</p> </li> 
       <li> <p>檢視</p> </li> 
       <li> <p>編輯</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>已將下列動作新增至使用者資源：</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>此動作會採用下列引數</p> 
      <ul> 
       <li> <p>id（字串）</p> </li> 
       <li> <p>objCode（字串）</p> </li> 
      </ul> </li> 
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
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>訂單指明任務或事件在敏捷積壓工作中的位置。</p> <p>此欄位已移除下列標幟：</p> 
      <ul> 
       <li> <p>動態，</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此欄位已新增下列標幟：</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>動態，</p> </li> 
       <li> <p>只讀(_O)</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>已新增此欄位，並代表使用者每天完成工作所需的小量、中量或大量工作。 可能的值包括：</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>如需Workfront中「工作成果」的詳細資訊，請參閱 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作成果概觀</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
