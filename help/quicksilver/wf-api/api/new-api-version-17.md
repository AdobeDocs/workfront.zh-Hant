---
content-type: api
navigation-topic: api-navigation-topic
title: API 17版的新增功能
description: Adobe Workfront於2022年4月6日發行API第17版。 API第17版具有第16版的下列變更。
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 1%

---

# API 17版的新增功能

Adobe Workfront於2023年10月12日發行API第17版。 API第17版具有第16版的下列變更。

## 新增的資源

<!--

### Booking (BOOKNG)

-->

### 外部檔案(EXTDOC)

ExternalDocument物件是位於Workfront外部的檔案儲存提供者中的檔案或其他數位資產。 這些資產可以連結至Workfront或從中連結。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>說明</b></p></li>
          <li><p><b>Documentproviderid</b></p></li>
          <li><p><b>分機</b></p></li>
          <li><p><b>檔案型別</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>名稱</b></p></li>
          <li><p><b>路徑</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>大小</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>說明</b></p></li>
          <li><p><b>Documentproviderid</b></p></li>
          <li><p><b>分機</b></p></li>
          <li><p><b>檔案型別</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>名稱</b></p></li>
          <li><p><b>物件代碼</b></p></li>
          <li><p><b>路徑</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>大小</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>值</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">預設欄位</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>名稱</b></p></li>
          <li><p><b>物件代碼</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObject</b></p></li>
          <li><p><b>setlinkedfoldermetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">查詢</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">營運</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### 使用者位置(USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li><p><b>分類器ID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>
        <ul>
          <li><p><b>客戶</b></p></li>
          <li><p><b>使用者</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>物件代碼</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## 已移除的資源

未移除API版本17的資源

## 已修改的資源

已針對API版本17修改下列資源。

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### 基線(BLIN)

基準線是專案在指定時間的效能快照。 這類檔案會儲存專案的關鍵資訊，例如關鍵日期、進度、成本和收入值。

基準線物件已移除旗標&#x200B;**INLINE_EDITABLE**。

### 記帳記錄(BILL)

BillingRecord物件會記錄可記帳的收入、時數或費用。 此資訊可用於在外部會計系統中建立商業發票。

BillingRecord物件已移除旗標&#x200B;**INLINE_EDITABLE**。

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### 公司(CMPY)

Company物件代表由人員集合組成的組織。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>已移除</p>
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
            <p>新增可能的值「config.defaultToNewHomeDescription」 (customer：config.defaultToNewHome)&gt;/p？<p>這可讓組織將新的「首頁」體驗設為使用者的預設體驗。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

DocumentVersion物件代表檔案的特定版本（例如書面材料、影像或其他形式的資訊）。

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
            <p>已新增可能的值「Frame.io」(FRAMEIO)</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>新增可能的值「enum.filetype.site」(site)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 匯率（匯率）

ExchangeRate物件代表Workfront中設定的貨幣匯率。 ExchangeRate物件不是動態的。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已新增下列欄位：
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>已新增。</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### 費用(EXPN)

費用代表專案期限內可能產生的非人力成本。

Expense物件已移除旗標&#x200B;**INLINE_EDITABLE**。

### 群組（群組）

群組物件代表一組使用者和團隊。 群組通常代表部門結構。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>已移除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hour (HOUR)

Hour物件代表使用者在時程表上記錄的一小時。

Hour物件已移除旗標&#x200B;**INLINE_EDITABLE**。

### 反複專案(ITRN)

反複專案物件代表單一敏捷反複專案。 反複專案是用來規劃和完成敏捷內文的離散時段。

反複專案物件已移除旗標&#x200B;**INLINE_EDITABLE**。


### 日誌專案(JRNLE)

