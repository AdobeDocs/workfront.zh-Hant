---
content-type: api
navigation-topic: api-navigation-topic
title: API 21版的新增功能
description: Adobe Workfront於2025年10月23日發行API版本21。 API版本21具有下列版本20的變更。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 50edbfa342ed7f51d1fe2b9654b55b579bb3f5af
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 4%

---

# API 21版的新增功能

Adobe Workfront於2025年10月23日發行API版本21。 API版本21具有下列版本20的變更。

## 新增的資源

### PoweringPlanTemplate (SPTMPL)

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
      <td role="rowheader">營運</td>
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

### AssignmentBillingRole (ASBLRL)

AssignmentBillingRole物件及其所有欄位已移除。

## 已修改的資源

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
            <p><b>coreAction</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
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
            <p><b>動作</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
         </li>
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
            <p><b>coreAction</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 宣告附件(ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>副檔名</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>團隊指派</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### 指定任務(ASSGN)

Assignment物件代表工作專案與指派處理該工作專案的使用者、專案團隊或群組之間的連線。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>已移除</p>
              </li>
            </ul>
         </li>
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
            <p><b>catObjCode</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> （團隊）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> （團隊）</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 客戶（客戶）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> （停用用於時間表計算的Java applet）
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 檔案（檔案）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 檔案資料夾

DocumentFolder物件已新增旗標`RESTORABLE`。

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
            <p><b>getTeresirmationCommentmporaryCloudURL</b>
            </p>
            <p>已新增驗證器 <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
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
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
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
        <ul>
          <li>
            <p><b>資料型別</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>RICHLX</code> （辭彙RTF文字）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> （單行統計）</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>已新增</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">預設欄位</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>已新增</p>
           </li>
           </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>貨幣</b>
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

QueueDef物件代表佇列，這是已發佈至服務檯區域的專案，可讓使用者向其提交問題。

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
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （編輯聯絡資訊）</p>
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
            <p><b>服務檯專案</b>
            </p>
            <p>已新增</p>
            </li>
            </ul>
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
            <p><b>localBillingPerHour</b>
            </p>
            <p>已移除</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>已移除</p>
              </li>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>格式</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，而這些問題的答案可讓經理瞭解專案與產品組合目標的對齊程度。<table>
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
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> （單行統計）</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### 人員配置計畫

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>已新增</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>已新增</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### 人員配置計畫資源

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>已新增</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>已新增</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>已新增</p>
              </li>
            </ul>
         </li>
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
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>團隊指派</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### 團隊

Team物件已新增旗標`DATA_EXTENDIBLE`和`SHARABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>類別識別碼</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">參考欄位</td>
      <td>
        <ul>
          <li>
            <p><b>類別</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>物件類別</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### 範本指派

TemplateAssignment物件已新增旗標`ATTRIBUTE_ATTACHABLE`。

### 時程表(TSHET)

時程表物件代表虛擬時程表，可讓使用者輸入任務、專案和管理費用時數型別的實際工作時數。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">核心欄位</td>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
            <p><b>團隊指派</b>
            </p>
            <p>已新增</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


