---
content-type: api
navigation-topic: general-api
title: 事件訂閱版本設定
description: 事件訂閱API
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: f34f48d974db200d9ce1815c805885707ab27f6d
workflow-type: tm+mt
source-wordcount: '0'
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
>* **2026年1月15日**：所有剩餘的第1版訂閱都會移轉至第2版。

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
   <td> <p>計算的引數值</p> </td> 
   <td> <p>從包含自訂表單的範本建立的任何物件若包含已計算的引數值，將會傳送<code>CREATE</code>事件，然後會傳送<code>UPDATE</code>與引數值（包括已計算的欄位及其值）。 </p> </td> 
   <td> <p>當從包含具有計算引數值的自訂表單的範本建立物件時，只會傳送<code>CREATE</code>事件，且會包含包括計算欄位的引數值。</p> </td> 
   <td> <p>如果您有<code>UPDATE</code>個事件的訂閱，且預期在使用計算的引數值建立物件後會收到<code>UPDATE</code>個事件，則您將不會再收到該<code>UPDATE</code>個事件。 如果您希望在建立物件時檢視計算的引數值，則必須建立額外的<code>CREATE</code>訂閱。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>多重選取型別欄位</p> </td> 
   <td> <p>針對包含多選型別欄位變更的任何事件型別，如果欄位僅包含一個值，則會轉換為並以字串形式傳送。 否則，會以陣列形式傳送。 </p><p>範例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> 已轉換並以<code>myMultiSelectField: "oneValue"</code>傳送。</li><li><code>myMultiSelectField: ["first", "second"]</code> 以<code>myMultiSelectField: ["first", "second"]</code>傳送。</li></ul> </td> 
   <td> <p>無論陣列中有多少值，都會以陣列的形式傳送。 </p><p>範例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> 以<code>myMultiSelectField: ["oneValue"]</code>傳送。</li><li><code>myMultiSelectField: ["first", "second"]</code> 以<code>myMultiSelectField: ["first", "second"]</code>傳送。</li></ul> </td> 
   <td> <p>如果您的訂閱在多重選取欄位上使用篩選器，且值為字串，則必須使用具有值為陣列的相同篩選器建立新訂閱。 </p> </td> 
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

如需使用此模組的說明，請參閱Workfront Fusion檔案中的[Workfront模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules)。

如需在事件訂閱升級期間保留Workfront Fusion案例的資源，包括網路研討會影片，請參閱[在事件訂閱V2升級期間保留Fusion案例](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/td-p/754182)。
