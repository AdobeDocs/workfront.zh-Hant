---
content-type: api
navigation-topic: general-api
title: 事件訂閱版本設定
description: 事件訂閱API
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: 82694183c32938905f1f8542c430d3c453274cb6
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 0%

---

# 事件訂閱版本設定

Workfront有兩個版本的事件訂閱。 本文會說明兩者之間的差異。

新版本並非變更Workfront API，而是變更事件訂閱功能。

升級或降級事件訂閱的功能可確保事件結構變更時，現有訂閱不會中斷，讓您測試和升級至新版本，不會有事件訂閱的間隙。


將事件訂閱升級或降級至另一個版本時，在版本變更後的五分鐘內，您會收到每個事件傳送的重複事件。 重複專案包括事件訂閱版本1和版本2各一個。 這可確保不會因為變更事件訂閱版本而遺漏任何事件。

如需用於升級或降級事件訂閱的端點資訊，請參閱文章事件訂閱API中的[事件訂閱版本設定](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)。

>[!IMPORTANT]
>
>下列版本將影響事件訂閱版本設定：
>
>* **25.2版** （2025年4月10日）：在25.2版之後建立的所有新訂閱皆建立為版本2。
>* **25.3版** （2025年7月17日）：在25.3版發行後，訂閱無法再降級為版本1。
>* **2025年9月1日**：所有剩餘的第1版訂閱都會移轉至第2版。

## 第1版與第2版之間的變更

已對事件訂閱版本2進行下列變更：


### 一般變更


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>受影響的欄位</b></p> </th> 
   <th> <p><b>第1版（先前行為）</b></p> </th> 
   <th> <p><b>第2版（變更）</b></p> </th> 
   <th> <p><b>修正動作</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>引數值</p> </td> 
   <td> <p>對於從包含自訂表單的範本建立的任何物件，會傳送<code>CREATE</code>事件，然後隨引數值（包括計算欄位及其值）傳送<code>UPDATE</code>。    </p> </td> 
   <td> <p>當從包含具有計算引數值的自訂表單的範本建立物件時，只會傳送<code>CREATE</code>事件，且會包含包括計算欄位的引數值。</p> </td> 
   <td> <p>如果您有訂閱 <tr><ul><ul><code>UPDATE<code> events and are expecting to receive an <code>UPDATE</code> event after an object is created with calculated parameter values, you will no longer receive that <code>UPDATE</code> event. If you wish to see calculated parameter values on object creation, you must create an additional <code>CREATE</code> subscription.</p> </td> 
  </tr> 
   
   <td> <p>Multi-Select type fields</p> </td> 
   <td> <p>For any type of event that contains a change on a multi-select type field, if the field only contained one value it would be converted to and sent as a string. Otherwise it would be sent as an array. </p><p>Examples:</p><li><code>myMultiSelectField: ["oneValue"]</code> is converted and sent as <code>myMultiSelectField: "oneValue"</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Regardless of how many values are in the array, it will be sent as an array. </p><p>Examples:</p><li><code>myMultiSelectField: ["oneValue"]</code> is sent as <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>If you have a subscription with a filter on a multi-select field, and the value as a string, you must create a new subscription with the same filter that has the value as an array. </p> </td> 
  </tr> 
 </tbody> 
</table>

