---
content-type: api
navigation-topic: api-navigation-topic
title: API 22版的新增功能
description: Adobe Workfront於2026年5月11日發行API第22版。 API版本22具有下列版本21的變更。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 1%

---

# API 22版的新增功能

Adobe Workfront於2026年5月8日發行API 22版。 API版本22具有下列版本21的變更。

## 新增的資源

已為API 22版新增下列資源。

### ReportShareableFolder (RPSHFD)

您可以使用可共用的報表資料夾來組織報表，並和其他使用者共用這些資料夾。 此功能是專為管理大量報告並需要可擴充、一致存取控制的團隊所設計。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>ID</li>
          <li>名稱</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>ID</li>
          <li>名稱</li>
          <li>物件代碼</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">預設欄位</td>
      <td>
        <ul>
          <li>名稱</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">作業</td>
      <td>
        <ul>
          <li>新增</li>
          <li>計數</li>
          <li>DELETE</li>
          <li>編輯</li>
          <li>GET</li>
          <li>報告</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## 已移除的資源

下列資源已從API 22版中移除。

### 使用者位置(USRLOC)

此物件已移除。

## 已修改的資源

已針對API 22版修改下列資源。

### AccessLevel (ACSLVL)

AccessLevel物件與使用者相關聯，並描述決定使用者可存取內容的AccessLevelPermissions集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>下列欄位已修改，並變更了可能的值。 如需詳細資訊，請參閱開發人員檔案。
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
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
      <td>下列欄位已修改，並變更了可能的值。 如需詳細資訊，請參閱開發人員檔案。
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>下列欄位已修改，並變更了可能的值。 如需詳細資訊，請參閱開發人員檔案。
        <ul>
          <li><b>動作</b></li>
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
      <td>下列欄位已修改，並變更了可能的值。 如需詳細資訊，請參閱開發人員檔案。
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmid</b></li>
          <li><b>isCscProject</b></li>
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
      <td>已新增下列欄位。
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### 公司(CMPY)

Company物件代表由人員集合組成的組織。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmProjectID</b></li>
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
      <td>已新增
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">查詢</td>
      <td>已新增
        <ul>
          <li><p><b>assignmentStatures</b></p></li>
          <li><p><b>bookingStatures</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### 客戶（客戶）

Customer物件代表使用Workfront例項的組織。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已修改下列欄位。
        <ul>
          <li>
            <p><b>customEnumType</b>
            </p>
            <p>已新增下列可能值。</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> （預訂狀態）</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> （指派狀態）</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>新增下列欄位以支援企業儲存管理。
         <ul>
         <li><b>isLegacycustomerEsmStorageEnabled</b></li>
         <li><b>isLegacycustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
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
      <td>已修改下列欄位。
        <ul>
          <li>
            <p><b>customEnumType</b>
            </p>
            <p>新增下列可能的值以支援企業儲存體管理：</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### 檔案（檔案）

Document物件代表檔案（例如書面材料、影像或其他形式的資訊）。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmid</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>已修改下列動作。
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>新增下列欄位以支援企業儲存管理。
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>物件ID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder (DOCFDR)

檔案可整理到資料夾中。 您可以在個人的「檔案」區域中建立個人資料夾。 DocumentFolder物件代表其中一個資料夾。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmid</b></li>
          <li><b>isEsmFolder</b></li>
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
      <td>新增下列欄位以支援企業儲存體管理。
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      已修改下列欄位。
        <ul>
          <li><b>version</b><p>移除驗證器「必要」。</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>已新增下列動作。
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">作業</td>
      <td>已新增下列作業。
        <ul>
          <li><p><b>編輯</b></p>
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
      <td>已新增下列欄位。
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
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
      <td>已修改下列欄位。
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>已新增下列可能值。</p>
             <ul>
              <li>
                <p><code>PFM</code>（行動資料夾）</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>旗標</b>
            </p>
            <p>已新增下列可能值。</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### 日誌欄位(JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已修改下列欄位。
        <ul>
          <li>
            <p><b>動作</b>
            </p>
            <p>已新增下列可能值。</p>
             <ul>
              <li>
                <p><code>PFM</code>（行動資料夾）</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### Op任務(OPTASK)

OpTask物件通常稱為「問題」。 問題指工作專案，通常表示發生問題而無法完成任務或專案。 問題也可以是服務檯請求。 變更單、請求和錯誤也是問題。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li><b>實際所需工作</b><p>已新增下列旗標：
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">搜尋欄位</td>
      <td>
        <ul>
          <li><b>實際工作</b><p>型別從<code>null</code>變更為<code>double</code>。</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">作業</td>
      <td>已新增下列作業。
        <ul>
          <li><p><b>計數</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>報告</b></p>
          <li><p><b>SEARCH</b></p>
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
      <td>已新增下列欄位。
        <ul>
          <li><b>enteredById</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### 引數群組(PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已新增下列欄位。
        <ul>
          <li><b>enteredById</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection (PTLSEC)

PortalSection物件是報表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已新增下列欄位。
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>已新增下列欄位。
        <ul>
          <li><b>reportShareableFolder</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Portfolio （連線埠）

Portfolio物件是競爭相同資源（通常是金錢或人力）的專案集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmid</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnable</b></li>
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
      <td role="rowheader">直接欄位</td>
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmid</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnable</b></li>
        </ul>
      已修改下列欄位。
        <ul>
          <li><b>portfolioID</b><p>新增驗證器「必要」。</li>
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
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmid</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnable</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef (QUED)

QueueDef物件代表Workfront中的請求佇列定義。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>下列欄位已修改，並變更了可能的值。 如需詳細資訊，請參閱開發人員檔案。
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 排程報告(SCHREP)

ScheduledReport物件代表已設定為排程傳送的報表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已修改下列欄位，並對可能的值做了大量變更。 如需詳細資訊，請參閱開發人員檔案。
        <ul>
          <li><b>格式</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 任務（任務）

Task物件代表作為達成最終目標（完成專案）的一部分而必須完成的工作專案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>已新增</p></li>
          <li><p><b>實際所需工作</b></p><p>已新增旗標<code>AUTO_LOAD</code>和<code>DYNAMIC</code>。</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>已新增</p>
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
      <td role="rowheader">直接欄位</td>
      <td>新增下列欄位以支援企業儲存管理。
        <ul>
          <li><b>esmid</b></li>
          <li><b>isCscProject</b></li>
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
      <td>已修改下列欄位。
        <ul>
          <li>
            <p><b>動作</b>
            </p>
            <p>已新增下列可能的值。</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
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
      <td role="rowheader">直接欄位</td>
      <td>已新增下列欄位。
        <ul>
          <li><b>Eauthuserid</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>下列欄位已移除。
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





