---
content-type: api
navigation-topic: api-navigation-topic
title: API 20版的新增功能
description: Adobe Workfront於2022年4月6日發行API版本20。 API 20版具有下列19版中的變更。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# API 20版的新增功能

Adobe Workfront於2025年5月4日發行API 20版。 API 20版具有下列19版中的變更。

## 新增的資源

未針對API版本20新增資源。

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## 已移除的資源

未移除API版本20的資源

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
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>實際成本</li>
              <li>actualExpenseCost</li>
              <li>實際勞力成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>實際值</li>
              <li>billedRevenue</li>
              <li>預算</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>costamount</li>
              <li>costType</li>
              <li>固定成本</li>
              <li>fixedrevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>計畫成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>風險績效指數</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>實際成本</li>
          <li>actualRevenue</li>
          <li>計畫成本</li>
          <li>plannedrevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>已新增旗標<code>DYNAMIC</code>、<code>LAZY_READ</code>和 <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>已新增標幟 <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>已新增可能的值<code>URH</code> （使用者和角色每小時） </li>
          <li><p><b>revenualtype</b></p> <p>已新增可能的值<code>URH</code> （使用者和角色每小時）、<code>URC</code> （使用者和角色每小時上限）和<code>URF</code> （使用者和角色每小時加固定）</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
          <p>已新增下列欄位：</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### 指定任務(ASSGN)

Assignment物件代表工作專案與指派處理該工作專案的使用者、專案團隊或群組之間的連線。

工作分派物件已新增旗標`ATTRIBUTE_ATTACHABLE`和`DOMAIN_EXTENDABLE`。


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### 頭像

頭像物件是使用者像片。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>已新增</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心欄位</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>已新增</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">營運</td>
      <td>
        <ul>
          <li>
            <p><b>副本</b>
            </p>
             <p>已新增</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>實際成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>預算</li>
              <li>eac</li>
              <li>plannedBillableExpenseCost</li>
              <li>計畫成本</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>實際成本</li>
          <li>計畫成本</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>已新增標幟 <code>CURRENCY</code></li>
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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>實際成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>計畫成本</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>實際成本</li>
          <li>計畫成本</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>已新增標幟 <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 記帳記錄(BILL)

BillingRecord物件會記錄可記帳的收入、時數或費用。 此資訊可用於在外部會計系統中建立商業發票。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>數量</li>
              <li>其他金額</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>已新增</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

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
            <p><b>組態</b>
            </p>
             <p>已新增</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 公司(CMPY)

Company物件代表由人員集合組成的組織。

公司物件已新增旗標`SHARABLE`。

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleassignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissuemove)</p></li>
            </ul>
          </li>
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
      <td>
           <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>評等</li>
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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixRevenue</li>
              <li>實際勞力成本</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>固定成本</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedFixedRevenue</li>
              <li>plannedLaborCost</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

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
            <p><b>貨幣</b>
            </p>
             <p>已新增</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>實際成本</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
              <li>實際成本</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>已新增</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### Op任務(OPTASK)

OpTask物件通常稱為「問題」。 問題指工作專案，通常表示發生問題而無法完成任務或專案。 問題也可以是服務檯請求。 變更單、請求和錯誤也是問題。

OpTask物件已新增標幟DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>實際成本</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
              <li>實際成本</li>
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
                <p><code>INTRNL</code> （內部查詢）</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> （多重選取內部查詢）</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio （連線埠）

Portfolio物件是競爭相同資源（通常是金錢或人力）的專案集合。

Portfolio物件已新增標幟`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>已對齊</li>
              <li>預算</li>
              <li>貨幣</li>
              <li>淨值</li>
              <li>預算</li>
              <li>準時</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### 方案(PRGM)

計畫物件是投資組合中專案的子集，其中類似的專案可以分組在一起。

程式物件已新增旗標`DOMAIN_EXTENDABLE`。

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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>實際成本</li>
              <li>actualExpenseCost</li>
              <li>實際勞力成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>實際值</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>billedRevenue</li>
              <li>預算</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>eac</li>
              <li>固定成本</li>
              <li>fixedrevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>計畫成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedrevenue</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>風險績效指數</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>實際成本</li>
          <li>actualRevenue</li>
          <li>計畫成本</li>
          <li>plannedrevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>已新增標幟 <code>CURRENCY</code></li>
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
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （從自訂資料移除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （新增子專案）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 費率（費率）

Rate物件代表Workfront中的計費費率。

Rate物件已新增旗標`ATTRIBUTE_ATTACHABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>已新增下列欄位：
          <ul>
          <li>貨幣</li>
          <li>已鎖定</li>
          <li>類型</li>
          <li>值</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 角色(ROLE)

