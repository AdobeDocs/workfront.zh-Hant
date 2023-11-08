---
content-type: api
navigation-topic: general-api
title: 事件訂閱API
description: 事件訂閱API
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: 7f11ddf290c24ac3436ea98f14eff1338388f314
workflow-type: tm+mt
source-wordcount: '2123'
ht-degree: 3%

---


# 事件訂閱API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

當事件訂閱支援的Adobe Workfront物件上發生動作時，您可以設定Workfront將回應傳送至您所需的端點。 這表示協力廠商應用程式在更新發生後不久就能透過Workfront API接收來自Workfront互動的更新。 一般而言，您可能會在5秒內收到記錄資料變更的webhook通知。 平均而言，客戶會在記錄資料變更後1秒內收到webhook通知。  

若要透過防火牆接收事件訂閱裝載，您必須將下列IP位址新增至允許清單：

**歐洲客戶：**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**對於位於歐洲以外地點的客戶：**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

下列主題支援事件訂閱API：

## 事件訂閱支援的物件

事件訂閱支援下列Workfront物件。

* 指派
* 公司
* 儀表板
* 文件
* 費用
* 欄位
* 小時
* 問題
* 備註
* 專案組合
* 方案
* 專案
* 記錄
* 記錄類型
* 報告
* 任務
* 範本
* 時程表
* 使用者

如需事件訂閱物件支援的欄位清單，請參閱 [事件訂閱資源欄位](../../wf-api/api/event-sub-resource-fields.md).

## 事件訂閱驗證

若要建立、查詢或刪除事件訂閱，您的Workfront使用者需要下列專案：

