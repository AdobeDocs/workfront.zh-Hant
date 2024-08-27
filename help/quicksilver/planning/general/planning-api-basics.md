---
title: Adobe Workfront規劃API基本需知
description: Adobe Workfront Planning API的目標是引入透過HTTP運作的REST-ful架構，簡化與Planning的整合建置。 本檔案假設您熟悉REST和JSON回應，並說明Planning API所採取的方法。
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 20e8d45264f9441d9576c7d4d5521e4f6053a7f3
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 1%

---


# Adobe Workfront Planning API基本需知

{{planning-important-intro}}

Adobe Workfront Planning API的目標是引入透過HTTP運作的REST-ful架構，簡化與Planning的整合建置。 本檔案假設您熟悉REST和JSON回應，並說明Planning API所採取的方法。

熟悉Workfront Planning綱要將有助於您瞭解可用來從Workfront Planning中提取資料以進行整合的資料庫關係。

您可以從Workfront自訂表單中的外部查詢欄位呼叫Planning API。

如需外部查閱欄位的詳細資訊，請參閱自訂表單中的[外部查閱欄位範例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)。

## Workfront規劃API URL

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### 營運

透過傳送HTTP請求至物件的唯一URI來控制物件。 要執行的作業會由HTTP方法指定。

標準HTTP方法會對應至下列作業：

* **GET** — 依識別碼擷取物件，依查詢搜尋所有物件
* **POST** — 插入新物件
* **PUT** — 編輯現有的物件
* **DELETE** — 刪除物件

如需每個作業的詳細資訊與範例，請參閱[Workfront Planning API開發人員檔案](https://developer.adobe.com/wf-planning/)。

### 欄位型別和搭配使用的搜尋修飾詞

您可以使用包含欄位的修飾詞和篩選器來控制要在結果中傳回哪些資料。

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### 使用搜尋修飾元

Workfront Planning支援下列搜尋修飾元：

<table>
    <tr>
        <td><b>修飾詞</b></td>
        <td><b>範例</b></td>
        <td><b>說明</b></td>
        <td><b>可能的值</b></td>
    </tr>
    <tr>
        <td>$contain </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>傳回其欄位值包含篩選器的記錄  </td>
        <td>"新產品上市"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>傳回欄位值不含篩選器的記錄  </td>
        <td>"新增啟動項"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>傳回其欄位值完全符合篩選器的記錄  </td>
        <td>"新產品上市"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>傳回欄位值完全不符合篩選器的記錄  </td>
        <td>"新產品上市"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>傳回欄位值非空白的記錄  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>傳回欄位值非空白的記錄  </td>
        <td>"新產品上市"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>傳回欄位值大於篩選器的記錄  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>傳回欄位值大於或等於篩選器的記錄  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>傳回欄位值小於篩選器的記錄  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>傳回欄位值小於或等於篩選器的記錄 </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>傳回欄位值在篩選器之後的記錄  </td>
        <td>「2024-05-15T20:00:00.000Z」  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>傳回欄位值在篩選器之前的記錄 </td>
        <td>「2024-05-12T20:00:00.000Z」 </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>傳回欄位值在篩選器之間的記錄  </td>
        <td><ul><li>「2024-05-12T20:00:00.000Z」 </li><li>「2024-05-14T20:00:00.000Z」 </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>傳回欄位值不在篩選器之間的記錄  </td>
        <td><ul><li>「2024-05-09T20:00:00.000Z」  </li><li>「2024-05-17T20:00:00.000Z」  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>傳回欄位值為任何篩選器的記錄  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>傳回其欄位值不為任何篩選器的記錄 </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>傳回欄位值具有任何篩選器的記錄  </td>
        <td><ul><li>["active"， "fixed"]  </li><li>["fixed"、"completed"、"finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>傳回其欄位值具有所有篩選器的記錄  </td>
        <td><ul><li>["active"， "completed"]   </li><li>["active"、"completed"、"finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>傳回欄位值不含任何篩選器的記錄 </td>
        <td>["fixed"， "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>傳回其欄位值剛好是篩選器的記錄  </td>
        <td>["active"， "completed"]  </td>
    </tr>
</table>

#### 欄位類型

以下是支援的欄位型別清單，以及可搭配這些欄位型別使用的搜尋修飾詞

| 欄位型別 | 支援的搜尋修飾元 |
|---|---|
| 文字 | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| 長文字 | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| 數字 | $is， $isNot， $greaterThan， $greaterThanOrEqual， $lessThan， $lessThanOrEqual， $isEmpty， $isNotEmpty |
| 百分比 | $is， $isNot， $greaterThan， $greaterThanOrEqual， $lessThan， $lessThanOrEqual， $isEmpty， $isNotEmpty |
| 貨幣 | $is， $isNot， $greaterThan， $greaterThanOrEqual， $lessThan， $lessThanOrEqual， $isEmpty， $isNotEmpty |
| 日期 | $is， $isNot， $isAfter， $isBefore， $isBetween， $isNotBetween， $isEmpty， $isNotEmpty |
| 單選 | $is， $isNot， $isAnyOf， $isNoneOf， $isEmpty， $isNotEmpty |
| 多選 | $hasAnyOf， $hasAllOf， $isExactly， $hasNoneOf， $isEmpty， $isNotEmpty |
| 布林值 | $is |
| 使用者 | $hasAnyOf， $hasAllOf， $isExactly， $hasNoneOf， $isEmpty， $isNotEmpty |
| 公式 | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| url | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| 建立者 | $is， $isNot， $isAnyOf， $isNoneOf |
| 建立時間 | $is， $isNot， $isAfter， $isBefore， $isBetween， $isNotBetween |
| 更新者 | $is， $isNot， $isAnyOf， $isNoneOf， $isEmpty， $isNotEmpty |
| 更新時間 | $is， $isNot， $isAfter， $isBefore， $isBetween， $isNotBetween， $isEmpty， $isNotEmpty |
| 參考 | $hasAnyOf， $hasAllOf， $isExactly， $hasNoneOf， $isEmpty， $isNotEmpty |
| 查詢 | 取決於連結的欄位 |

### 使用「And」和「Or」陳述式

在API呼叫中，您可以擁有根據由$and&quot;和&quot;$or&quot;陳述式結合的多項條件的篩選器

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

### 使用欄位請求引數

您可以使用欄位請求引數來指定應傳回的特定欄位清單（以逗號分隔）。 這些欄位名稱會區分大小寫。

例如，請求

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
....
```

會傳回類似下列的回應：


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### 排序API中的查詢結果

如果您將以下內容附加至API呼叫，則可以根據任何欄位來排序結果：


`/v1/records/search`

要求內文：

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

### 查詢限制和分頁回應

依預設，Planning API請求會從清單開頭傳回500個結果。 若要覆寫結果數目的預設限制，您可以在要求中使用`limit`引數，並將其設定為不同的數目，最多2000個結果。

建議您將`offset`引數新增至您的請求，以針對大型資料集使用分頁回應。 分頁回應可讓您指定應傳回的第一個結果的位置。

例如，如果要傳回結果2001-4000，您可以使用以下請求。 此範例會從2001年的結果開始，傳回處於作用中狀態的2000筆記錄：

`POST /v1/records/search `



要求內文：

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

為確保結果正確分頁，請使用排序引數。 如此可讓結果以相同順序傳回，因此分頁不會重複或略過結果。

如需排序的詳細資訊，請參閱本文中的[在API中排序查詢結果](#sorting-query-results-in-the-api)。
