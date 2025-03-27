---
content-type: api
navigation-topic: api-navigation-topic
title: API 19版的新增功能
description: Adobe Workfront於2022年4月6日發行API第19版。 API 19版具有下列18版中的變更。
author: Becky
feature: Workfront API
role: Developer
exl-id: 84909dea-7ce1-4ad3-90f5-9dbdb354eaa4
source-git-commit: 1c1f9f46ea25ffa7d01c1a762b0478a5edb3339e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# API 19版的新增功能

Adobe Workfront於2024年4月8日發行API第19版。 API 19版具有下列18版中的變更。

## 新增的資源

未針對API版本19新增資源。

## 已移除的資源

未移除API版本19的資源

## 已修改的資源

### AccessLevel (ACSLVL)

AccessLevel物件與使用者相關聯，並描述決定使用者可存取內容的AccessLevelPermissions集合。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>已新增下列可能值：
            </p>
            <ul>
              <li>
                <p>停用Workfront AI助理(AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 指定任務(ASSGN)

Assignment物件代表工作專案與指派處理該工作專案的使用者、專案團隊或群組之間的連線。

工作分派物件已新增旗標&#x200B;**DATA_EXTENDIBLE**。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已新增下列直接欄位：
        <ul>
          <li>
            <p><b>categoryID</b><p>類別是自訂表單。 此欄位支援將自訂表單新增到指派的功能。
            </p>
          </li>
          <li>
            <p><b>優先順序</b><p>此欄位允許下列值：
            <ul>
              <li>0 （無）</li>
              <li>1 （低）</li>
              <li>2 （一般）</li>
              <li>3 （高）</li>
              <li>4 （緊急）</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>已新增下列參考欄位：
        <ul>
          <li>
            <p><b>類別</b><p>類別是自訂表單。 此欄位支援將自訂表單新增到指派的功能。
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>已新增下列集合欄位：
        <ul>
          <li>
            <p><b>物件類別</b><p>類別是自訂表單。 此欄位支援將自訂表單新增到指派的功能。
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### 類別(CTGY)

類別物件是自訂表單。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已新增下列欄位以支援新增自訂表單至指派的功能。
        <ul>
          <li>
            <p><b>catObjCode</b><p>已新增下列可能值：
            </p>
            <ul>
              <li>
                <p>指定任務(ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>物件型別</b><p>已新增下列可能值：
            </p>
            <ul>
              <li>
                <p>指定任務(ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 分類器(CLSF)

分類器是一個位置。

<table>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>已新增下列動作：
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### 客戶

Customer物件代表使用Workfront例項的組織。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumType</b><p>已新增下列可能值：
            </p>
            <ul>
              <li>
                <p>指定優先順序(PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>CustomEnum物件可協助將狀態代碼轉換為人類看得懂的文字。</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 客戶偏好設定(CUSTPR)

CustomerPreferences物件代表客戶已針對其Workfront例項設定的偏好設定集。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>名稱</b><p>已移除下列可能值：
            </p>
            <ul>
              <li>
                <p>在更新串流中啟用縮放整合(password：zoomIntegrationEnabled)
                </p>
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
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>已新增欄位<code>folderID</code>。</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>已新增。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### 匯率（匯率）

ExchangeRate物件代表Workfront中設定的貨幣匯率。 ExchangeRate物件不是動態的。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
      <ul>
      <li>下列欄位已新增驗證器<code>REQUIRED</code>：
        <ul>
          <li><p><b>貨幣</b></li>
          <li><p><b>評等</b></li></ul>
      <li>已新增下列欄位：
        <ul>
          <li><p><b>enteredById</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>
      <ul>
        <li>已新增下列欄位：
        <ul>
          <li><p><b>輸入者</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 群組（群組）

群組物件代表一組使用者和團隊。 群組通常代表部門結構。

群組物件已新增旗標&#x200B;**可共用**。

### Hour (HOUR)

Hour物件代表使用者在時程表上記錄的一小時。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
      已新增下列欄位：
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>rejectedByID</b></li>
          <li><p><b>rejectedOnDate</b></li>
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submittedById</b></li>
          </ul>
          <p>已對<b>小時</b>欄位進行下列變更。</p>
          <ul> 
          <li> 已移除驗證器<b>GREATER_THAN</b></li>
          <li> 已新增驗證器<b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">動作</td>
      <td>
      已新增下列動作：
        <ul>
          <li><p><b>核准</b></li>
          <li><p><b>取消核准</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### 日誌專案(JRNLE)

JournalEntry物件可設定為每次修改特定物件欄位時，記錄這些欄位的相關資訊。 當欄位設定為記錄為日誌專案物件的一部分時，每次修改該欄位時都會建立對應的日誌專案。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>標幟</b><p>已新增下列可能值：
            </p>
            <ul>
              <li>
                <p>為成本率(CR)
                </p>
              </li>
              <li>
                <p>記帳費率(BR)
                </p>
              </li>
              <li>
                <p>為一般財務(GF)
                </p>
              </li>
              <li>
                <p>為組合財務(CF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 引數（引數）

Parameter物件是自訂欄位。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>資料型別</b></p><p>已新增下列可能值：
            <ul>
            <li>期間(DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>顯示型別</b></p><p>為了建立更方便使用者且更彈性的系統，<b>Widget (WIDGET)</b>欄位型別已過時，並分割為下列欄位型別：
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>影像（影像）</li>
            <li>PDF (PDF)</li>
            <li>視訊（視訊）</li>
            <li>外部查詢(EXTRNL)</li>
            <li>多重選取外部查閱(MULTEXTRNL)</li>
            <li>原生欄位(WFNATIVE)</li>
            <li>計畫欄位(WFPLANNING)</li>
            <li>時間階段KPI （時間階段）</li>
            <li>統計（統計）</li>
            <li>檔案（檔案）</li>
           </ul>
          </li>
          <li>
            <p><b>設定</b><p>已新增。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### 角色(ROLE)

角色物件（工作角色）代表使用者可能填入的功能容量或技能集，例如Designer或產品經理。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
    已新增下列欄位：
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>
        已新增下列欄位：
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScorecardQuestion {#scorecardquestion}

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，而這些問題的答案可讓經理瞭解專案與產品組合目標的對齊程度。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
            <p><b>顯示型別</b></p><p>為了建立更方便使用者且更彈性的系統，<b>Widget (WIDGET)</b>欄位型別已過時，並分割為下列欄位型別：
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>影像（影像）</li>
            <li>PDF (PDF)</li>
            <li>視訊（視訊）</li>
            <li>外部查詢(EXTRNL)</li>
            <li>多重選取外部查閱(MULTEXTRNL)</li>
            <li>原生欄位(WFNATIVE)</li>
            <li>計畫欄位(WFPLANNING)</li>
            <li>時間階段KPI （時間階段）</li>
            <li>統計（統計）</li>
            <li>檔案（檔案）</li>
           </ul>
      </td>
  </tbody>
</table>

### 範本指派(TASSGN)

TemplateAssignment物件代表範本任務與受指派處理該任務的使用者、專案團隊或群組之間的連線。 當範本用於專案時，該使用者、團隊或群組會指派給任務。

TemplateAssignment物件已新增旗標&#x200B;**DATA_EXTENDIBLE**。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>已新增下列直接欄位：
        <ul>
          <li>
            <p><b>categoryID</b><p>類別是自訂表單。 此欄位支援將自訂表單新增到指派的功能。
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>已新增下列參考欄位：
        <ul>
          <li>
            <p><b>類別</b><p>類別是自訂表單。 此欄位支援將自訂表單新增到指派的功能。
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>已新增下列集合欄位：
        <ul>
          <li>
            <p><b>物件類別</b><p>類別是自訂表單。 此欄位支援將自訂表單新增到指派的功能。
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
  <tbody>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>物件代碼</b></p><p>已移除。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>
