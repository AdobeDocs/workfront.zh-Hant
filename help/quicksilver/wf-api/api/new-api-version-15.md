---
content-type: api
navigation-topic: api-navigation-topic
title: API 15版的新增功能
description: Adobe Workfront於2022年6月14日發行API第14版。 API第15版具有第14版的下列變更。
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# API 15版的新增功能

Adobe Workfront於2022年6月14日發行API第15版。 API第15版具有第14版的下列變更。

## 新增的資源

* [方案(INITIV)](#Initiati)

* [Issdef (ISSDEF)](#IssueDef)

* [物件整合(OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [使用者核准(USRAPV)](#UserAppr)

### 方案(INITIV)

方案物件會在Workfront情境規劃工具中建立職位角色的種類和數量、固定成本和計畫福利的估計值。

如需方案的詳細資訊，請參閱 [情境規劃工具中的方案概觀](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>這是內部物件。</p>
          </li>
          <li>
            <p><b>期間</b>
            </p>
            <p>endDate和startDate之間的時間量。</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>方案的計畫完成日期。</p>
          </li>
          <li>
            <p><b>enteredById</b>
            </p>
            <p>與提交請求之使用者相關聯的ID。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>與動作相關聯的ID</p>
          </li>
          <li>
            <p><b>行動方案ID</b>
            </p>
            <p>與方案相關聯的ID。</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>上次在Workfront情境規劃工具中發佈行動方案的日期。</p>
          </li>
          <li>
            <p><b>名稱</b>
            </p>
            <p>方案的名稱</p>
          </li>
          <li>
            <p><b>planid</b>
            </p>
            <p>與方案相關聯的計畫ID。</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>與方案關聯的計畫名稱。</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>與方案相關聯的專案ID。</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>與方案關聯的Workfront情境規劃工具中的情境ID。</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>方案的計劃開始日期。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <ul>
          <li>
            <p><b>客戶</b>
            </p>
          </li>
          <li>
            <p><b>輸入者</b>
            </p>
          </li>
          <li>
            <p><b>專案</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>名稱</b>
            </p>
          </li>
          <li>
            <p><b>物件代碼</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">作業</td>
      <td>
        <ul>
          <li>
            <p><b>計數</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>報告 </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Issdef (ISSDEF)

IssueDef物件代表關於問題格式的一組資料。 此物件可附加到專案或範本，並影響新增到該專案或範本的問題。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>物件代碼</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 物件整合(OBJINT)

在某些情況下，可以直接將Workfront工作專案連結到外部軟體產品中的物件。 ObjectIntegration物件代表此連結。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>這是內部物件。</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>ObjectIntegration輸入Workfront系統的日期和時間。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>特定ObjectIntegration物件的唯一Workfront ID。</p>
          </li>
          <li>
            <p><b>integrationtype</b>
            </p>
            <p>ObjectIntegration物件用來建立連結的外部軟體。 可能的值包括：</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>物件ID</b>
            </p>
            <p>與ObjectIntegration相關聯的Workfront物件。</p>
          </li>
          <li>
            <p><b>物件代碼</b>
            </p>
            <p>與ObjectIntegration相關聯之Workfront中物件的物件程式碼。</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <ul>
          <li>
            <p><b>客戶</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>物件代碼</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

TaskDef物件代表關於工作格式的一組資料。 此物件可附加到專案或範本，並影響新增到該專案或範本的任務。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <ul>
          <li>
            <p><b>defaultProvalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>物件類別
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>物件代碼</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 使用者核准(USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位 </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>要求者ID</b>
            </p>
          </li>
          <li>
            <p><b>狀態</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <ul>
          <li>
            <p><b>核准者</b>
            </p>
          </li>
          <li>
            <p><b>客戶</b>
            </p>
          </li>
          <li>
            <p><b>要求者</b>
            </p>
          </li>
          <li>
            <p><b>使用者</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>物件代碼</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">預設欄位</td>
      <td >
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>要求者ID</b>
            </p>
          </li>
          <li>
            <p><b>狀態</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>核准</b>
            </p>
          </li>
          <li>
            <p><b>拒絕</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">作業</td>
      <td>
        <ul>
          <li>
            <p><b>新增</b>
            </p>
          </li>
          <li>
            <p><b>計數</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>報告</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## 已移除的資源

未移除API版本15的資源。

## 已修改的資源

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [存取規則(ACSRUL)](#AccessRu)

* [核准(APPROVAL)](#Approval)

* [類別(CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [客戶偏好設定(CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [群組（群組）](#Group)

* [日誌專案(JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [Op任務/問題(OPTASK)](#OpTask)

* [引數（引數）](#Paramete)

* [Portfolio（連線埠）](#Portfoli)

* [方案(PRGM)](#Program)

* [專案（專案）](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [任務（任務）](#Task)

* [範本(TMPL)](#Template)

* [時程表(TSHET)](#Timeshee)

* [檢視(UIVIEW)](#View)

* [更新（更新）](#Update)

* [使用者(USER)](#User)

* [使用者附註(USRNOT)](#UserNote)

* [工作（工作）](#Work)

### AccessLevel (ACSLVL)

AccessLevel物件與使用者相關聯，並描述決定使用者可存取內容的AccessLevelPermissions集合。

如需存取層級的詳細資訊，請參閱 [存取層級](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>VTMAWMG （檢視與我的群組相關聯的團隊）</p>
              </li>
              <li>
                <p>VALLTM （檢視所有團隊）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions (ALVPER)

AccessLevelPermissions物件代表存取、建立或修改Workfront物件的特定許可權。 然後，這些許可權可以與存取層級相關聯。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

如果使用者無權存取Workfront中他們需要的物件，他們可以請求存取該物件。 AccessRequest物件代表此要求。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>動作</b> （字串）</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> （字串）</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 存取規則(ACSRUL)

AccessRule物件代表自訂存取層級中的規則集，可決定使用者如何共用他們建立的專案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 核准(APPROVAL)

指定的工作專案，例如工作、檔案或時程表，可能需要主管或其他使用者登出該工作專案。 Approval物件代表在工作專案上簽核的動作。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <ul>
          <li>
            <p><b>方案</b>
            </p>
            <p>已新增.</p>
            <p>方案物件會在Workfront情境規劃工具中建立職位角色的種類和數量、固定成本和計畫福利的估計值。 </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>已新增.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>已新增.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">已新增.</p>
            <p>在某些情況下，可以直接將Workfront工作專案連結到外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 類別(CTGY)

類別物件是自訂表單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> （字串）</p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>群組（群組）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>物件型別</b> (string[])</p>
            <p>已新增.</p>
            <p style="font-weight: normal;">此引數是可附加自訂表單的可能物件陣列。 新增此項是為了支援將自訂表單附加到多種物件型別的功能。</p>
            <p>可能的值： </p>
            <p>CMPY，連線埠， PRGM，專案，任務， OPTASK，使用者， DOCU，費用， ITRN，帳單，群組</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>物件型別</b> (string[])</p>
            <p>已新增.</p>
            <p style="font-weight: normal;">此引數是可附加自訂表單的可能物件陣列。 新增此項是為了支援將自訂表單附加到多種物件型別的功能。</p>
            <p>可能的值： </p>
            <p>CMPY，連線埠， PRGM，專案，任務， OPTASK，使用者， DOCU，費用， ITRN，帳單，群組</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormalFromDescription</b>
            </p>
            <p>已新增.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>已新增.</p>
          </li>
          <li>
            <p><b>rawCustomExpress</b>
            </p>
            <p>已新增.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 客戶偏好設定(CUSTPR)

CustomerPreferences物件代表客戶已針對其Workfront例項設定的偏好設定集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>名稱</b>
            </p>
            <p>已新增下列值：</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint (Graph API) 整合已啟用)</p>
                <p>此值支援更新的Sharepoint整合。</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (允許使用者在不使用範本的情況下建立專案)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

檔案可整理到資料夾中。 您可以在個人的「檔案」區域中建立個人資料夾。 DocumentFolder物件代表其中一個資料夾。

DocumentFolder物件已新增標幟 `SHARABLE`.

### DocumentVersion (DOCV)

DocumentVersion物件代表檔案的特定版本（例如書面材料、影像或其他形式的資訊）。

如需檔案版本的詳細資訊，請參閱 [上傳檔案的新版本](../../documents/managing-documents/upload-new-document-version.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>已新增下列值： </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>此值支援更新的Sharepoint整合。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 群組（群組）

群組物件代表一組使用者和團隊。 群組通常代表部門結構。

如需群組的詳細資訊，請參閱群組與團隊。

群組物件已新增標幟 `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <p>已新增下列欄位：</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>類別是自訂表單。 新增此引數是為了支援新增自訂Forms至群組物件的功能。 </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>如果物件為「作用中」，則此為布林值引數；如果物件為「非作用中」，則此值為false。 設定為「作用中」的物件會出現在下拉式選單和預先輸入欄位中，並可附加到其他物件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <p>已新增下列欄位：</p>
        <ul>
          <li>
            <p><b>核准者</b>
            </p>
          </li>
          <li>
            <p><b>客戶</b>
            </p>
          </li>
          <li>
            <p><b>要求者</b>
            </p>
          </li>
          <li>
            <p><b>使用者</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <p>已新增下列欄位：</p>
        <ul>
          <li>
            <p><b>物件類別</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情況下，可以直接將Workfront工作專案連結到外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">預設欄位</td>
      <td >
        <p>已新增下列欄位：</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>如果物件為「作用中」，則此為布林值引數；如果物件為「非作用中」，則此值為false。 設定為「作用中」的物件會出現在下拉式選單和預先輸入欄位中，並可附加到其他物件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <p>已新增下列欄位：</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>此動作會重新計算自訂表單欄位中的運算式。</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 日誌專案(JRNLE)

JournalEntry物件可設定為每次修改特定物件欄位時，記錄這些欄位的相關資訊。 當欄位設定為記錄為日誌專案物件的一部分時，每次修改該欄位時都會建立對應的日誌專案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>已新增下列值： </p>
        <ul>
          <li>
            <p>DW （下載）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

LinkedFolder物件代表連結自外部檔案提供者(例如Google Drive或Dropbox)的資料夾。

如需連結資料夾的詳細資訊，請參閱從外部應用程式連結檔案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>已新增下列值： </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>此值支援更新的Sharepoint整合。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Op任務/問題(OPTASK)

OpTask物件通常稱為「問題」。 問題指工作專案，通常表示發生問題而無法完成任務或專案。 問題也可以是服務檯請求。 變更單、請求和錯誤也是問題。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <p>已新增下列動作：</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>已修改下列動作：</p>
        <ul>
          <li>
            <p><b>copyissue</b>
            </p>
            <p>已新增欄位 <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 引數（引數）

Parameter物件是自訂欄位。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <p>已新增下列欄位：</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>下列欄位已修改：</p>
        <ul>
          <li>
            <p><b>資料型別</b>
            </p>
            <p>已新增可能的值 <code>WIDGET </code>(Widget) </p>
            <p>此值支援在自訂表單中使用影像。</p>
          </li>
          <li>
            <p><b>顯示型別</b>
            </p>
            <p>已新增可能的值 <code>WIDGET </code>(Widget)</p>
            <p>此值支援在自訂表單中使用影像。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio（連線埠）

Portfolio物件是競爭相同資源（通常是金錢或人力）的專案集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 方案(PRGM)

計畫物件是投資組合中專案的子集，其中類似的專案可以分組在一起。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 專案（專案）

專案是Workfront內的工作專案，也是Workfront協助人們完成工作的主要建置組塊。 Project物件代表具有共同特定目標的一組任務。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <ul>
          <li>
            <p><b>方案</b>
            </p>
            <p>方案物件會在Workfront情境規劃工具中建立職位角色的種類和數量、固定成本和計畫福利的估計值。 </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情況下，可以直接將Workfront工作專案連結到外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

QueueDef物件代表佇列，這是已發佈至服務檯區域的專案，可讓使用者向其提交問題。

如需請求佇列的詳細資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (編輯我管理的群組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，而他們的答案可讓經理瞭解專案與產品組合目標的對齊程度。

如需計分卡問題的詳細資訊，請參閱 [建立計分卡](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>顯示型別</b>
            </p>
            <p>已新增可能的值 <code>WIDGET </code>(Widget)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 任務（任務）

Task物件代表作為達成最終目標（完成專案）的步驟而必須執行的工作專案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情況下，可以直接將Workfront工作專案連結到外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 範本(TMPL)

Template物件代表專案的模式。 可以從範本建立專案以節省時間。 範本包含專案團隊和任務，這些專案將會複製到從範本建立的任何專案中。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 時程表(TSHET)

時程表物件代表虛擬時程表，可讓使用者輸入任務、專案和管理費用時數型別的實際工作時數。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <p>下列欄位已移除：</p>
        <ul>
          <li>
            <p><b>物件代碼</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 檢視(UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>下列可能的值已移除：</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (四欄式配置)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (更新)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (更新)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (處理中)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (自訂資料)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (更新自訂資料)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (狀態更新)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (狀態更新)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (狀態更新)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (狀態更新)</p>
              </li>
              <li>
                <p><code>DLIST</code> (詳細資訊清單)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (詳細資訊清單部分)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 更新（更新）

Workfront中的工作專案可以更新，以隨時通知使用者目前的狀態。 Update物件代表其中一項更新。 更新可由使用者輸入，或由Workfront系統建立。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>已新增可能的值 <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 使用者(USER)

使用者物件代表擁有Workfront帳戶的人員，該帳戶可以登入並與系統互動。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 使用者附註(USRNOT)

UserNote物件是通知。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>eventtype</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>DUP </code>（要求您校稿檔案）</p>
              </li>
              <li>
                <p><code>DUV </code>（可讓您檢視檔案）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 工作（工作）

Work物件是Task和OpTask都繼承的公用介面，並在兩者之間共用公用程式碼。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情況下，可以直接將Workfront工作專案連結到外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
