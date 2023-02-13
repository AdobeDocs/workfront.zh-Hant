---
content-type: api
navigation-topic: general-api
title: 事件訂閱API
description: 事件訂閱API
author: John
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c52f1839d3d00c71c6d567084dafd586d161d8fb
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 3%

---


# 事件訂閱API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

當事件訂閱支援的Adobe Workfront物件上發生動作時，您可以設定Workfront以傳送回應至您想要的端點。 這表示協力廠商應用程式在Workfront互動發生後，就可透過Workfront API立即接收更新。 一般而言，您可能會在記錄資料變更後不到5秒內收到Webhook通知。 客戶平均會在1秒內收到來自記錄中資料變更的網頁連結通知。  

若要透過防火牆接收事件訂閱裝載，您必須將下列IP位址新增至允許清單：

**歐洲客戶：**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**歐洲以外地區的客戶：**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

下列主題支援事件訂閱API:

## 事件訂閱支援的對象

事件訂閱支援下列Workfront物件。

* 指派
* 公司
* 儀表板
* 文件
* 費用
* 時數
* 問題
* 備註
* 專案組合
* 方案
* 專案
* 報告
* 任務
* 範本
* 時程表
* 使用者

有關事件訂閱對象支援的欄位清單，請參見 [事件訂閱資源欄位](../../wf-api/api/event-sub-resource-fields.md).

## 事件訂閱驗證

若要建立、查詢或刪除事件訂閱，您的Workfront使用者需要：

* 「系統管理員」的訪問級別
* apiKey

   >[!NOTE]
   >
   >如果您的使用者已使用Workfront的API，則您的使用者應已擁有apiKey。 您可以透過下列HTTP要求擷取apiKey:

**請求URL:**

```
PUT https://<HOSTNAME>/attask/api/v7.0/USER?action=getApiKey&username=<USERNAME>&password=<PASSWORD>
```

**請求標題：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>標題名稱</p> </th> 
   <th> <p>標題值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>內容類型</p> </td> 
   <td> <p>文字/html</p> </td> 
  </tr> 
 </tbody> 
</table>

**回應代碼：**

| 回應代碼 | 說明 |
|---|---|
| 200（確定） | 已成功處理請求，應在回應內文中傳回使用者的現有apiKey。 |
| 401（未授權） | 伺服器確認請求，但無法處理，因為請求的apiKey/使用者沒有提出此請求的存取權。 |

{style=&quot;table-layout:auto&quot;}

**回應內文範例：**

```
{
               "data"{
               "result": "rekxqndrw9783j4v79yhdsakl56bu1jn"
               }
      }
```

>[!NOTE]
>
> 如果您是第一次使用Workfront API，則需要產生apiKey，您可以透過此連結進行：


```
PUT https://<HOSTNAME>/attask/api/v7.0/USER/generateApiKey?username=<USERNAME>&password=<PASSWORD>
```

## 形成訂閱資源

訂閱資源包含下列欄位。

* objId（選用）

   * **字串**  — 為其引發事件的指定objCode物件的ID。 如果未指定此欄位，則用戶將接收指定類型的所有對象的事件。

* objCode（必要）

   * **字串**  — 訂閱變更之物件的objCode。 objCode的可能值列於下表。

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>物件</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">指派</td> 
        <td scope="col"><p>ASSGN</p></td> 
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
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>費用</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>時數</p></td> 
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
        <td scope="col"><p>埠</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>方案</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>專案</p></td> 
        <td scope="col"><p>PROJ</p></td> 
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
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">時程表</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">使用者</td> 
        <td scope="col">使用者</td> 
       </tr> 
      </tbody> 
     </table>

* eventType（必要）

   * **字串**  — 代表物件所訂閱之事件類型的值。 可用的事件類型包括：

      * 建立
      * DELETE 
      * 更新

* url（必要）

   * **字串**  — 透過HTTP傳送訂閱事件裝載的端點URL。

* authToken（必要）

   * **字串** - OAuth2承載權杖，用於使用「URL」欄位中指定的URL進行驗證。 

## 建立事件訂閱API請求

在確保使用者擁有管理員存取權並形成訂閱資源後，您就可以建立事件訂閱。

使用下列語法來建構URL。

**請求URL:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**請求標題：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>標題名稱</p> </th> 
   <th> <p>標題值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>內容類型</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>授權</p> </td> 
   <td> <p>apiKey值</p> </td> 
  </tr> 
 </tbody> 
</table>

**請求內文範例：**

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
| 201（已建立） | 已成功建立事件訂閱。 |
| 400(Bad Request) | 訂閱資源的URL欄位被視為無效。 |
| 401（未授權） | 提供的apiKey為空或被視為無效。 |
| 403（禁止） | 與提供的apiKey相符的使用者沒有管理員存取權。 |

將訂閱資源傳遞為要求內文（內容類型為「application/json」），會導致針對指定的物件建立事件訂閱。 回應代碼201（已建立）表示已建立訂閱。 201以外的回應代碼表示訂閱為 **NOT** 已建立。

