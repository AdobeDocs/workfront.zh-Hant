---
content-type: api
navigation-topic: api-navigation-topic
title: API 15版的新功能
description: Adobe Workfront於2022年6月14日發行API 14版。 API 15版提供第14版的下列變更。
author: John
feature: Workfront API
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# API 15版的新功能

Adobe Workfront已於2022年6月14日發行API 15版。 API 15版提供第14版的下列變更。

## 新增資源

* [計畫(INITIV)](#Initiati)

* [IssueDef(ISSDEF)](#IssueDef)

* [ObjectIntegration(OBJINT)](#ObjectIn)

* [RtfTextGroupParameterValue(GRCVAL)](#RichText)

* [TaskDef(TSKDEF)](#TaskDef)

* [UserApproval(USRAPV)](#UserAppr)

### 計畫(INITIV)

方案對象在Workfront方案計畫員中建立任務職責的種類和數量、固定成本和計畫福利的估計。

有關計畫的詳細資訊，請參閱 [方案計畫器中的方案概覽](../../scenario-planner/initiatives-overview.md).

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
            <p>endDate和startDate之間的時間。</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>計畫的完成日期。</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>與提交請求的使用者相關聯的ID。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>與動作相關聯的ID</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>與計畫相關聯的ID。</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>在Workfront方案規劃器中上次發佈方案的日期。</p>
          </li>
          <li>
            <p><b>名稱</b>
            </p>
            <p>計畫的名稱</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>與計畫關聯的計畫ID。</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>與計畫關聯的計畫的名稱。</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>與方案關聯的項目ID。</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>與方案關聯的Workfront方案計畫器中方案的ID。</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>計畫起始日期。</p>
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
            <p><b>enteredBy</b>
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
            <p><b>objCode</b>
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
            <p><b>報表 </b>
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

### IssueDef(ISSDEF)

IssueDef對象表示一組與問題格式有關的資料。 此對象可附加到項目或模板，並影響添加到該項目或模板的問題。

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
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration(OBJINT)

在某些情況下，可將Workfront工作項目直接連結至外部軟體產品中的物件。 ObjectIntegration物件代表此連結。

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
            <p>在Workfront系統中輸入ObjectIntegration的日期和時間。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>特定ObjectIntegration物件的唯一Workfront ID。</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>ObjectIntegration對象建立連結的外部軟體。 可能的值包括：</p>
            <ul>
              <li>
                <p>吉拉</p>
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
            <p><b>objID</b>
            </p>
            <p>Workfront中與ObjectIntegration相關聯的物件。</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>ObjectIntegration所關聯之Workfront中物件的物件程式碼。</p>
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
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef(TSKDEF)

TaskDef對象表示一組與任務格式有關的資料。 此對象可附加到「項目」或「模板」，並影響添加到該「項目」或「模板」的任務。

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
            <p><b>defaultApprovalProcess </b>
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
            <p><b>objectCategories
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
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval(USRAPV)

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
            <p><b>requestorID</b>
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
            <p><b>請求者</b>
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
            <p><b>objCode</b>
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
            <p><b>requestorID</b>
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
            <p><b>報表</b>
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

## 已移除資源

未移除API 15版的資源。

## 修改的資源

* [AccessLevel(ACSLVL)](#AccessLe)

* [AccessLevelPermissions(ALVPER)](#AccessLe2)

* [AccessRequest(ACSREQ)](#AccessRe)

* [AccessRule(ACSRUL)](#AccessRu)

* [批准（批准）](#Approval)

* [類別(CTGY)](#Category)

* [CategoryParameter(CTGYPA)](#Category2)

* [客戶偏好設定(CUSTPR)](#Customer)

* [DocumentFolder(DOCFDR)](#Document)

* [DocumentVersion(DOCV)](#Document2)

* [組（組）](#Group)

* [日誌條目(JRNLE)](#JournalE)

* [LinkedFolder(LNKFDR)](#LinkedFo)

* [OpTask /問題(OPTASK)](#OpTask)

* [參數(PARAM)](#Paramete)

* [Portfolio（埠）](#Portfoli)

* [方案](#Program)

* [項目(PROJ)](#Project)

* [QueueDef(QUED)](#QueueDef)

* [ScoreCardQuestion(SCOREQ)](#ScoreCar)

* [任務(TASK)](#Task)

* [範本(TMPL)](#Template)

* [工時單(TSHET)](#Timeshee)

* [視圖(UIVIEW)](#View)

* [更新（更新）](#Update)

* [用戶（用戶）](#User)

* [UserNote(USRNOT)](#UserNote)

* [工作（工作）](#Work)

### AccessLevel(ACSLVL)

AccessLevel對象與用戶關聯，並描述了決定用戶可以訪問的AccessLevelPermissions集。

有關訪問級別的詳細資訊，請參見 [存取層級](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

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
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>VTMAWMG（查看與我的組關聯的團隊）</p>
              </li>
              <li>
                <p>VALLTM（查看所有團隊）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions(ALVPER)

AccessLevelPermissions對象表示訪問、建立或修改Workfront對象的特定權限。 然後，這些權限便可與存取層級相關聯。

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
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest(ACSREQ)

如果使用者沒有必要存取Workfront中物件的權限，可以要求存取該物件。 AccessRequest物件代表此請求。

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
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> （字串）</p>
            <p>新增下列可能值：</p>
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

### AccessRule(ACSRUL)

AccessRule對象表示自定義訪問級別中的規則集，該規則確定用戶如何共用他們建立的項目。

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
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 批准（批准）

給定的工作項（如任務、文檔或時間表）可能要求主管或其他用戶簽出該工作項。 Approval對象表示簽出工作項的操作。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerDekededHours </b>
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
            <p><b>倡議</b>
            </p>
            <p>已新增.</p>
            <p>方案對象在Workfront方案計畫員中建立任務職責的種類和數量、固定成本和計畫福利的估計。 </p>
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
            <p>在某些情況下，可將Workfront工作項目直接連結至外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
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
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>組（組）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>已新增.</p>
            <p style="font-weight: normal;">此參數是可附加自訂表單的可能對象陣列。 已新增此功能，以支援將自訂表單附加至多種物件類型的功能。</p>
            <p>可能的值： </p>
            <p>CMPY，埠， PRGM, PROJ，任務， OPTASK，用戶， DOCU, EXPNS, ITRN，清單，組</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>已新增.</p>
            <p style="font-weight: normal;">此參數是可附加自訂表單的可能對象陣列。 已新增此功能，以支援將自訂表單附加至多種物件類型的功能。</p>
            <p>可能的值： </p>
            <p>CMPY，埠， PRGM, PROJ，任務， OPTASK，用戶， DOCU, EXPNS, ITRN，清單，組</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter(CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>已新增.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>已新增.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>已新增.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 客戶偏好設定(CUSTPR)

CustomerPreferences物件代表客戶為其Workfront例項所設定的偏好設定集。

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
            <p>新增下列值：</p>
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

### DocumentFolder(DOCFDR)

文檔可以組織成資料夾。 您可以在個人文檔區域中建立個人資料夾。 DocumentFolder對象表示其中一個資料夾。

已添加標籤的DocumentFolder對象 `SHARABLE`.

### DocumentVersion(DOCV)

DocumentVersion對象表示檔案的特定版本（如書面材料、影像或其他形式的資訊）。

有關文檔版本的詳細資訊，請參閱 [上傳新版本的檔案](../../documents/managing-documents/upload-new-document-version.md).

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
            <p>新增下列值： </p>
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

### 組（組）

群組物件代表一組使用者和團隊。 團體往往代表部門結構。

如需群組的詳細資訊，請參閱群組與團隊的比較。

群組物件已新增標幟 `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <p>新增下列欄位：</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>類別是自訂表單。 已新增此參數，以支援將自訂Forms新增至群組物件的功能。 </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>如果物件為「作用中」，則此為布林值參數，如果物件為「false」，則值為true。 設定為「活動」(Active)的對象會顯示在下拉菜單和「預先輸入」(Type-ahead)欄位中，並可附加到其他對象。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td >
        <p>新增下列欄位：</p>
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
            <p><b>請求者</b>
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
        <p>新增下列欄位：</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情況下，可將Workfront工作項目直接連結至外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
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
            <p>如果物件為「作用中」，則此為布林值參數，如果物件為「false」，則值為true。 設定為「活動」的對象會顯示在下拉菜單和「預先輸入」欄位中，並可附加到其他對象。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <p>新增下列欄位：</p>
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

### 日誌條目(JRNLE)

JournalEntry對象可以設定為在修改這些欄位時記錄有關特定對象欄位的資訊。 將欄位設定為作為日記帳分錄對象的一部分進行記錄時，每次修改該欄位時都將建立相應的日記帳分錄。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>新增下列值： </p>
        <ul>
          <li>
            <p>DW（下載）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder(LNKFDR)

LinkedFolder對象表示從外部文檔提供程式(如Google驅動器或Dropbox)連結的資料夾。

有關連結資料夾的詳細資訊，請參閱從外部應用程式連結文檔。

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
            <p>新增下列值： </p>
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

### OpTask /問題(OPTASK)

OpTask物件通常稱為「問題」。 問題是工作項，通常表示存在問題，無法完成任務或項目。 問題也可以是服務台請求。 變更訂單、請求和錯誤也是問題。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <p>新增下列動作：</p>
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
            <p><b>copyIssue</b>
            </p>
            <p>新增欄位 <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 參數(PARAM)

參數物件是自訂欄位。

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
        <p>已修改下列欄位：</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>新增可能的值 <code>WIDGET </code>（介面工具集） </p>
            <p>此值支援在自訂表單中使用影像。</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>新增可能的值 <code>WIDGET </code>（介面工具集）</p>
            <p>此值支援在自訂表單中使用影像。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio（埠）

Portfolio物件是專案的集合，這些專案會爭奪相同的資源，通常是金錢或人員來完成。

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

### 方案

方案物件是產品組合內的專案子集，可將類似專案分組。

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

### 項目(PROJ)

專案是Workfront內的工作項目，是Workfront協助人們工作的主要建置要素。 專案物件代表一組具有共同特定目標的工作。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerDekededHours</b>
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
            <p><b>倡議</b>
            </p>
            <p>方案對象在Workfront方案計畫員中建立任務職責的種類和數量、固定成本和計畫福利的估計。 </p>
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
            <p>在某些情況下，可將Workfront工作項目直接連結至外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef(QUED)

QueueDef對象表示「隊列」，該項目已發佈到「幫助台」區域，允許用戶向其提交問題。

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
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（編輯我所在的團隊）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(編輯我管理的組中的團隊（僅限群組管理員）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion(SCOREQ)

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，他們的答案使經理能夠了解項目與產品組合目標的一致程度。

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
            <p><b>displayType</b>
            </p>
            <p>新增可能的值 <code>WIDGET </code>（介面工具集）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 任務(TASK)

任務對象表示一個工作項，必須作為實現最終目標（完成項目）的步驟執行。

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
            <p>在某些情況下，可將Workfront工作項目直接連結至外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 範本(TMPL)

範本物件代表專案的模式。 可從範本建立專案，以節省時間。 範本包含團隊和任務，這些團隊和任務將複製到從範本建立的任何專案。

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

### 工時單(TSHET)

工時單對象表示一個虛擬工時單卡，它允許用戶輸入實際工時，以處理任務、項目和間接費用工時類型。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <p>已移除下列欄位：</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 視圖(UIVIEW)

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
            <p>已移除下列可能值：</p>
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

Workfront中的工作項目可以更新，讓使用者隨時了解目前狀態。 更新對象表示其中一個更新。 使用者可輸入更新，或由Workfront系統建立。

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
            <p>新增可能的值 <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 用戶（用戶）

使用者物件代表擁有Workfront中可登入並與系統互動之帳戶的人員。

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

### UserNote(USRNOT)

UserNote對象是通知。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>eventType</b>
            </p>
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p><code>DUP </code>（請您校樣檔案）</p>
              </li>
              <li>
                <p><code>DUV </code>（允許查看文檔）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 工作（工作）

Work對象是Task和OpTask都繼承的公共介面，並且兩者之間共用公共代碼。

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
            <p>在某些情況下，可將Workfront工作項目直接連結至外部軟體產品中的物件。 ObjectIntegration物件代表此連結。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
