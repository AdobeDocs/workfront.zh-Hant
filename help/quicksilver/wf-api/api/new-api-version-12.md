---
content-type: api
navigation-topic: api-navigation-topic
title: API 12版的新增功能
description: Workfront於2020年11月12日發行API第12版。 API第12版具有第11版的下列變更
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '2422'
ht-degree: 1%

---

# API 12版的新增功能

Workfront於2020年11月12日發行API第12版。 API第12版具有第11版的下列變更

## 新增的資源

下列是Workfront API 12版的新資源。

* [BreadCrumb](#breadcrumb)
* [RtfParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

BreadCrumb物件代表Adobe Workfront工作專案之父/子階層中的元素。 階層連結可指出工作專案如何融入Portfolio、專案、專案和任務的較大結構。

如需Workfront階層連結的詳細資訊，請參閱新Adobe Workfront體驗中的[階層連結概觀](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

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

### RtfParameterValue {#richtextparametervalue}

RTF文字欄位現在可用於更多物件。 已將RichTextParameterValue物件新增至Workfront，以支援此可用性。

如需詳細資訊，請參閱Adobe Workfront API中的[&#x200B; RTF欄位](../../wf-api/general/rich-text-field-api.md)。

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
     <li style="font-weight: bold;">物件代碼</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 已移除的資源

未移除API版本12的資源。

## 已修改的資源

已針對Workfront API 12版修改下列資源。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">存取層級</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">存取規則</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">活動記錄檔</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnouncementAttachment</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">核准</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">行事曆區段</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">公司</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">客戶</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">客戶喜好設定</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">檔案</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">群組</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">引數</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">程式</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">排程報告</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">任務</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">團隊</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">範本任務</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">時程表</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">使用者</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">工作</a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### 存取層級 {#accesslevel}

AccessLevel物件與使用者相關聯，並描述決定使用者可存取內容的AccessLevelPermissions集合。

如需存取層級的詳細資訊，請參閱[存取層級的運作方式](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)。

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

AccessLevelPermissions物件代表存取、建立或修改Workfront物件的特定許可權。 然後，這些許可權可以與存取層級相關聯。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包含此許可權的存取層級的使用者可以在工作負載平衡器中更新規劃時數。</p> <p>如需詳細資訊，請參閱<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器</a>中管理使用者指派時<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任務計畫時數</a>。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此許可權的存取層級的使用者可以將欄位新增到自訂表單。</p> <p>如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">建立或編輯自訂表格</a>。</p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> <p>具有包含此許可權的存取層級的使用者可以在系統範圍內以刪除存取權共用自訂欄位。</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> </li> 
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

如果使用者無權存取Workfront中他們需要的物件，他們可以請求存取該物件。 AccessRequest物件代表此要求。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">動作</p> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包含此許可權的存取層級的使用者可以在工作負載平衡器中更新規劃時數。</p> <p>如需詳細資訊，請參閱<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器</a>中管理使用者指派時<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任務計畫時數</a>。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此許可權的存取層級的使用者可以將欄位新增到自訂表單。</p> <p>如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">建立或編輯自訂表格</a>。</p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> <p>具有包含此許可權的存取層級的使用者可以在系統範圍內以刪除存取權共用自訂欄位。</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包含此許可權的存取層級的使用者可以在工作負載平衡器中更新規劃時數。</p> <p>如需詳細資訊，請參閱<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器</a>中管理使用者指派時<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任務計畫時數</a>。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此許可權的存取層級的使用者可以將欄位新增到自訂表單。</p> <p>如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">建立或編輯自訂表格</a>。</p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> <p>具有包含此許可權的存取層級的使用者可以在系統範圍內以刪除存取權共用自訂欄位。</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 活動記錄 {#activitylog}

ActivityLog物件是在指定Workfront Proof帳戶中發生的所有活動的完整清單。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>營運</p> </td> 
   <td> <p>下列作業已從ActivityLog物件中移除：</p> 
    <ul> 
     <li> <p><strong>新增</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 宣告附件 {#announcementattachment}

AnnouncementAttachment物件代表已附加至Workfront宣告的檔案。

如需宣告附件的詳細資訊，請參閱[傳送宣告](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>副檔名</strong> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>已移除下列標幟：</p> 
      <ul> 
       <li> <p>動態，</p> </li> 
       <li> <p>延遲讀取，</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>已新增下列旗標</p> 
      <ul> 
       <li> <p>AUTO_LOAD，</p> </li> 
       <li> <p>動態，</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>工作量</strong> </p> <p>此欄位已新增，並代表使用者需要少量、中量或大量每日努力才能完成任務。 可能的值包括：</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>如需有關Workfront中工作量的詳細資訊，請參閱<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作量概觀</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 行事曆區段 {#calendarsection}

行事曆區段是行事曆報告。

如需行事曆報告的詳細資訊，請參閱[行事曆報告總覽](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> <p style="font-weight: normal;">CalendarSection物件新增了下列欄位，以支援在行事曆報表中使用自訂日期的新功能。 </p> <p style="font-weight: normal;">如需詳細資訊，請參閱<a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">在行事曆報告中使用自訂日期欄位</a>。</p> 
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

Company物件代表由人員集合組成的組織。

如需有關公司的詳細資訊，請參閱[建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">與公司相關聯的群組ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">與公司相關聯的群組。 將公司與群組建立關聯可讓群組管理員擴充對公司的群組存取權和許可權。</p> </li> 
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
  <tr> 
   <td>動作</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>產品已啟用</strong> </p> <p style="font-weight: normal;">此動作會採用CustomerProductTypeEnum引數並傳回布林值，指出該客戶是否有該產品的帳戶。 </p> </li> 
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
       <li style="font-weight: normal;">password：zoomIntegrationEnabled （啟用更新資料流中的縮放整合）</li> 
       <li style="font-weight: normal;"> 密碼：quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">已新增</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 檔案版本 {#documentversion}

DocumentVersion物件代表檔案的特定版本（例如書面材料、影像或其他形式的資訊）。

如需檔案版本的詳細資訊，請參閱[上傳檔案的新版本](../../documents/managing-documents/upload-new-document-version.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">已移除可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>校訂決定</strong> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> <p>下列動作已新增至Document物件。</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">此動作採用documentVersonID引數（字串）並傳回指出檢閱者決定的地圖。</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">此動作會採用下列引數：</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID （字串）</p> </li> 
       <li> <p>reviewerDecision （字串）</p> </li> 
       <li> <p>註解（字串）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 群組  {#group}

群組物件代表一組使用者和團隊。 群組通常代表部門結構。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>業務領導者ID</p> <p style="font-weight: normal;">指派給群組的業務領導者ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>業務領導者</p> <p style="font-weight: normal;">指派給群組的業務領導者。 業務主管是負責為群組制定業務決策的人。</p> <p style="font-weight: normal;">如需商務領導者的詳細資訊，請參閱<a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">商務領導概述</a>。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>動作</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>此動作會採用下列引數：</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID （字串）</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>此動作會採用下列引數：</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder物件代表連結自外部檔案提供者(例如Google Drive或Dropbox)的資料夾。

如需連結資料夾的詳細資訊，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">已移除可能的值：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Op 任務 {#optask}

OpTask物件通常稱為「問題」。 問題指工作專案，通常表示發生問題而無法完成任務或專案。 問題也可以是服務檯請求。 變更單、請求和錯誤也是問題。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>直接欄位</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>「順序」表示任務或劇本在敏捷待辦專案上的位置。</p> <p>此欄位已移除下列標幟：
       <ul>
        <li>動態，</li>
        <li>延遲讀取，</li>
        <li>NOT_GROUPABLE：</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>這些動作新增引數狀態以支援新的「開始」按鈕功能，當使用者按一下按鈕以指示他們已開始處理專案時，該功能會變更工作專案的狀態。</p> <p>如需詳細資訊，請參閱<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">以開始按鈕取代處理它按鈕</a>。</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 參數 {#parameter}

Parameter物件是自訂欄位。

Parameter資源已新增可共用的標幟。

如需自訂欄位的詳細資訊，請參閱[建立或編輯自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)中的[建立或編輯自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>資料型別</strong> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>RTF (RTF)</p> <p>如需詳細資訊，請參閱Adobe Workfront API中的<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref"> RTF欄位</a>。</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>新增可能的值：</p> 
      <ul> 
       <li> <p>RTF （含格式的文字欄位）</p> <p>如需詳細資訊，請參閱Adobe Workfront API中的<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref"> RTF欄位</a>。</p> </li> 
      </ul> </li> 
     <li> <p><strong>標籤</strong> </p> <p>已新增</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">集合欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>存取規則</strong> </p> <p>已新增</p> </li> 
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

Portfolio物件是競爭相同資源（通常是金錢或人力）的專案集合。

如需投資組合的詳細資訊，請參閱[Adobe Workfront中的Portfolio概觀](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">與投資組合相關聯的群組ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">與投資組合相關聯的群組。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 方案 {#program}

計畫物件是投資組合中專案的子集，其中類似的專案可以分組在一起。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">與方案相關聯的群組ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>參考欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>群組</p> <p style="font-weight: normal;">與方案相關聯的群組。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef物件代表佇列，這是已發佈至服務檯區域的專案，可讓使用者向其提交問題。

如需請求佇列的詳細資訊，請參閱[建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li><strong>requestorCoreAction</strong> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>具有包含此許可權的存取層級的使用者可以在工作負載平衡器中更新規劃時數。</p> <p>如需詳細資訊，請參閱<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器</a>中管理使用者指派時<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">更新任務計畫時數</a>。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>具有包含此許可權的存取層級的使用者可以將欄位新增到自訂表單。</p> <p>如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">建立或編輯自訂表格</a>。</p> </li> 
       <li> <p>EDIT_SYSTEM範圍 </p> <p>具有包含此許可權的存取層級的使用者可以在系統範圍內以刪除存取權共用自訂欄位。</p> </li>
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEM範圍 </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 排程報告 {#scheduledreport}

ScheduledReport物件代表已設定為排程傳送的報表。

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
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScorecardQuestion {#scorecardquestion}

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，而他們的答案可讓經理瞭解專案與產品組合目標的對齊程度。

如需計分卡問題的詳細資訊，請參閱[建立計分卡](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>顯示型別</p> <p style="font-weight: normal;">新增可能的值RTF （文字欄位含格式） </p> <p style="font-weight: normal;">如需詳細資訊，請參閱Adobe Workfront API中的<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref"> RTF欄位</a>。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 任務 {#task}

Task物件代表作為達成最終目標（完成專案）的步驟而必須執行的工作專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>工作量</strong> </p> <p>此欄位已新增，並代表使用者需要少量、中量或大量每日努力才能完成任務。 可能的值包括：</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>如需有關Workfront中工作量的詳細資訊，請參閱<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作量概觀</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>這些動作新增引數狀態以支援新的「開始」按鈕功能，當使用者按一下按鈕以指示他們已開始處理專案時，該功能會變更工作專案的狀態。</p> <p>如需詳細資訊，請參閱<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">以開始按鈕取代處理它按鈕</a>。</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 團隊 {#team}

Team物件是可指派至工作專案的「使用者」集合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> <p>下列欄位已新增至小組資源：</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>此欄位代表已完成卡片保留在Kanban面板上的天數。</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此欄位會將團隊與群組建立關聯。 這會將團隊識別為群組的一部分，並允許群組管理員管理團隊。</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>這是一個布林值引數，可指出團隊的「處理它」按鈕是否已設定為「開始」按鈕。 當專案團隊成員按一下「開始」按鈕開始處理工作專案時，專案的狀態會從「新增」變更為專案團隊設定中設定的狀態。</p> </li> 
     <li> <p>下列欄位可讓您為個別工作專案上的「開始」按鈕指定自訂狀態。</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>有關[開始]按鈕的詳細資訊，請參閱<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">以[開始]按鈕取代[處理它]按鈕</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">參考欄位</td> 
   <td> <p>下列欄位已新增至「專案團隊」資源：</p> 
    <ul> 
     <li> <p><strong>群組</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 範本任務 {#templatetask}

TemplateTask物件代表屬於Template一部分的Task。 範本任務會成為使用範本之專案中的任務。

如需範本工作的詳細資訊，請參閱[編輯範本工作](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>工作量</strong> </p> <p>此欄位已新增，並代表使用者需要少量、中量或大量每日努力才能完成任務。 可能的值包括：</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>如需有關Workfront中工作量的詳細資訊，請參閱<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作量概觀</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 時程表 {#timesheet}

時程表物件代表虛擬時程表，可讓使用者輸入任務、專案和管理費用時數型別的實際工作時數。

如需時程表的詳細資訊，請參閱[時程表總覽](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">核心欄位</td> 
   <td> <p>下列欄位已從時程表資源中移除：</p> 
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
     <li> <p><strong>updateType</strong> </p> <p>已新增下列可能值：</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">如需方案的詳細資訊，請參閱情境規劃工具</a>中的<a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">方案概觀。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 使用者 {#user}

使用者物件代表擁有Workfront帳戶的人員，該帳戶可以登入並與系統互動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接欄位</td> 
   <td> <p>下列欄位已新增至使用者資源：</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>這代表停用使用者的日期和時間。</p> <p>如需已停用使用者的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>。</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>此欄位會顯示使用者對Workfront目標的存取權。 可能的值包括：</p> 
      <ul> 
       <li> <p>無存取權</p> </li> 
       <li> <p>檢視</p> </li> 
       <li> <p>編輯</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> <p>下列動作已新增至使用者資源：</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>此動作會採用下列引數</p> 
      <ul> 
       <li> <p>ids （字串）</p> </li> 
       <li> <p>物件代碼（字串）</p> </li> 
      </ul> </li> 
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
   <td>直接欄位</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>「順序」表示任務或劇本在敏捷待辦專案上的位置。</p> <p>此欄位已移除下列標幟：</p> 
      <ul> 
       <li> <p>動態，</p> </li> 
       <li> <p>延遲讀取，</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>此欄位新增了下列旗標：</p> 
      <ul> 
       <li> <p>AUTO_LOAD，</p> </li> 
       <li> <p>動態，</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>工作量</strong> </p> <p>此欄位已新增，並代表使用者需要少量、中量或大量每日努力才能完成任務。 可能的值包括：</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>如需有關Workfront中工作量的詳細資訊，請參閱<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作量概觀</a>。</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