>[!NOTE]
 「位置」響應標題包含新建立的事件訂閱的URI。

**回應標題範例：**

| 回應標題 | 範例 |
|---|---|
| Content-Length | `→0` |
| 日期 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| 位置 | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| 伺服器 | `→Apache-Coyote/1.1` |

## 查詢事件訂閱

查詢Workfront的HTTP時，請使用GET方法。 有兩種方式可查詢事件訂閱：依訂閱ID進行查詢（請參閱下文）或查詢所有事件訂閱。

### 查詢所有事件訂閱

您可以按照apiKey值的指定，查詢客戶的所有事件訂閱。 您也可以使用下列選項來管理回應：

* **頁面**:查詢參數選項，以指定要傳回的頁數。 預設為1。
* **限制**:查詢參數選項，以指定每頁要傳回的結果數。 預設值為100，最大值為1000。

列出特定客戶之所有事件訂閱的要求語法如下：

**請求URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**請求標題：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>標題名稱</p> </th> 
   <th> <p>標題值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授權</p> </td> 
   <td> <p>apiKey值</p> </td> 
  </tr> 
 </tbody> 
</table>

**回應代碼：**

| 回應代碼 | 說明 |
|---|---|
| 200（確定） | 傳回的請求包含針對符合所提供apiKey之客戶的所有事件訂閱。 |
| 401（未授權） | 提供的apiKey為空。 |
| 403（禁止） | 與提供的apiKey相符的使用者沒有管理員存取權。 |


**回應標題範例：**

| 回應標題 | 範例 |
|---|---|
| 內容類型 | `→application/json;charset=UTF-8` |
| 日期 | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| 伺服器 | `→Apache-Coyote/1.1` |
| 傳輸編碼 | `→chunked` |


**回應內文範例：**

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

* **頁面** 和 **限制** 是請求中提供的值，如果未提供值，則為預設值
* **page_count** 是可查詢的總頁數。
* **total_count** 是符合查詢的訂閱總數。

### 按事件訂閱ID查詢

您可以依事件訂閱的ID來查詢事件訂閱。 列出事件訂閱的要求語法如下：

**請求URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**請求標題：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>標題名稱</p> </th> 
   <th> <p>標題值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授權</p> </td> 
   <td> <p>apiKey值</p> </td> 
  </tr> 
 </tbody> 
</table>

**回應代碼：**

| 回應代碼 | 說明 |
|---|---|
| 200（確定） | 傳回的請求與提供的訂閱ID相符的事件訂閱。 |
| 401（未授權） | 提供的apiKey為空。 |
| 403（禁止） | 與提供的apiKey相符的使用者沒有管理員存取權。 |


**回應內文範例：**

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

事件訂閱篩選可用來確保您只收到相關訊息。 為訂閱建立篩選器可能會大幅減少端點需要使用的訊息數量。

例如， **更新 — 任務** 事件訂閱只能在 **newState** 事件有效負載的定義 **taskStatus** as **電流**.

>[!IMPORTANT]
以下屬性適用於事件訂閱篩選

* 當篩選欄位具有非空白值時，只會傳送 **newState** 包含篩選索引鍵和值會傳送至訂閱的URL
* 您可以依據包含在 **newState** 和/或 **oldState**&#x200B;對象
* 系統只會根據篩選條件是否等於特定值來評估篩選條件
* 如果您的篩選語法不正確或不符合 **newState** 裝載時，將不會傳回驗證訊息，以指出發生錯誤
* 無法針對目前存在的訂閱更新篩選器；必須使用新的篩選參數建立新訂閱。
* 多個篩選器可套用至單一訂閱，且只有在符合所有篩選條件時才會傳送訂閱。
* 將多個篩選器套用至單一訂閱，這等同於使用 **和** 邏輯運算子。
* 只要一個或多個事件訂閱欄位參數在每個事件訂閱之間不同，就可以將多個事件訂閱套用至單一物件。
* 將多個事件訂閱指派給單個對象時，與該對象關聯的所有事件訂閱都可以返回到單個終結點。 此作法可作為邏輯運算子的等效替代 **或** 無法使用篩選參數來設定。

### 使用比較運算子

您可以指定比較欄位與篩選欄位。 在此對欄位中使用比較運算子，以篩選比較結果。 例如，您可以建立UPDATE - TASK訂閱，該訂閱僅在任務狀態不等於當前時發送裝載。 您可以使用下列比較運算子：

#### eq:等於

如果發生的變更符合，此篩選器可讓訊息傳遞 `fieldValue` 填入。 此 `fieldValue` 值區分大小寫。

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

#### 一：不等於

如果發生的變更不符合，此篩選器可讓訊息傳遞 `fieldValue` 填入。 此 `fieldValue` 值區分大小寫。

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

#### gt:大於

如果指定的 `fieldName` 大於的值 `fieldValue`.

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

#### get:大於或等於

如果指定的 `fieldName` 大於或等於 `fieldValue`.

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

#### lt:小於

如果指定的 `fieldName` 小於的值 `fieldValue`.

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

