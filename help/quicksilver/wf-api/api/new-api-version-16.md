---
content-type: api
navigation-topic: api-navigation-topic
title: API 16版的新增功能
description: Adobe Workfront於2022年4月6日發行API第16版。 API第16版具有第15版的下列變更。
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# API 16版的新增功能

Adobe Workfront於2023年4月6日發行API第16版。 API第16版具有第15版的下列變更。

## 新增的資源

未針對API版本16新增資源。

## 已移除的資源

未移除API版本16的資源

## 已修改的資源

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [核准(APPROVAL)](#approval-approval)
* [客戶偏好設定(CUSTPR)](#customerpreferences-custpr)
* [外部截面(EXTSEC)](#externalsection-extsec)
* [Hour (HOUR)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [附註（附註）](#note-note)
* [Op任務/問題(OPTASK)](#note-note)
* [專案（專案）](#project-proj)
* [費率（費率）](#rate-rate)
* [RTF備註(RHNOTE)](#richtextnote-rhnote)
* [角色/工作角色(ROLE)](#role--job-role-role)
* [任務（任務）](#task-task)
* [時程表(TSHET)](#timesheet-tshet)
* [UIFilter /篩選器(UIFT)](#uifilter--filter-uift)
* [UIGroupBy /群組(UIGB)](#uigroupby--grouping-uigb)
* [檢視/檢視(UIVW)](#uiview--view-uivw)
* [使用者(USER)](#user-user)
* [使用者附註(USRNOT)](#usernote-usrnot)

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
            <p><b>workPerDate</b>
            </p>
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為<code>YYYY-MM-DD: (number of minutes)</code>，並考慮到時區。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 指定任務(ASSGN)

工作指派物件代表工作專案與指派處理該工作專案的使用者、專案團隊或群組之間的連線。

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
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為<code>YYYY-MM-DD: (number of minutes)</code>，並考慮到時區。</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>此欄位已新增，其為布林值，可反映指派是否已設定輪廓。 如果指派的每日分鐘數已在工作負載平衡器中編輯，則指派已設定為輪廓。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### 自訂列舉(CSTEM)

CustomEnum物件可協助將狀態代碼轉換為人類看得懂的文字。

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
            <p>已新增下列可能值：</p>
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
            <p>此動作會傳回布林值，說明客戶是否已停用自動升級貢獻者授權持有者的選項。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 外部截面(EXTSEC)

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
            <p>新增此引數，並計算報表中內嵌之iFrame的URL。</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>新增此功能，並計算報表中內嵌iFrame的URL。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Hour (HOUR)

Hour物件代表使用者在時程表上記錄的一小時。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>時程表小時識別碼</b>
            </p>
            <p>已新增。 此引數用於識別使用<code>batchSave</code>建立的小時。 </p>
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

### 附註（附註）

Note物件是在Workfront物件上所做的註解或更新。

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
            <p>此欄位已新增，並代表附加至評論的檔案清單。</p>
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
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為<code>YYYY-MM-DD: (number of minutes)</code>，並考慮到時區。</p>
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
            <p>此動作新增欄位<code>teamIDs</code>以支援將多個團隊指派至一個任務或問題的功能。</p>
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
            <p>此欄位已新增，並代表專案上所有預算時數的總和。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 費率（費率）

Rate物件代表Workfront中的計費費率。

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
           <p>這些引數已從Role物件移至Rate物件，因此Role和User物件可以有多個值（適用於個別的日期範圍）。</p>
          </li>
          <li><p><b>物件ID</b></p><p><b>物件代碼</b></p>
          <p>這些引數代表Rate所附加物件的ID與物件程式碼。
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
           <p>此動作已新增，並將Rate物件附加到指定的Object。 此端點適用於所有速率可附加物件。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RTF備註(RHNOTE)

RtfNote物件是在Workfront物件上所做的註解或更新，其中包括RTF文字，例如粗體或斜體文字。

RichTextNote物件已移除旗標`REPORTABLE`。

### 角色/工作角色(ROLE)

角色物件（工作角色）代表使用者可能填入的功能容量或技能集，例如Designer或產品經理。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
           <li>
            <p><b>費率</b>
            </p>
            <p>此專案已新增，並代表附加至此角色的Rate物件。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 任務（任務）

Task物件代表作為達成最終目標（完成專案）的步驟而必須執行的工作專案。

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
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為<code>YYYY-MM-DD: (number of minutes)</code>，並考慮到時區。</p>
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
            <p>此動作新增欄位<code>teamIDs</code>以支援將多個團隊指派至一個任務或問題的功能。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### 時程表(TSHET)

時程表物件代表虛擬時程表，可讓使用者輸入任務、專案和管理費用時數型別的實際工作時數。

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
            <p>此引數已移除旗標<code>READ_ONLY</code>。</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>此引數已移除旗標<code>READ_ONLY</code>。</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>已新增此引數，且無論「完整Workday的相等時數」有何變更，都以天為單位儲存時程表持續時間。  例如，如果「對等時數」設為6，並記錄一天，則「對等時數」會變更為8小時，<code>totalDays</code>的值仍為1。</p>
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
            <p>此動作已新增，而且採用篩選器查詢對應，並為可空欄位新增<code>allowingnull</code>聯結。</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>這些動作支援在整個系統內共用篩選器、檢視和群組的功能。</p><p>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">讓所有使用者都可以使用篩選器、檢視或群組</a>。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy /群組(UIGB)


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
            <p>這些動作支援在整個系統內共用篩選器、檢視和群組的功能。</p><p>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">讓所有使用者都可以使用篩選器、檢視或群組</a>。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### 檢視/檢視(UIVW)

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
            <p>已新增下列可能值：</p>
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
            <p>這些動作支援在整個系統內共用篩選器、檢視和群組的功能。</p><p>如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">讓所有使用者都可以使用篩選器、檢視或群組</a>。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 使用者(USER)

使用者物件代表擁有Workfront帳戶的人員，該帳戶可以登入並與系統互動。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
           <li>
            <p><b>費率</b>
            </p>
            <p>此專案已新增，並代表附加至此使用者的Rate物件。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 使用者附註(USRNOT)

UserNote物件是通知。

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
            <p>已新增下列可能值：
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

Work物件是Task和OpTask都繼承的公用介面，並在兩者之間共用公用程式碼。

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
            <p>此欄位已新增，並顯示您每天需要執行的工作分鐘數。 其格式為<code>YYYY-MM-DD: (number of minutes)</code>，並考慮到時區。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
