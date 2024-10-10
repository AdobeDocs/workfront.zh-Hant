---
content-type: api
navigation-topic: api-navigation-topic
title: API 18版的新增功能
description: Adobe Workfront於2022年4月6日發行API第18版。 API 18版具有下列17版中的變更。
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# API 18版的新增功能

Adobe Workfront於2024年4月8日發行API第18版。 API 18版具有下列17版中的變更。

## 新增的資源

沒有為API版本18新增資源。

## 已移除的資源

未移除API版本18的資源

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
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
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
            <p><b>動作</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
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
            <p><b>coreAction</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
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
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 等待核准(AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">營運</td>
      <td>
        <ul>
          <li>
            <p>已新增下列作業：
            </p>
            <ul>
              <li>
                <p><b>新增</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 基線(BLIN)

基準線是專案在指定時間的效能快照。 這類檔案會儲存專案的關鍵資訊，例如關鍵日期、進度、成本和收入值。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 基準線任務(BSTSK)

基準線是專案在指定時間的效能快照。 這類檔案會儲存專案的關鍵資訊，例如關鍵日期、進度、成本和收入值。 當您建立基準線時，也會擷取該基準線之基準線工作上的工作資訊。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
            <p><b>catObjCode</b>：
            </p>
            <p>已新增下列可能值：
            <ul>
              <li>
                <p><code>NLBRCY</code> （非人工資源分類）
                </p>
              </li>
              <li>
                <p><code>HOUR</code> （小時）
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> （評等卡）
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>：
            </p>
            <p>已新增下列可能值：
            <ul>
              <li>
                <p><code>NLBRCY</code> （非人工資源分類）
                </p>
              </li>
              <li>
                <p><code>HOUR</code> （小時）
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> （評等卡）
                </p>
              </li>
             </ul>
             </p>
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
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>：
            </p>
            <p>已新增下列引數：
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>：
            </p>
            <p>已新增。 這個新動作會採用下列引數：
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 財務資料(FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.open)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decisions.maked)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
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
      <td role="rowheader">動作</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>：
            </p>
            <p>已新增下列欄位：
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>：
            </p>
            <p>已新增下列欄位：
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
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
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>已新增。
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>識別碼</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>識別碼</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
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
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （檢視成本費率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （檢視收費率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （檢視一般財務）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （編輯成本費率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （編輯收費率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （編輯一般財務）</p>
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
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>已新增下列旗標：
            </p>
            <ul>
              <li>
                <p>自動載入
                </p>
              </li>
              <li>
                <p>動態
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>顯示名稱</b></p><p>已新增。</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>顯示名稱</b>
            </p><p>已新增。</p>
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
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>convertToProject</b>
            </p>
             <p>已新增下列欄位：
             <ul><li><code>copyCategories</code></li></ul>
            </p>
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
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 範本任務(TTSK)

TemplateTask物件代表屬於Template一部分的Task。 範本任務會成為使用範本之專案中的任務。<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole （團隊）

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>識別碼</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>識別碼</b>
                </p>
              </li>
             </ul>
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
            <p>已移除下列欄位：
            </p>
            <ul>
              <li>
                <p><b>物件代碼</b>
                </p>
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
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>已新增。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

UserPrefValue物件代表使用者偏好設定。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>值</b>
            </p>
            <p>已新增驗證器 <code>MAX_LENGTH</code></p>
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
            <p>已新增下列欄位：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