* 需要「系統管理員」的存取層級才能使用事件訂閱。
* A `sessionID`  標題為必填欄位，才能使用事件訂閱API

  如需詳細資訊，請參閱 [驗證](api-basics.md#authentication) 在 [API基本需知](api-basics.md).

## 形成訂閱資源

訂閱資源包含下列欄位。

* 物件ID （選擇性）

   * **字串**  — 為其引發事件的指定物件程式碼的物件識別碼。 如果未指定此欄位，使用者會收到指定型別之所有物件的事件。

* 物件代碼（必要）

   * **字串**  — 訂閱變更的物件物件代碼。 objCode的可能值列於下表。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>物件</p></th> 
        <th><p>物件代碼</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">指派</td> 
        <td scope="col"><p>指派</p></td> 
       </tr> 
       <tr> 
        <td scope="col">公司 </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">儀表板</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>文件</p></td> 
        <td scope="col">檔案 </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>費用</p></td> 
        <td scope="col">費用</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>欄位</p></td> 
        <td scope="col"><p>欄位</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>小時</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">問題</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">備註</td> 
        <td scope="col">附註</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>專案組合</p></td> 
        <td scope="col"><p>連線埠</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>方案</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>專案</p></td> 
        <td scope="col"><p>專案</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>記錄</p></td> 
        <td scope="col"><p>記錄</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>記錄類型</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>報告</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>任務</p></td> 
        <td scope="col"><p>任務</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>範本</p></td> 
        <td scope="col"><p>範本</p></td> 
       </tr> 
       <tr> 
        <td scope="col">時程表</td> 
        <td scope="col">表格</td> 
       </tr> 
       <tr> 
        <td scope="col">使用者</td> 
        <td scope="col">使用者</td> 
       </tr> 
      </tbody> 
     </table>

* eventType （必要）

   * **字串**  — 代表物件訂閱的事件型別的值。 可用的事件型別包括：

      * 建立
      * DELETE 
      * 更新

* url （必要）

   * **字串**  — 透過HTTP傳送訂閱事件裝載的端點URL。

* authToken （必要）

   * **字串**  — 用於使用「URL」欄位中指定的URL進行驗證的OAuth2持有人權杖。 

## 建立事件訂閱API請求

在確保使用者具有管理員存取權並形成訂閱資源後，您就可以建立事件訂閱了。

請使用下列語法來建構URL。

**請求URL：**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**請求標頭：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>頁首名稱</p> </th> 
   <th> <p>標頭值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID值</p> </td> 
  </tr> 
 </tbody> 
</table>

**要求內文範例：**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| 回應代碼 | 說明 |
|---|---|
| 201 （已建立） | 已成功建立事件訂閱。 |
| 400 （錯誤請求） | 訂閱資源的URL欄位被視為無效。 |
| 401 （未獲授權） | 提供的sessionID是空的或被視為無效。 |
| 403 （禁止存取） | 符合所提供sessionID的使用者沒有管理員存取權。 |

以要求內文傳遞訂閱資源（內容型別是&quot;application/json&quot;）會導致系統針對指定的物件建立事件訂閱。 回應代碼201 （已建立）表示已建立訂閱。 201以外的回應代碼表示訂閱為 **NOT** 已建立。

>[!NOTE]
>
> 「Location」回應標頭包含新建立之事件訂閱的URI。

**回應標頭範例：**

| 回應標頭 | 範例 |
|---|---|
| Content-Length | `→0` |
| 日期 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| 位置 | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| 伺服器 | `→Apache-Coyote/1.1` |

## 查詢事件訂閱

查詢Workfront的HTTP時，請使用GET方法。 查詢事件訂閱有兩種方式：依訂閱ID查詢（請參閱下文）或查詢所有事件訂閱。

### 查詢所有事件訂閱

您可以查詢客戶的所有事件訂閱，或使用下列專案來管理回應。 您也可以使用下列選項來管理回應：

* **頁面**：查詢引數選項，用於指定要傳回的頁數。 預設值為1。
* **limit**：查詢引數選項，用於指定每頁傳回的結果數。 預設值為100，最大值為1000。

列出特定客戶之所有事件訂閱的請求語法如下：

**請求URL：**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**請求標頭：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>頁首名稱</p> </th> 
   <th> <p>標頭值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID值</p> </td> 
  </tr> 
 </tbody> 
</table>

**回應代碼：**

| 回應代碼 | 說明 |
|---|---|
| 200 （確定） | 針對符合所提供sessionID的客戶，所傳回的請求包含所有找到的事件訂閱。 |
| 401 （未獲授權） | 提供的sessionID是空的。 |
| 403 （禁止存取） | 符合所提供sessionID的使用者沒有管理員存取權。 |


**回應標頭範例：**

| 回應標頭 | 範例 |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| 日期 | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| 伺服器 | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**回應本文範例：**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

位置

* **頁面** 和 **limit** 是請求中提供的值，如果未提供值，則為預設值
* **page_count** 是可查詢的頁面總數。
* **total_count** 是符合查詢的訂閱總數。

### 依事件訂閱ID查詢

您可以依事件訂閱ID來查詢事件訂閱。 列出事件訂閱的請求語法如下：

**請求URL：**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**請求標頭：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>頁首名稱</p> </th> 
   <th> <p>標頭值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID值</p> </td> 
  </tr> 
 </tbody> 
</table>

**回應代碼：**

| 回應代碼 | 說明 |
|---|---|
| 200 （確定） | 請求傳回的事件訂閱與提供的訂閱ID相符。 |
| 401 （未獲授權） | 提供的sessionID是空的。 |
| 403 （禁止存取） | 符合所提供sessionID的使用者沒有管理員存取權。 |


**回應本文範例：**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## 事件訂閱篩選

事件訂閱篩選可用於確保您僅接收相關訊息。 為您的訂閱建立篩選器可能會大幅減少端點需要使用的訊息數量。

例如， **更新 — 任務** 事件訂閱只能設定為以下情況觸發： **newState** 事件有效負載的 **任務狀態** 作為 **目前**.

>[!IMPORTANT]
>
下列屬性適用於事件訂閱篩選

* 當篩選欄位具有非空白值時，只會訊息具有 **newState** 包含篩選鍵和值，以傳送至訂閱的URL
* 您可以依據包含在 **newState** 和/或 **oldState**&#x200B;物件的
* 篩選器僅會根據其是否等於特定值進行評估
* 如果您的篩選器語法不正確或不符合 **newState** 在承載中，將不會傳回驗證訊息來指示已發生錯誤
* 無法在現有的訂閱上更新篩選器；必須使用新的篩選器引數建立新的訂閱。
* 多個篩選器可套用至單一訂閱，且只有當滿足所有篩選器條件時，才會傳送訂閱。
* 將多個篩選器套用至單一訂閱，其實務等於使用 **和** 邏輯運運算元。
* 只要每個事件訂閱之間有一或多個事件訂閱欄位引數不同，就可以將多個事件訂閱套用至單一物件。
* 將多個事件訂閱指派給單一物件時，與該物件相關聯的所有事件訂閱都可以傳回至單一端點。 此作法可以當做邏輯運運算元的對等替代使用 **或** 無法使用篩選引數來設定。

### 使用比較運運算元

您可以指定比較欄位以及篩選欄位。 在此至欄位中使用比較運運算元，以篩選比較結果。 例如，您可以建立UPDATE - TASK訂閱，僅在任務狀態不等於current時傳送裝載。 您可以使用下列比較運運算元：

#### eq： equal

如果發生的變更相符，此篩選器可允許傳遞訊息 `fieldValue` 在篩選器中完全符合。 此 `fieldValue` 值區分大小寫。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne：不等於

如果發生的變更不符，此篩選器可允許傳遞訊息 `fieldValue` 在篩選器中完全符合。 此 `fieldValue` 值區分大小寫。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt：大於

如果指定的更新，此篩選器可允許訊息通過 `fieldName` 大於的值 `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte：大於或等於

如果指定的更新，此篩選器可允許訊息通過 `fieldName` 大於或等於 `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt：小於

如果指定的更新，此篩選器可允許訊息通過 `fieldName` 小於 `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte：小於或等於

如果指定的更新，此篩選器可允許訊息通過 `fieldName` 小於或等於 `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### 包含

如果發生的變更包含 `fieldValue` 在篩選中。 此 `fieldValue` 值區分大小寫

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### 變更

此篩選器只允許指定欄位(`fieldName`)在oldstate和newstate中有不同的值。 更新指定欄位以外的其他欄位(`fieldName`)將不會傳回該變更。

>[!NOTE]
>
`fieldValue` 在以下的濾鏡陣列中沒有任何效果。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

此聯結器將篩選套用到已建立或更新之物件的新狀態或舊狀態。 當您想知道某個專案在哪裡變更到另一個專案時，這會很有幫助。
`oldState` 無法在CREATE上執行 `eventTypes`.

>[!NOTE]
>
底下具有指定篩選器的訂閱只會傳回工作名稱包含的訊息 `again` 於 `oldState`，即更新任務之前的狀態。
此情況下的使用案例是尋找從一個事物變更為另一個事物的objCode訊息。 例如，找出從「Research Some name」變更為「Research TeamName Some name」的所有任務

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### 使用聯結器欄位

此 `filterConnector` 訂閱裝載上的欄位可讓您選擇應如何套用篩選器。 預設值為「AND」，其中所有篩選器必須為 `true` 讓訂閱訊息顯示。 若指定「OR」，則只有一個篩選器必須符合訂閱訊息才能通過。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## 刪除事件訂閱

刪除Workfront的HTTP時，請使用DELETE方法。 依訂閱ID刪除單一事件訂閱的請求語法如下：

**請求URL：**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**請求標頭：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>頁首名稱</p> </th> 
   <th> <p>標頭值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID值 </p> </td> 
  </tr> 
 </tbody> 
</table>

**回應代碼：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>回應代碼</p> </th> 
   <th> 說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 （無內容）</td> 
   <td>伺服器已成功移除符合所提供subscriptionID的事件訂閱。</td> 
  </tr> 
  <tr> 
   <td>401 （未獲授權）</td> 
   <td>提供的sessionID是空的。</td> 
  </tr> 
  <tr> 
   <td>403 （禁止存取）</td> 
   <td>符合所提供sessionID的使用者沒有管理員存取權。</td> 
  </tr> 
  <tr> 
   <td>404 （找不到）</td> 
   <td>伺服器找不到符合提供刪除之subscriptionID的事件訂閱。</td> 
  </tr> 
 </tbody> 
</table>

**回應標頭範例：**

| 回應標頭 | 範例 |
|---|---|
| 日期 | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| 伺服器 | `→Apache-Coyote/1.1` |


**回應本文範例：** 不適用

## 事件裝載範例

使用者收到的有效負載會依物件型別而異，但有一致性的格式，可用於傳送這些不同的有效負載。

例如，下列屬性在所有事件裝載中維持一致：

* eventtype
* subscriptionId
* oldState
* newState
* eventTime

雖然格式一致，但屬性中包含的值在不同的物件與物件型別之間有所不同。

以下顯示UPDATE事件和CREATE事件的裝載範例。 請注意，在UPDATE範例中，oldState物件與newState物件相同，而在CREATE範例中，oldState物件是空的（不是NULL）。

以下是UPDATE事件的裝載範例：

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

以下是CREATE事件的裝載範例：

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Base 64編碼

如果事件訂閱因為事件訂閱中包含的特殊字元與網路設定之間的衝突而被拒絕，則您可以使用Base64編碼來傳遞事件訂閱。 Base64是一組編碼配置，可將任何任意資料轉換為ASCII字串格式。 請務必注意，Base64並非一種安全性加密形式。

### Base 64編碼欄位

base64Encoding欄位是選用欄位，用來啟用事件訂閱裝載的Base64編碼。 預設值為false，可能的值為： true、false和「 」 （空白）。

### 使用base64Encoding欄位的要求範例

如果使用設為true的base64Encoding欄位提出要求，則 **newState** 和 **oldState** 承載中的物件會以base 64編碼字串形式傳送。 如果base64Encoding欄位設為false、保留空白或未包含於請求中，則傳回的裝載將不會以base 64編碼。

以下是使用base64Encoding欄位的要求範例：

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### 基底64編碼中的回應裝載範例

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## 查詢所有事件訂閱的方法已過時

下列API端點已過時，不應該用於新的實作。 我們也建議將舊的實作轉換成 **查詢事件訂閱** 一節中說明。

您可以查詢sessionID值所指定的客戶的所有事件訂閱。 列出特定客戶之所有事件訂閱的請求語法如下URL：

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**請求標頭：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>頁首名稱</p> </th> 
   <th> <p>標頭值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID值 </p> </td> 
  </tr> 
 </tbody> 
</table>

**回應代碼：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>回應代碼</p> </th> 
   <th> 說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 （無內容）</td> 
   <td>該請求已成功傳回為使用者找到的所有事件訂閱。</td> 
  </tr> 
  <tr> 
   <td>401 （未獲授權）</td> 
   <td>提供的sessionID是空的。</td> 
  </tr> 
  <tr> 
   <td>403 （禁止存取）</td> 
   <td>符合所提供sessionID的使用者沒有管理員存取權。</td> 
  </tr> 
 </tbody> 
</table>

 

### 回應本文範例

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