角色物件（工作角色）代表使用者可能填入的功能容量或技能集，例如Designer或產品經理。

角色物件已新增旗標`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
        <ul>
          <li>
          <p>已新增下列欄位：
          <ul>
          <li>billingRates</li>
          <li>costRates</li>
          </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>格式</b>
            </p>
             <p>已新增下列可能值：</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

ScoreCardQuestion物件代表已新增至計分卡的問題。 這些問題通常由Portfolio經理決定，而這些問題的答案可讓經理瞭解專案與產品組合目標的對齊程度。

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
             <p>已新增下列可能值：</p>
             <ul>
              <li><p><code>INTRNL</code> （內部查詢）</p></li>
              <li><p><code>MULTINTRNL</code> （多重選取內部查詢）</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 任務（任務）

Task物件代表作為達成最終目標（完成專案）的步驟而必須執行的工作專案。

Task物件已新增旗標`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>實際成本</li>
              <li>actualExpenseCost</li>
              <li>實際勞力成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costamount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedrevenue</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>實際成本</li>
          <li>actualRevenue</li>
          <li>計畫成本</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>已新增下列可能值：<ul><li><code>URH</code> （使用者和角色每小時）</li></ul></li>
          <li><p><b>revenualtype</b></p> <p>已新增下列可能值：<ul><li><code>URH</code> （使用者和角色每小時）</li><li><code>URC</code> （受限的使用者和角色小時）</li><li><code>URF</code> （使用者和角色每小時加固定）</li></ul></li>
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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>預算</li>
              <li>固定成本</li>
              <li>fixedrevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>計畫成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedrevenue</li>
              <li>plannedRiskCost</li>
              <li>所需工作</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>計畫成本</li>
          <li>plannedrevenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
          <p>已新增下列欄位：</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### 範本任務(TTSK)

TemplateTask物件代表屬於Template一部分的Task。 範本任務會成為使用範本之專案中的任務。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>billingAmount</li>
              <li>costamount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedrevenue</li>
              <li>revenualtype</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>計畫成本</li>
          <li>plannedrevenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>已新增下列可能值：<ul><li><code>URH</code> （使用者和角色每小時）</li></ul></li>
          <li><p><b>revenualtype</b></p> <p>已新增下列可能值：<ul><li><code>URH</code> （使用者和角色每小時）</li><li><code>URC</code> （受限的使用者和角色小時）</li><li><code>URF</code> （使用者和角色每小時加固定）</li></ul></li>
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
        <ul>
          <li>
            <p><b>物件代碼</b>
            </p>
             <p>已移除</p>
          </li>
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
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 使用者(USER)

使用者物件代表擁有Workfront帳戶的人員，該帳戶可以登入並與系統互動。

使用者物件已新增欄位`ATTRIBUTE_ATTACHABLE`和`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接欄位</td>
      <td>
        <ul>
          <li>
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">集合欄位</td>
      <td>
          <p>已新增下列欄位：</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
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
            <p>下列欄位已新增旗標<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>實際成本</li>
              <li>actualExpenseCost</li>
              <li>實際勞力成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costamount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>計畫成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedrevenue</li>
            </ul>
          </li>
          <li>
          <p>下列欄位將其型別從<code>double</code>變更為<code>class java.math.BigDecimal</code>：
          <ul>
          <li>實際成本</li>
          <li>actualRevenue</li>
          <li>計畫成本</li>
          <li>plannedrevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>已新增旗標<code>DYNAMIC</code>、<code>LAZY_READ</code>和 <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>已新增標幟 <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>已新增可能的值<code>URH</code> （使用者和角色每小時） </li>
          <li><p><b>revenualtype</b></p> <p>已新增可能的值<code>URH</code> （使用者和角色每小時）、<code>URC</code> （使用者和角色每小時上限）和<code>URF</code> （使用者和角色每小時加固定）</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