#### lte:小於或等於

如果指定的 `fieldName` 小於或等於 `fieldValue`.

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

如果發生的變更包含 `fieldValue` 中。 此 `fieldValue` 值區分大小寫

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

此篩選器僅允許在指定欄位(`fieldName`)在oldstate和newstate中有不同的值。 更新指定欄位以外的其他欄位(`fieldName`)不會傳回該變更。

>[!NOTE]
`fieldValue` 在下方的「篩選器」陣列中沒有作用。

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

此連接器使過濾器應用於已建立或更新的對象的新狀態或舊狀態。 如果您想要了解從某個項目變更為另一個項目的位置，此功能會很好用。
`oldState` 在CREATE上不可能 `eventTypes`.

>[!NOTE]
以下具有指定篩選器的訂閱只會傳回任務名稱包含的訊息 `again` 在 `oldState`，在對任務進行更新之前的情況。
其使用案例是尋找從一個項目變更為另一個項目的objCode訊息。 例如，查找從「Research Some name」更改為「Research TeamName Some name」的所有任務

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

### 使用連接器欄位

此 `filterConnector` 訂閱裝載上的欄位可讓您選擇應如何套用篩選器。 預設值為「AND」，其中篩選器必須全部為 `true` 讓訂閱訊息傳入。 如果指定&quot;OR&quot;，則只有一個篩選器必須符合，訂閱訊息才能通過。

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

刪除Workfront的HTTP時，請使用DELETE方法。 依訂閱ID刪除單一事件訂閱的要求語法如下：

**請求URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**請求標題：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>標題名稱</p> </th> 
   <th> <p>標題值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授權</p> </td> 
   <td> <p> 使用者的apiKey </p> </td> 
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
   <td>200（無內容）</td> 
   <td>伺服器已成功刪除與提供的subscriptionID匹配的事件訂閱。</td> 
  </tr> 
  <tr> 
   <td>401（未授權）</td> 
   <td>提供的apiKey為空。</td> 
  </tr> 
  <tr> 
   <td>403（禁止）</td> 
   <td>符合所提供apiKey的使用者沒有管理員存取權。</td> 
  </tr> 
  <tr> 
   <td>404（找不到）</td> 
   <td>伺服器找不到與提供用於刪除的subscriptionID匹配的事件訂閱。</td> 
  </tr> 
 </tbody> 
</table>

**回應標題範例：**

| 回應標題 | 範例 |
|---|---|
| 日期 | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| 伺服器 | `→Apache-Coyote/1.1` |


**回應內文範例：** 不適用

## 事件裝載範例

用戶接收的有效負載根據對象類型而有所不同，但有一種一致的格式，用於傳送這些不同的有效負載。

例如，下列屬性在所有事件裝載中保持一致：

* eventType
* subscriptionId
* oldState
* newState
* eventTime

雖然格式一致，但屬性中包含的值在不同對象和對象類型之間有所不同。

UPDATE事件和CREATE事件的裝載範例如下所示。 請注意，在UPDATE示例中， oldState和newState對象是相同的，而在CREATE示例中， oldState對象是空的（非NULL）。

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

## 基64編碼

如果由於事件訂閱中包含的特殊字元與網路設定之間的衝突而拒絕事件訂閱，則可以使用Base64編碼來傳遞事件訂閱。 Base64是一組編碼方案，可將任意資料轉換為ASCII字串格式。 請務必注意，Base64不是一種安全加密形式。

### 基礎64編碼欄位

base64Encoding欄位是可選欄位，用於啟用事件訂閱負載的Base64編碼。 預設值為false，可能的值為：true、false和&quot; &quot;（空白）。

### 使用base64Encoding欄位的請求範例

如果使用base64Encoding欄位設為true來提出要求，則 **newState** 和 **oldState** 有效負載中的物件會以基本64編碼字串的形式傳送。 如果base64Encoding欄位設為false、保留為空白或未包含在請求中，則傳回的裝載將不會在base64中編碼。

以下是使用base64Encoding欄位之請求的範例：

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

### 基礎64編碼中的回應裝載範例

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

## 已廢止的查詢所有事件訂閱的方法

下列API端點已遭取代，不應用於新實作。 我們也建議將舊實作轉換為 **查詢事件訂閱** 一節。

您可以按照apiKey值的指定，查詢客戶的所有事件訂閱。 列出特定客戶之所有事件訂閱的請求語法如下：

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**請求標題：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>標題名稱</p> </th> 
   <th> <p>標題值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授權</p> </td> 
   <td> <p> 使用者的apiKey </p> </td> 
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
   <td>200（無內容）</td> 
   <td>請求已成功返回為用戶找到的所有事件訂閱。</td> 
  </tr> 
  <tr> 
   <td>401（未授權）</td> 
   <td>提供的apiKey為空。</td> 
  </tr> 
  <tr> 
   <td>403（禁止）</td> 
   <td>符合所提供apiKey的使用者沒有管理員存取權。</td> 
  </tr> 
 </tbody> 
</table>

 

### 回應內文範例

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