### 物件特定變更

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>物件代碼</b> </th> 
   <th> <b>受影響的欄位</b> </th> 
   <th> <b>第1版（先前行為）</b></th> 
   <th> <b>版本2 （變更）</b> </th> 
   <th> <b>補救動作</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">指派</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>更新此物件時，<code>UPDATE</code>事件有時會錯誤地顯示受影響的欄位從<code>null</code>變更為<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果受影響的欄位有篩選器，則只有在這些欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他值已變更時收到。
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">檔案</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>在此物件上更新任何引數值時，<code>UPDATE</code>事件未正確地顯示從<code>null</code>到<code>object id</code>受影響的欄位變更。 </td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果受影響的欄位有篩選器，則只有在這些欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他值已變更時收到。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>刪除檔案時，<code>DELETE</code>事件將受影響的欄位錯誤地顯示為之前狀態的空白陣列。    </td> 
   <td><code>DELETE</code>事件正確顯示處於之前狀態的受影響欄位。</td> 
   <td>無。 <code>DELETE</code>事件仍會傳送，但現在會顯示受影響欄位的正確資料。 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>更新此物件時，將會傳送兩個<code>UPDATE</code>事件。 第一個事件未包含受影響的欄位，而第二個事件包含。</td> 
   <td>所有欄位更新（包括受影響的欄位）都只會出現在一個<code>UPDATE</code>事件中，而不會傳送第二個不必要的事件。     </td> 
   <td>無。 如果受影響的欄位有篩選條件，事件會在第一個事件中傳送。 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">費用</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>在費用上更新任何引數值時，<code>UPDATE</code>事件錯誤地顯示了topReferenceObjCode從<code>EXPNS</code>到<code>PROJ</code>的變更，以及<code>referenceObjectName</code>從<code>null</code>到<code>string value of project name</code>的變更。      </td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果受影響的欄位有篩選器，則只有在這些欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他值已變更時收到。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>刪除Expense物件時，會傳送<code>UPDATE</code>事件，並在傳送<code>DELETE</code>事件之前將受影響的欄位變更為Null。    </td> 
   <td>未傳送額外的<code>UPDATE</code>事件。 <code>DELETE</code>事件具有先前狀態中受影響欄位的正確值。 </td> 
   <td>如果您有<code>UPDATE</code>事件中受影響欄位的篩選器，且您希望在物件被刪除時收到該篩選器，則您將不再收到該<code>UPDATE</code>事件。 如果您希望在刪除物件時看到這些欄位，則必須建立額外的<code>DELETE</code>訂閱。
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HOUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>刪除此物件時，<code>DELETE</code>事件將受影響的欄位錯誤地顯示為<code>null</code>在之前的狀態。 </td> 
   <td><code>DELETE</code>事件正確顯示受影響欄位在「之前」狀態。</td> 
   <td>無。 <code>DELETE</code>事件仍會傳送，但現在會顯示受影響欄位的正確資料。 </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>在此物件上更新任何引數值時，<code>UPDATE</code>事件未正確地顯示從<code>null</code>到<code>ID value</code>受影響的欄位變更。 </td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果您在受影響的欄位上有篩選器，則只有在欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他引數值已變更時收到。
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>更新此物件時，<code>UPDATE</code>事件有時會錯誤地顯示受影響的欄位從<code>null</code>變更為<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件將顯示受影響欄位的正確值。    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">專案</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>在此物件上更新任何引數值時，<code>UPDATE</code>事件未正確地顯示從<code>null</code>到<code>ID value</code>受影響的欄位變更。 </td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果您在受影響的欄位上有篩選器，則只有在欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他引數值已變更時收到。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>更新此物件時，<code>UPDATE</code>事件有時會錯誤地顯示受影響的欄位從<code>null</code>變更為<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果您在受影響的欄位上有篩選器，則只有在欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他引數值已變更時收到。
  </tr> 
  <tr> 
   <th rowspan="2">任務</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>在此物件上更新任何引數值時，<code>UPDATE</code>事件未正確地顯示從<code>null</code>到<code>ID value</code>受影響的欄位變更。 </td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果您在受影響的欄位上有篩選器，則只有在欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他引數值已變更時收到。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>更新此物件時，<code>UPDATE</code>事件有時會錯誤地顯示受影響的欄位從<code>null</code>變更為<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件都會顯示受影響欄位的正確值。</td> 
   <td>無。 如果您在受影響的欄位上有篩選器，則只有在欄位實際變更時，才會收到<code>UPDATE</code>事件，而不會在任何其他引數值已變更時收到。
 </tbody> 
</table>


## 更新Workfront Fusion案例中的事件訂閱版本

Workfront Fusion使用事件訂閱來監視Workfront中的變更以觸發情境。 您可以使用「Workfront >更新事件裝載版本」模組，更新Fusion直接在案例中使用的事件訂閱版本。

如需使用此模組的說明，請參閱Workfront Fusion檔案中的[Workfront模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules)。
