---
content-type: api
navigation-topic: workfront-objects
title: 類別
description: 「類別」物件可用的欄位表格，及其說明和值型別。
author: Becky
feature: Workfront API
role: Developer
exl-id: 24c900ee-a8f1-458e-a18b-c098c6314e0c
source-git-commit: 8c72a44c49d137c6c73f7c213cb411e45f5a6e24
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 28%

---


# 類別

<!-- Audited: 5/2025 -->

<!--Fieldsclass: "java.lang.IllegalArgumentException",  
message: "APIModel INTERNAL does not support field projectid (OpTask)"-->

<table style="table-layout:auto"> 
 <col width="100"> 
 <col width="100"> 
 <col width="100"> 
 <col width="240"> 
 <col width="200"> 
 <col width="100"> 
 <thead> 
  <tr> 
   <th>姓名</th> 
   <th>標籤</th> 
   <th>類型</th> 
   <th>說明</th> 
   <th>可能的值</th> 
   <th>標誌</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}"><strong>識別碼</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}">ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Identifying GUID&quot;}">識別GUID</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;accessorIDs&quot;}"><strong>accessorIDs</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;acessorIDs&quot;}">存取子IDs</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String Array&quot;}">字串陣列</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;List of People/Team IDs that can access this object&quot;}">可存取此物件的人員/團隊ID清單</td> 
   <td> </td> 
   <td> <p><span class="dtRead">唯讀</span> </p> <p><span class="dtLazy">延遲讀取</span> </p> <p><span class="dtDyn">動態</span> </p> <p><span class="dtGrp">無法分組</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;catObjCode&quot;}"><strong>catObjCode</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">類型</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type of Object the Custom form is related to&quot;}">與自訂表單相關的物件型別</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;[{\&quot;label\&quot;:\&quot;Company\&quot;,\&quot;value\&quot;:\&quot;CMPY\&quot;},{\&quot;label\&quot;:\&quot;Task\&quot;,\&quot;value\&quot;:\&quot;TASK\&quot;},{\&quot;label\&quot;:\&quot;Project\&quot;,\&quot;value\&quot;:\&quot;PROJ\&quot;},{\&quot;label\&quot;:\&quot;Portfolio\&quot;,\&quot;value\&quot;:\&quot;PORT\&quot;},{\&quot;label\&quot;:\&quot;Program\&quot;,\&quot;value\&quot;:\&quot;PRGM\&quot;},{\&quot;label\&quot;:\&quot;User\&quot;,\&quot;value\&quot;:\&quot;USER\&quot;},{\&quot;label\&quot;:\&quot;Document\&quot;,\&quot;value\&quot;:\&quot;DOCU\&quot;},{\&quot;label\&quot;:\&quot;Issue\&quot;,\&quot;value\&quot;:\&quot;OPTASK\&quot;},{\&quot;label\&quot;:\&quot;Expense\&quot;,\&quot;value\&quot;:\&quot;EXPNS\&quot;},{\&quot;label\&quot;:\&quot;Iteration\&quot;,\&quot;value\&quot;:\&quot;ITRN\&quot;}]&quot;}"><code>[{"label":"Company","value":"CMPY"},{"label":"Task","value":"TASK"},{"label":"Project","value":"PROJ"},{"label":"Portfolio","value":"PORT"},{"label":"Program","value":"PRGM"},{"label":"User","value":"USER"},{"label":"Document","value":"DOCU"},{"label":"Issue","value":"OPTASK"},{"label":"Expense","value":"EXPNS"},{"label":"Iteration","value":"ITRN"}]</code> </td> 
   <td> <p><span class="dtEdit">可編輯</span> </p> <p><span class="dtReq">必要</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;customerID&quot;}"><strong>customerID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Customer ID&quot;}">客戶 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the Customer&quot;}">客戶的ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">無法分組</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;description&quot;}"><strong>描述</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">說明</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">說明</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">可編輯</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;enteredByID&quot;}"><strong>enteredByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Entered By ID&quot;}">輸入者 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the User that added the Custom Form&quot;}">新增自訂表單的使用者ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">無法分組</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;extRefID&quot;}"><strong>extRefID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;External Reference ID&quot;}">外部參考 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;User Editable Field inteded to be used a link to an external object&quot;}">使用者可編輯欄位，用於連結外部物件</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">可編輯</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;groupID&quot;}"><strong>groupID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Group ID&quot;}">群組 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the first group with access to the custom form&quot;}">可存取自訂表單的第一個群組ID</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">可編輯</span> </p> <p><span class="dtGrp">無法分組</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;hasCalculatedFields&quot;}"><strong>hasCalculatedField</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Has Calculated Fields&quot;}">有計算欄位</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Boolean&quot;}">布林值</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Does the form have calculated fields associated with it?&quot;}">表單是否有相關的計算欄位？</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">無法分組</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdateDate&quot;}"><strong>lastUpdateDate</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Update Date&quot;}">上次更新日期</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date/Time&quot;}">日期/時間</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date of when the object was last modified&quot;}">上次修改物件的日期</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdatedByID&quot;}"><strong>lastUpdatedByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Updated By ID&quot;}">上次更新者 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the last user to Update the object&quot;}">上次更新物件的使用者識別碼</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">無法分組</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;name&quot;}"><strong>名稱</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name&quot;}">姓名</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">字串</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name of the Object&quot;}">物件的名稱</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">可編輯</span> </p> <p><span class="dtReq">必要</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 參考

| 姓名 | 標籤 | 類型 | 輸入物件程式碼 |
|---|---|---|---|
| 客戶 | 客戶 | 客戶 | 客戶 |
| 輸入者 | 輸入者 | 使用者 | 使用者 |
| 群組 | 群組 | 群組 | 群組 |
| 上次更新者 | lastUpdatedBy | 使用者 | 使用者 |


## 集合

| 姓名 | 標籤 | 類型 | 輸入物件程式碼 |
|---|---|---|---|
| 存取權限規則 | accessRules | 存取規則 | ACSURL |
| 類別存取規則 | categoryAccessRules | 類別存取規則 | 字幕 |
| 類別重疊顯示規則 | categoryCascadeRules | 類別重疊顯示規則 | CTCSRL |
| 類別參數 | categoryParameters | 類別參數 | CTGYPA |
| 其他群組 | 其他群組 | 群組 | 群組 |


## 動作

| 標籤 | 姓名 | 引數 |
|---|---|---|
| 指派類別 | assignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| 指派類別 | assignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
| 取消指派類別 | unassignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| 取消指派類別 | unassignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