JournalEntry物件可設定為每次修改特定物件欄位時，記錄這些欄位的相關資訊。 當欄位設定為記錄為日誌專案物件的一部分時，每次修改該欄位時都會建立對應的日誌專案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>已新增核准者(AAA)</li>
              <li>已新增檢閱者(AAR)</li>
              <li>已移除的檢閱者(ARR)</li>
              <li>已移除核准者(ARA)</li>
              <li>決定已核准(ADA)</li>
              <li>決定已核准變更(ADC)</li>
              <li>決策需求工作(ADN)</li>
              <li>決定已撤銷(ADR)</li>
              <li>核准者已變更(AAC)</li>
              <li>檢閱者已變更(ARC)</li>
              <li>檢閱完成(RDC)</li>
              <li>檢閱已撤銷(RDR)</li>
              <li>Publish (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban面板(KNBNBD)

Kanban展示板用於追蹤敏捷環境中的任務。

Kanban Board物件已移除旗標&#x200B;**INLINE_EDITABLE**。


### LinkedFolder (LNKFDR)

LinkedFolder物件代表連結自外部檔案提供者(例如Google Drive或Dropbox)的資料夾。

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
            <p>新增可能的值「Frame.io (FRAMEIO)」</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Op任務/問題(OPTASK)

OpTask物件通常稱為「問題」。 問題指工作專案，通常表示發生問題而無法完成任務或專案。 問題也可以是服務檯請求。 變更單、請求和錯誤也是問題。

問題物件已移除旗標&#x200B;**INLINE_EDITABLE**。

### 專案（專案）

專案是Workfront內的工作專案，也是Workfront協助人們完成工作的主要建置組塊。 Project物件代表具有共同特定目標的一組任務。

專案物件已移除旗標&#x200B;**INLINE_EDITABLE**。

### 專案使用者(PRTU)

ProjectUser物件代表與特定專案相關聯的使用者。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### 費率（費率）

Rate物件代表Workfront中的計費費率。

Rate物件已移除旗標&#x200B;**INLINE_EDITABLE**。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>已新增下列動作以支援費率卡功能：
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>已修改<b>setRatesForRole</b>動作以新增下列欄位：
        <ul>
        <li>分類器ID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 風險（風險）

風險物件代表可能阻止專案按時完成或在預算內完成的事件。 在計畫階段中會為專案新增風險，以在核准任何工作之前識別潛在障礙。

風險物件已移除旗標&#x200B;**INLINE_EDITABLE**。

### 角色/工作角色(ROLE)

角色物件（工作角色）代表使用者可能填入的功能容量或技能集，例如Designer或產品經理。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>已移除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 任務（任務）

Task物件代表作為達成最終目標（完成專案）的步驟而必須執行的工作專案。

Task物件已移除旗標&#x200B;**INLINE_EDITABLE**。

### 團隊(TEAMOB)

Team物件是可指派至工作專案的「使用者」集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>已移除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 團隊成員(TEAMMB)

TeamMember物件是與特定專案團隊相關聯的使用者。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 範本使用者(TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
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
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>物件代碼</b>
            </p>
            <p>已移除</p>
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
            <p><b>changeType</b>
            </p>
            <p>已新增下列值：</p>
            <ul>
              <li>已新增核准者(assetapprovalAddApprover)</li>
              <li>已新增稽核者(assetapprovalAddReviewer)</li>
              <li>已移除核准者(assetapprovalRemoveApprover)</li>
              <li>已移除稽核者(assetapprovalRemoveReviewer)</li>
              <li>決定已核准(assetapprovalDecisionApproved)</li>
              <li>決定需求工作(assetapprovalDecisionNeedsWork)</li>
              <li>決定已核准變更(assetapprovalDecisionApprovedChanges)</li>
              <li>決定已撤銷(assetapprovalDecisionRevoced)</li>
              <li>核准者已變更(assetapprovalApproverChanged)</li>
              <li>檢閱者已變更(assetapprovalReviewerChanged)</li>
              <li>檢閱完成(assetapprovalReviewerDecisionComplete)</li>
              <li>檢閱已撤銷(assetapprovalReviewerDecisionRevoced)</li>
              <li>外部檔案傳送錯誤(externalDocumentSendError)</li>
              <li>檔案版本已發佈(documentVersionPublish)</li>
              <li>連結的資料夾工作流程(linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### 使用者(USER)

使用者物件代表擁有Workfront帳戶的人員，該帳戶可以登入並與系統互動。

使用者物件已移除旗標&#x200B;**INLINE_EDITABLE**。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>工作時間</b>
            </p>
            <p>此欄位已新增，是介於0和1之間的數字，代表使用者每天可花費在專案工作（非經常性工作）的時間百分比。 值1表示使用者可以將100%的時間花在專案工作上。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 使用者群組(USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
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
            <p><b>changeType</b>
            </p>
            <p>已新增下列值：</p>
            <ul>
              <li>檔案需要您的核准(AAA)</li>
              <li>檔案需要您的稽核(AAR)</li>
              <li>檔案不再需要您的核准(ARA)</li>
              <li>檔案不再需要您的檢閱(ARR)</li>
              <li>檔案需求（使用者）核准(ATA)</li>
              <li>檔案需求（使用者）稽核(ATR)</li>
              <li>檔案不再需要（使用者）核准(RTA)</li>
              <li>檔案不再需要（使用者）的稽核(RTR)</li>
              <li>檔案已核准(ADA)</li>
              <li>檔案已核准變更(ADC)</li>
              <li>檔案需求工作(ADN)</li>
              <li>（使用者）已將（檔案）標示為已核准。 不再需要您的核准。 (AAN)</li>
              <li>（使用者）已將（檔案）標示為已核准，但有變更。 不再需要您的核准。 (ACN)</li>
              <li>（使用者）已將（檔案）標示為需要工作。 不再需要您的核准。 (AWN)</li>
              <li>檔案需要您立即稽核而非核准(AAC)</li>
              <li>檔案現在需要您的核准而非稽核(ADN)</li>
              <li>檔案已檢閱(RDC)</li>
              <li>檔案已檢閱(TRC)</li>
              <li>（使用者）已檢閱（檔案）為完成。 不再需要您的評論。 (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 使用者角色(USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>識別碼</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
