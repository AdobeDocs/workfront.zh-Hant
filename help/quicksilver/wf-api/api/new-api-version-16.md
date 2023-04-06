---
content-type: api
navigation-topic: api-navigation-topic
title: API 16版的新功能
description: Adobe Workfront於2022年4月6日發行API 16版。 API 16版提供第15版的下列變更。
author: Becky
feature: Workfront API
source-git-commit: 19978aaa2886008afc3c0faa9cfd18bd7c4b2555
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# API 16版的新功能

Adobe Workfront於2022年4月6日發行API 16版。 API 16版提供第15版的下列變更。

## 新增資源

未為API 16版新增資源。

## 已移除資源

未移除API 16版的資源

## 修改的資源

* <!--[AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [批准（批准）](#approval-approval)
* [客戶偏好設定(CUSTPR)](#customerpreferences-custpr)
* [ExternalSection(EXTSEC)](#externalsection-extsec)
* [小時（小時）](#hour-hour)
* [版面範本(UITMPL)](#layouttemplate-uitmpl)
* [注（注）](#note-note)
* [OpTask /問題(OPTASK)](#note-note)
* [項目(PROJ)](#project-proj)
* [比率（比率）](#rate-rate)
* [RichTextNote(RHNOTE)](#richtextnote-rhnote)
* [角色/作業角色（角色）](#role--job-role-role)
* [任務(TASK)](#task-task)
* [工時單(TSHET)](#timesheet-tshet)
* [UIFilter /篩選器(UIFT)](#uifilter--filter-uift)
* [UIGroupBy /分組(UIGB)](#uigroupby--grouping-uigb)
* [UIView /視圖(UIVW)](#uiview--view-uivw)
* [用戶（用戶）](#user-user)
* [UserNote(USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

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
            <p><b>workPerDate</b>
            </p>
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為 <code>YYYY-MM-DD: (number of minutes)</code>、和會將時區納入考量。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 分配(ASSGN)

分配對象表示工作項與被分配用於處理該工作項的用戶、團隊或組之間的連接。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為 <code>YYYY-MM-DD: (number of minutes)</code>、和會將時區納入考量。</p>
          </li>
          <li>
            <p><b>為輪廓</b>
            </p>
            <p>此欄位已新增，且是布林值，可反映指派是否具有曲面。 如果已在工作負載平衡器中編輯了分配每天的分鐘數，則分配已被定形。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum(CSTEM)

CustomEnum物件有助於將狀態代碼轉換為人類看得懂的文字。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>此動作會傳回布林值，說明客戶是否已停用自動升級貢獻者授權持有人的選項。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection(EXTSEC)

ExternalSection物件是內嵌於Workfront報表中的外部網頁。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>新增此URL，並計算內嵌於報表中之iFrame的URL。</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>新增此URL，並計算內嵌於報表中的iFrame的URL。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 小時（小時）

Hour對象表示用戶在時間表上記錄的一小時。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>已新增. 此參數用於識別使用 <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### 注（注）

Note物件是對Workfront物件所做的註解或更新。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
            </p>
            <p>此欄位已新增，並代表附加至註解的檔案清單。</p>
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
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為 <code>YYYY-MM-DD: (number of minutes)</code>、和會將時區納入考量。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>此動作已新增欄位 <code>teamIDs</code> 支援為任務或問題指派多個團隊的功能。</p>
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
            <p>已新增此欄位，並代表專案上所有預算小時數的總和。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 比率（比率）

比率物件代表Workfront中的計費比率。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>這些參數已從角色對象移到Rate對象，因此角色和用戶對象可以有多個值（對於單獨的日期範圍）。</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>這些參數表示Rate所附加的對象的ID和對象代碼。
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>此動作已新增，並將Rate物件附加至指定物件。 此端點適用於所有速率可附加對象。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote(RHNOTE)

RichTextNote物件是對Workfront物件所做的註解或更新，包含RTF文字，例如粗體或斜體文字。

RichTextNote物件已移除標幟 `REPORTABLE`.

### 角色/作業角色（角色）

角色對象（作業角色）表示用戶可能填寫的功能能力或技能集，如設計人員或產品經理。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
           <li>
            <p><b>比率</b>
            </p>
            <p>這已新增，並代表附加至此角色的比率物件。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 任務(TASK)

任務對象表示一個工作項，必須作為實現最終目標（完成項目）的步驟執行。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為 <code>YYYY-MM-DD: (number of minutes)</code>、和會將時區納入考量。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>此動作已新增欄位 <code>teamIDs</code> 支援為任務或問題指派多個團隊的功能。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### 工時單(TSHET)

工時單對象表示一個虛擬工時單卡，它允許用戶輸入實際工時，以處理任務、項目和間接費用工時類型。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>此參數已移除標幟 <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>此參數已移除標幟 <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>已新增此參數，不論「完整Workday的等同小時數」變更為何，都會以天為單位儲存時間表持續時間。  例如，如果「等同小時數」設為6，並記錄了一天，則「等同小時數」會變更為8小時， <code>totalDays</code> 仍有值1。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter /篩選器(UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>已新增此動作，並採取篩選查詢對映並新增 <code>allowingnull</code> 可空欄位的連接。</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>這些動作支援在全系統共用篩選器、檢視和分組的功能。</p><p>如需詳細資訊，請參閱 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">讓所有使用者都能使用篩選器、檢視或群組</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy /分組(UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>這些動作支援在全系統共用篩選器、檢視和分組的功能。</p><p>如需詳細資訊，請參閱 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">讓所有使用者都能使用篩選器、檢視或群組</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView /視圖(UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>新增下列可能值：</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>這些動作支援在全系統共用篩選器、檢視和分組的功能。</p><p>如需詳細資訊，請參閱 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">讓所有使用者都能使用篩選器、檢視或群組</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 用戶（用戶）

使用者物件代表擁有Workfront中可登入並與系統互動之帳戶的人員。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
           <li>
            <p><b>比率</b>
            </p>
            <p>這已新增，並代表附加至此使用者的比率物件。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote(USRNOT)

UserNote對象是通知。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">查詢</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>新增下列可能值：
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 工作（工作）

Work對象是Task和OpTask都繼承的公共介面，並且兩者之間共用公共代碼。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為 <code>YYYY-MM-DD: (number of minutes)</code>、和會將時區納入考量。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
