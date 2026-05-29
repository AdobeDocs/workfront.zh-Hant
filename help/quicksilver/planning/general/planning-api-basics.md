---
title: Adobe Workfront規劃API基本需知
description: Adobe Workfront Planning API的目標是引入透過HTTP運作的REST-ful架構，簡化與Planning的整合建置。 本檔案假設您熟悉REST和JSON回應，並說明Planning API所採取的方法。
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: a9f14c6726bcec0cc9b040dde9b6bf90a5868edc
workflow-type: tm+mt
source-wordcount: '2232'
ht-degree: 2%

---


# Adobe Workfront Planning API基本需知

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

Adobe Workfront Planning API的目標是引入透過HTTP運作的RESTful架構，簡化與Planning的整合建置。 本檔案假設您熟悉REST和JSON回應。

如需完整的端點參考、要求/回應結構描述和版本特定詳細資訊，請參閱[Workfront Planning API開發人員檔案](https://developer.adobe.com/wf-planning)。

## Authentication

Workfront Planning API使用OAuth 2.0進行驗證。 認證是透過Adobe Developer Console設定的。

根據您的整合型別，我們支援下列兩個流程：

* **伺服器對伺服器驗證(JWT)**：針對沒有使用者互動的自動整合與後端服務。 使用OAuth伺服器對伺服器認證（使用者端認證授予 — 您的應用程式會使用其使用者端ID和密碼直接驗證，以取得存取權杖，無需使用者登入或同意步驟）。

  如需詳細資訊，請參閱[伺服器對伺服器驗證](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/)。

* **使用者驗證（授權碼流程）**：代表特定使用者執行整合作業。 使用OAuth網頁應用程式或單頁應用程式認證（授權代碼授予 — 使用者登入並同意，之後您的應用程式會收到授權代碼，然後交換存取權杖）。

  如需詳細資訊，請參閱[使用者驗證](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/)。

若要開始使用，請在Adobe Developer Console中建立專案，並新增Workfront Planning API以取得您的認證。

若要設定認證，請在Workfront中建立OAuth2應用程式。

如需詳細資訊，請參閱[為Workfront整合建立OAuth2應用程式](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)。

>[!NOTE]
>
>Workfront Planning不支援`/login`端點和API金鑰驗證。 請勿使用`sessionID`或`apiKey`引數。


## API版本設定

Planning API是透過URL路徑建立版本。

以下是目前支援的版本：

<!--

(*****************add deprecation date column above, when we have one*****************)

-->

| 版本 | 發行日期 |
|-----------|----------------|
| 第1版 | 2024 年 7 月 |
| 第2版 | 2026年5月 |

>[!NOTE]
>
>適用於Workfront Fusion的Workfront Planning聯結器尚未更新為API版本2，在進一步通知之前，它將繼續使用版本1。

如需目前支援版本的詳細資訊，請參閱文章[Workfront Planning API開發人員檔案](https://developer.adobe.com/wf-planning)。

我們建議在所有整合中明確鎖定版本：

```
https://{customer-domain}/maestro/api/v2/...
```

發行新的主要版本時，在傳達淘汰日期之前，將繼續提供舊版。

請依照Workfront發行說明操作，及時瞭解API變更。


## URL結構和操作

透過傳送HTTP請求至物件的唯一URI來控制物件。 操作由HTTP方法指定。

| 方法 | 作業 |
|----------|----------------------------------------------------------------------|
| GET | 依ID擷取單一物件，或搜尋/列出物件 |
| 張貼 | 建立新物件 |
| PUT | 取代現有物件（完整更新） |
| PATCH | 部分更新現有物件（僅修改提供的欄位） |
| DELETE | 刪除物件 |

>[!NOTE]
>
>**版本1不支援** `PATCH`。 使用`PUT`進行所有更新。


如需完整的端點路徑和要求/回應範例，請參閱[developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)上的&#x200B;**API參考**。

## HTTP狀態碼

Planning API會傳回標準HTTP狀態代碼：

| 程式碼 | 含義 |
|------------------------|-------------------------------------------------|
| 200 OK | 成功的GET、PUT或PATCH |
| 201已建立 | 成功發佈（已建立資源） |
| 204無內容 | 成功的DELETE |
| 207多重狀態 | 大量作業已完成，但結果有好有壞，有些專案成功，有些專案失敗。 如需詳細資訊，請檢視個別專案回應。 |
| 400錯誤請求 | 無效的請求 — 如需詳細資料，請參閱錯誤回應 |
| 401未獲授權 | 缺少驗證權杖或驗證權杖無效 |
| 403禁止 | 已驗證但許可權不足 |
| 404找不到 | 資源不存在 |
| 409衝突 | 寫入衝突，資源已由另一個請求修改。 請使用最新版本重試。 |
| 429太多請求 | 超出速率限制 |

>[!NOTE]
>
>**第1版備註：**&#x200B;第1版為所有成功的作業（包括POST和DELETE）傳回`200 OK`。


## 錯誤處理

Planning API會以一致的格式傳回錯誤。 每個錯誤回應都包含可讀取的訊息、機器可讀取的錯誤代碼以及支援升級的請求ID。

範例錯誤回應：

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

使用`errorCode` （非`status`）來驅動程式化錯誤處理。 它提供最具體的失敗分類。

>[!NOTE]
>
>**第1版備註：**&#x200B;第1版錯誤回應使用數值`type`欄位（例如`40001`）而非字串`errorCode`，並將詳細資料包裝在`report`物件而非最上層`detail`欄位中。

## 篩選記錄

在記錄搜尋要求中使用`filter`引數，僅傳回符合特定條件的記錄。 對於POST要求，`filter`是要求內文中的JSON屬性。 對於GET要求，`filter`是包含JSON編碼篩選群組的查詢引數。 篩選器使用具有明確邏輯運運算元的型別化複合結構。

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

篩選器可以使用`AND` / `OR`運運算元巢狀化以建置複合條件：

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**第1版備註：**&#x200B;第1版在`filters`物件中使用Mongo樣式無型別運運算元。 運運算元以`$`為前置詞（例如`$and`、`$or`、`$is`、`$contains`、`$isBetween`）。 分頁引數(`offset`、`limit`)和`recordTypeId`是在要求內文中傳遞，而非作為URL路徑和查詢引數。


## 欄位型別和搜尋修飾詞

您可以使用包含欄位的修飾詞和篩選器來控制要在結果中傳回哪些資料。

如需範例，請參閱[Workfront Planning API開發人員檔案](https://developer.adobe.com/wf-planning/)。

### 使用搜尋修飾元

Workfront Planning支援下列搜尋修飾元：


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>修飾詞</th>
      <th>範例</th>
      <th>說明</th>
      <th>可能的值</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："CONTAINS"，"value"："product"}</td><td>傳回其欄位值包含篩選器的記錄</td><td class="possible">"新產品上市"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："DOES_NOT_CONTAIN"，"value"："product"}</td><td>傳回欄位值不含篩選器的記錄</td><td class="possible">"新增啟動項"</td></tr>
    <tr><td class="modifier">是</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS"，"value"："new product launch"}</td><td>傳回其欄位值完全符合篩選器的記錄</td><td class="possible">"新產品上市"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NOT"，"value"："product"}</td><td>傳回欄位值不完全符合篩選器的記錄</td><td class="possible">"新產品上市"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_EMPTY"}</td><td>傳回欄位值空白的記錄</td><td class="possible">「」或null</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NOT_EMPTY"}</td><td>傳回欄位值非空白的記錄</td><td class="possible">"新產品上市"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："GREATER_THAN"，"value"："10"}</td><td>傳回欄位值大於篩選器的記錄</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："GREATER_THAN_OR_EQUAL"，"value"："10"}</td><td>傳回欄位值大於或等於篩選器的記錄</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："LESS_THAN"，"value"："10"}</td><td>傳回欄位值小於篩選器的記錄</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："LESS_THAN_OR_EQUAL"，"value"："10"}</td><td>傳回欄位值小於或等於篩選器的記錄</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_BETWEEN"，"value"：["2024-01-01"，"2024-12-31"]}</td><td>傳回欄位值介於兩個篩選值之間的記錄</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NOT_BETWEEN"，"value"：["2024-01-01"，"2024-12-31"]}</td><td>傳回欄位值未介於兩個篩選值之間的記錄</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_AFTER"，"value"："2024-01-01"}</td><td>傳回日期欄位值在篩選器之後的記錄</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_BEFORE"，"value"："2024-12-31"}</td><td>傳回日期欄位值在篩選器之前的記錄</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_ANY_OF"，"value"：["Active"，"Planned"]}</td><td>傳回其欄位值符合篩選器清單中任何值的記錄</td><td class="possible">["Active"，"Planned"，"Complete"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NONE_OF"，"value"：["Active"，"Planned"]}</td><td>傳回欄位值不符合篩選器清單中所有值的記錄</td><td class="possible">[「作用中」，「計畫」]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："HAS_ANY_OF"，"value"：["Tag1"，"Tag2"]}</td><td>傳回多值欄位包含任何篩選值的記錄</td><td class="possible">["Tag1"，"Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："HAS_ALL_OF"，"value"：["Tag1"，"Tag2"]}</td><td>傳回多值欄位包含所有篩選值的記錄</td><td class="possible">["Tag1"，"Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_EXACTLY"，"value"：["Tag1"]}</td><td>傳回其多值欄位只包含篩選值而不包含其他值的記錄</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："HAS_NONE_OF"，"value"：["Tag1"]}</td><td>傳回多值欄位不含任何篩選值的記錄</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>版本1備註： V1修飾詞名稱使用`$-prefixed camelCase` （例如`$contains`、`$isNot`、`$isEmpty`、`$greaterThan`、`$greaterThanOrEqual`、`$lessThan`、`$lessThanOrEqual`、`$isBetween`、`$isNotBetween`、`$isAnyOf`、`$hasAllOf`）。 每個修飾元的行為都相同。


## 依欄位型別支援的篩選條件

| 欄位型別 | 支援的條件 |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| 文字，長文字 | 包含、DOES_NOT_CONTAIN、IS、IS_NOT、IS_EMPTY、IS_NOT_EMPTY |
| 數字，百分比，貨幣 | IS、IS_NOT、GREATER_THAN、GREATER_THAN_OR_EQUAL、LESS_THAN_OR_EQUAL、IS_EMPTY、IS_NOT_EMPTY |
| 日期 | IS、IS_NOT、IS_AFTER、IS_BEFORE、IS_BETWEEN、IS_NOT_BETWEEN、IS_EMPTY、IS_NOT_EMPTY |
| 單選 | IS、IS_NOT、IS_ANY_OF、IS_NONE_OF、IS_EMPTY、IS_NOT_EMPTY |
| 多選，使用者 | HAS_ANY_OF， HAS_ALL_OF， IS_EXACTLY， HAS_NONE_OF， IS_EMPTY， IS_NOT_EMPTY |
| 布林值 | 是 |
| 公式 | 包含、DOES_NOT_CONTAIN、IS、IS_NOT、IS_EMPTY、IS_NOT_EMPTY |
| 建立者 | IS、IS_NOT、IS_ANY_OF、IS_NONE_OF |
| 更新者 | IS、IS_NOT、IS_ANY_OF、IS_NONE_OF、IS_EMPTY、IS_NOT_EMPTY |
| 建立時間 | IS、IS_NOT、IS_AFTER、IS_BEFORE、IS_BEGIN、IS_NOT_BETWEEN |
| 更新時間 | IS、IS_NOT、IS_AFTER、IS_BEFORE、IS_BETWEEN、IS_NOT_BETWEEN、IS_EMPTY、IS_NOT_EMPTY |
| 參考 | HAS_ANY_OF， HAS_ALL_OF， IS_EXACTLY， HAS_NONE_OF， IS_EMPTY， IS_NOT_EMPTY |
| 查詢 | 取決於連結的欄位型別 |

>[!NOTE]
>
>**第1版備註：**&#x200B;第1版使用`$`首碼運運算元名稱（例如`$contains`、`$greaterThan`、`$isAnyOf`、`$hasAllOf`）。 每個欄位型別的支援條件集是相同的。

## 依人員欄位篩選

人員欄位篩選器(`user`、`created-by`、`updated-by`、`approved-by`)同時接受Adobe IMS使用者ID和Workfront使用者ID。 純字串值會解譯為Adobe IMS使用者ID。

若要設定識別碼型別以檢查Workfront使用者識別碼，您必須明確傳遞`id`和`idType`引數。 `idType`支援的值在Workfront使用者ID為&quot;`WF`&quot;，在Adobe IMS使用者ID為&quot;`IMS`&quot;。

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> 第1版注意：V1僅支援依使用者的IMS ID篩選。

## 依外部ID篩選外部參考欄位

外部參考欄位會將記錄連結到其他Adobe系統（例如Workfront專案或AEM Assets）中的物件。 在內部，Planning會將Planning記錄ID指定給這些物件。 若要直接依原始物件識別碼篩選這些欄位，請新增`"matchExternalId": true`至篩選條件。

此旗標僅適用於`referenceOptions.isExternal`為`true`的參考欄位；非外部參考欄位會忽略此旗標。 如果無法解析單一字串值，則要求會失敗，並產生`400 Bad Request`。 如果提供清單值，未解析的專案會透過未變更且完全不相符。

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>版本1注意： V1不支援依外部物件ID篩選。

## 外部連線欄位

Planning記錄型別可以託管外部參考欄位，這些欄位將記錄連結到其他Adobe系統中的物件，而不是其他Planning記錄型別。

若要透過API建立外部參考欄位，請將新`REFERENCE`欄位上的`referenceOptions.recordTypeId`設定為所需外部記錄型別的識別碼。 伺服器會自動從目標籤錄型別衍生`referenceOptions.isExternal=true`和連線中繼資料(`connectionName, objectName`)。

支援的外部物件型別包括Workfront物件（專案、工作、方案、產品組合、公司、群組、團隊、使用者）和AEM Assets （資產、內容片段）。

>[!NOTE]
>
>第1版注意： V1不支援建立外部連線欄位。


## 排序

在您的要求中加入`sort`陣列，依任何欄位排序結果：

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

系統會依順序評估多個排序欄位。 編頁時一律套用排序，以確保跨頁面順序一致。

若要將結果分組，請在排序時加入群組陣列：

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>第1版備註： V1使用`sorting` （非`sort`）、`groupingFieldIds` （欄位識別碼陣列，非`group`物件）以及現在已棄用的`rowOrderViewId`套用現有檢視的列順序。 版本不支援這些V1引數

## 欄位投影

若要限制回應中傳回的欄位，請使用逗號分隔清單中的`fieldIds`或`fieldAliases`查詢引數。 這樣會減少回應裝載大小，建議用於高容量或對延遲敏感的整合。

>[!NOTE]
>
>**第1版備註：**&#x200B;第1版使用`?attributes=`來投影（例如`?attributes=data,createdBy`），而非`?fieldIds=`或`?fieldAliases=`。

## 分頁

Planning API支援分頁回應，以管理大型資料集。

* **以游標為基礎的分頁**&#x200B;用於工作區、記錄型別、欄位和檢視。 傳遞上一個回應中的`cursor`值以擷取下一個頁面。 游標型回應包含hasMore旗標，以指出是否有更多頁面。
* **以頁面為基礎的分頁**&#x200B;用於記錄搜尋。 使用`page`和`size`作為查詢引數。 編頁時一律套用排序，以確保跨頁面順序一致。 請注意，分頁是以零為基準，因此若要擷取第二頁的結果，請使用&quot;`page=1`&quot;作為引數。

例如，使用以下請求，從記錄搜尋中擷取500筆記錄的第二頁：

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

所有分頁回應都包含一個結構化信封，指示是否有更多可用結果。 編頁時一律套用排序，以確保跨頁面順序一致。

>[!NOTE]
>
> **第1版備註：** V1使用傳入要求內文中的`offset`和`limit` （預設為500，最大為2,000）。 若要擷取記錄2001-4000，請在要求內文中設定&quot;`offset`&quot;： &quot;`2000`&quot;，&quot;`limit`&quot;： &quot;`2000`&quot;。 回應會傳回含有`totalCount`欄位的純資料記錄陣列。

## 大量作業

Planning API支援大量建立、更新、修補及刪除單一請求中的記錄。 如需端點路徑、要求格式和每個作業的記錄限制，請參閱[developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)的&#x200B;**API參考**。

>[!NOTE]
>
>**第1版注意：**&#x200B;第1版不提供大量作業。


## 權限

實體的許可權透過專用許可權API進行管理，與資源端點本身分開。 這可讓您讀取目前許可權、管理共用清單，以及獨立於資料作業處理存取請求。 如需詳細資訊，請參閱文章[Workfront Planning API](https://developer.adobe.com/wf-planning)中的「API參考」一節。

>[!NOTE]
>
>**第1版注意：**&#x200B;第1版未公開公開公開許可權API。 許可權層級會直接內嵌在資源回應DTO中。

## 搭配Workfront自訂表單使用Planning API

您可以從Workfront自訂表單中的外部查閱欄位呼叫Planning API，以直接在Workfront物件中呈現Planning資料。 如需詳細資訊，請參閱自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)中的外部查閱欄位範例[。

## 相關資源

如需更多API相關檔案，另請參閱下列文章：

* [Workfront Planning API](https://developer.adobe.com/wf-planning)開發人員檔案與參考
* [開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning存取權概觀](/help/quicksilver/planning/access/access-overview.md)
* [為Workfront整合建立OAuth2應用程式](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->