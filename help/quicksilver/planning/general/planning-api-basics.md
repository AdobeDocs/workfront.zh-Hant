---
title: Adobe Workfront規劃API基本需知
description: Adobe Workfront Planning API的目標是引入透過HTTP運作的REST-ful架構，簡化與Planning的整合建置。 本檔案假設您熟悉REST和JSON回應，並說明Planning API所採取的方法。
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: f11daa69f72c32418298ac75f81b0fb64835d99b
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 2%

---


# Adobe Workfront Planning API基本需知

{{planning-important-intro}}

<!--
Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 
-->

<!--
To comment out when we release V2 - everything else under this gets hidden after V2 release: 

# Adobe Workfront Planning API Basics

The goal of the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a RESTful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses.

For complete endpoint reference, request/ response schemas, and version-specific details, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

## Authentication

The Workfront Planning API uses OAuth 2.0 for authentication. Credentials are set up via the Adobe Developer Console. 

We support the following two flows depending on your integration type:

* **Server-to-server authentication (JWT)**: For automated integrations and backend services with no user interaction. Uses the OAuth Server-to-Server credential (client credentials grant — your application authenticates directly using its client ID and secret to obtain an access token, with no user login or consent step). 

    For information, see [Server to Server authentication](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).

* **User authentication (Authorization Code flow)**: for integrations acting on behalf of a specific user. Uses the OAuth Web App or Single Page App credential (authorization code grant — the user logs in and consents, after which your application receives an authorization code it exchanges for an access token). 

    For information, see [User Authentication](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/).

To get started, create a project in the Adobe Developer Console and add the Workfront Planning API to obtain your credentials. 

To set up credentials, create an OAuth2 application in Workfront. 

For information, see [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md). 

>[!NOTE]
>
>The `/login` endpoint and API key authentication are not supported for Workfront Planning. Do not use `sessionID` or `apiKey` parameters.


## API versioning

The Planning API is versioned via the URL path. 

The following are current supported versions: 

| Version   | Release date   |
|-----------|----------------|
| Version 1 | July 2024 |
| Version 2 | May 2026   |

(*****************add deprecation date column above, when we have one*****************)


For more information about the current supported versions, see the article [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

We recommend explicitly targeting a version in all integrations:

```
https://{customer-domain}/maestro/api/v2/...

```

When a new major version is released, the previous version will continue to be available until a deprecation date is communicated.

Follow the Workfront release notes to stay informed of API changes.


## URL structure and operations

Objects are manipulated by sending an HTTP request to their unique URI. The operation is specified by the HTTP method.

| Method   | Operation                                                            |
|----------|----------------------------------------------------------------------|
| GET      | Retrieve a single object by ID, or search/list objects               |
| POST     | Create a new object                                                  |
| PUT      | Replace an existing object (full update)                             |
| PATCH    | Partially update an existing object (only provided fields are modified) |
| DELETE   | Delete an object                                                     |

>[!NOTE]
>
>**Version1 note:** `PATCH` is not supported in Version 1. Use `PUT` for all updates.


For full endpoint paths and request/response examples, see the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## HTTP status codes

The Planning API returns standard HTTP status codes:

| Code                   | Meaning                                         |
|------------------------|-------------------------------------------------|
| 200 OK                 | Successful GET, PUT, or PATCH                   |
| 201 Created            | Successful POST (resource created)              |
| 204 No Content         | Successful DELETE                               |
| 207 Multi-Status          | Bulk operation completed with mixed results, where some items succeeded and some failed. Check individual item responses for details.                              |
| 400 Bad Request        | Invalid request — see error response for details |
| 401 Unauthorized       | Missing or invalid authentication token         |
| 403 Forbidden          | Authenticated but insufficient permissions      |
| 404 Not Found          | Resource does not exist                         |
| 409 Conflict           | Write conflict, the resource was modified by another request. Retry with the latest version.                          |
| 429 Too Many Requests  | Rate limit exceeded                             |

>[!NOTE]
>
>**Version 1 note:** Version 1 returns `200 OK` for all successful operations, including POST and DELETE.


## Error handling

The Planning API returns errors in a consistent format. Each error response includes a human-readable message, a machine-readable error code, and a request ID for support escalation.

Example error response:

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

Use `errorCode` (not `status`) to drive programmatic error handling. It provides the most specific classification of the failure.

>[!NOTE]
>
>**Version 1 note:** Version 1 error responses use a numeric `type` field (e.g. `40001`) instead of a string `errorCode`, and wrap detail in a `report` object rather than a top-level `detail` field.

## Filtering records

Use the `filter` parameter in record search requests to return only records matching specific criteria. For POST requests, `filter` is a JSON property in the request body. For GET requests, `filter` is a query parameter containing a JSON-encoded filter group. Filters use a typed composite structure with explicit logical operators.  

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

Filters can be nested using `AND` / `OR` operators to build compound conditions:

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
>**Version 1 note:** Version 1 uses Mongo-style untyped operators in a `filters` object. Operators are prefixed with `$` (e.g. `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Pagination parameters (`offset`, `limit`) and `recordTypeId` are passed in the request body rather than as URL path and query parameters.


## Field types and search modifiers

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Using search modifiers 

Workfront Planning supports the following search modifiers: 


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>Modifier</th>
      <th>Example</th>
      <th>Description</th>
      <th>Possible values</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"CONTAINS","value":"product"}</td><td>Returns records whose field value contains the filter</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"DOES_NOT_CONTAIN","value":"product"}</td><td>Returns records where the field value does not contain the filter</td><td class="possible">"New Launch"</td></tr>
    <tr><td class="modifier">IS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS","value":"new product launch"}</td><td>Returns records whose field value exactly matches the filter</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT","value":"product"}</td><td>Returns records whose field value does not exactly match the filter</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EMPTY"}</td><td>Returns records whose field value is empty</td><td class="possible">"" or null</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_EMPTY"}</td><td>Returns records whose field value is not empty</td><td class="possible">"New Product Launch"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN","value":"10"}</td><td>Returns records whose field value is greater than the filter</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN_OR_EQUAL","value":"10"}</td><td>Returns records whose field value is greater than or equal to the filter</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN","value":"10"}</td><td>Returns records whose field value is less than the filter</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN_OR_EQUAL","value":"10"}</td><td>Returns records whose field value is less than or equal to the filter</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Returns records whose field value falls between the two filter values</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Returns records whose field value does not fall between the two filter values</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_AFTER","value":"2024-01-01"}</td><td>Returns records whose date field value is after the filter</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BEFORE","value":"2024-12-31"}</td><td>Returns records whose date field value is before the filter</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_ANY_OF","value":["Active","Planned"]}</td><td>Returns records whose field value matches any value in the filter list</td><td class="possible">["Active","Planned","Complete"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NONE_OF","value":["Active","Planned"]}</td><td>Returns records whose field value matches none of the values in the filter list</td><td class="possible">["Active","Planned"]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ANY_OF","value":["Tag1","Tag2"]}</td><td>Returns records whose multi-value field contains any of the filter values</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ALL_OF","value":["Tag1","Tag2"]}</td><td>Returns records whose multi-value field contains all of the filter values</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EXACTLY","value":["Tag1"]}</td><td>Returns records whose multi-value field contains exactly the filter values and no others</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_NONE_OF","value":["Tag1"]}</td><td>Returns records whose multi-value field contains none of the filter values</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>
 
### Field types 

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

## Supported filter conditions by field type

| Field Type                  | Supported Conditions                                                                                         |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| text, long-text             | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                              |
| number, percentage, currency| IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY      |
| date                        | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY                         |
| single-select               | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                                   |
| multi-select, user          | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| boolean                     | IS                                                                              |
| formula               | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                               |
| created-by       | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF                                                                             |
| updated-by        | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                                                              |
| created-at      | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN                                                  |
| updated-at      | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY                                                   |
| reference                   | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| lookup                      | Depends on the linked field type                                                                             |

>[!NOTE]
>
>**Version 1 note:** Version 1 uses `$`-prefixed operator names (e.g. `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). The set of supported conditions per field type is the same.

## Filtering by People fields 

People field filters (`user`, `created-by`, `updated-by`, `approved-by`) accept both Adobe IMS user IDs and Workfront user IDs. A plain string value is interpreted as an Adobe IMS user ID. 

To set the identifier type to check the Workfront user ID, you need to explicitly pass `id` and `idType` parameters. Supported values for `idType` are "`WF`" for Workfront user IDs, and "`IMS`" for Adobe IMS user IDs. 

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
> Version 1 note: V1 only supports filtering by users' IMS ID.  

## Filtering External Reference Fields by External ID 

External reference fields link records to objects in other Adobe systems (such as Workfront projects or AEM Assets). Internally, Planning assigns Planning record IDs to these objects. To filter such fields directly by their original object ID, add `"matchExternalId": true` to a filter condition. 

This flag is only valid for reference fields where `referenceOptions.isExternal` is `true`; it is ignored for non-external reference fields. If a single string value cannot be resolved, the request fails with `400 Bad Request`. If a list value is supplied, unresolved entries pass through unchanged and simply do not match. 

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
>Version 1 note: V1 does not support filtering by external object IDs. 

## External Connection Fields 

Planning record types can host external reference fields that link records to objects in other Adobe systems instead of other Planning record types. 

To create an external reference field via the API, set `referenceOptions.recordTypeId` on a new `REFERENCE` field to the ID of the desired external record type. The server automatically derives `referenceOptions.isExternal=true` and the connection metadata (`connectionName, objectName`) from the target record type. 

Supported external object types include Workfront objects (projects, tasks, programs, portfolios, companies, groups, teams, users) and AEM Assets (assets, content fragments). 

>[!NOTE]
>
>Version 1 note: V1 does not support creating external connection fields. 


## Sorting

Sort results by any field by including a `sort` array in your request:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}

```

Multiple sort fields are evaluated in order. Always apply a sort when paginating to ensure consistent ordering across pages.

To group results, include a group array alongside sort: 

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 

```

>[!NOTE]
>
>Version 1 note: V1 uses `sorting` (not `sort`), `groupingFieldIds` (array of field IDs, not `group` objects), and the now-deprecated `rowOrderViewId` to apply an existing view's row order. None of these V1 parameters are supported in Version 2. 


---

## Field projection

To limit which fields are returned in a response, use the `fieldIds` or `fieldAliases` query parameters with a comma-separated list. This reduces response payload size and is recommended for high-volume or latency-sensitive integrations.

>[!NOTE]
>
>**Version 1 note:** Version 1 uses `?attributes=` for projection (e.g. `?attributes=data,createdBy`) rather than `?fieldIds=` or `?fieldAliases=`.

## Pagination

The Planning API supports paginated responses to manage large datasets.

* **Cursor-based pagination** is used for workspaces, record types, fields, and views. Pass a `cursor` value from the previous response to retrieve the next page. Cursor-based responses include a hasMore flag to indicate if there are more pages or not.
* **Page-based pagination** is used for record search. Use `page` and `size` as query parameters. Always apply a sort when paginating to ensure consistent ordering across pages. Note that pagination is zero-based, so in order to retrieve the results of the second page, use "`page=1`" as the parameter.   

For example, use the following request to retrieve the second page of 500 records from a record search: 

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 

```

All paginated responses include a structured envelope indicating whether more results are available. Always apply a sort when paginating to ensure consistent ordering across pages.

>[!NOTE]
>
> **Version 1 note:** V1 uses `offset` and `limit` passed in the request body (default 500, max 2,000). To retrieve records 2001–4000, set "`offset`": "`2000`", "`limit`": "`2000`" in the request body. The response returns a flat records array with a `totalCount` field.

## Bulk operations

The Planning API supports bulk create, update, patch, and delete of records in a single request. Refer to the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning) for endpoint paths, request formats, and per-operation record limits.

>[!NOTE]
>
>**Version 1 note:** Bulk operations are not available in Version 1.


## Permissions

Permissions to entities are managed through a dedicated Permissions API, separate from the resource endpoints themselves. This allows you to read current permissions, manage the sharing list, and handle access requests independently of data operations. For more information, see the "API references" section in the article [Workfront Planning API](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Version 1 note:** Version 1 does not expose a public Permissions API. Permission level is embedded directly in resource response DTOs.

## Using the Planning API with Workfront custom forms

You can call the Planning API from an External lookup field in a Workfront custom form to surface Planning data directly within Workfront objects. For more information, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Related resources

For more API-related documentation, also see the following articles:

* [Workfront Planning API](https://developer.adobe.com/wf-planning) developer documentation and reference
* [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md)
* [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

-->

Adobe Workfront Planning API的目標是引入透過HTTP運作的REST-ful架構，簡化與Planning的整合建置。 本檔案假設您熟悉REST和JSON回應，並說明Planning API所採取的方法。

熟悉Workfront Planning綱要將有助於您瞭解可用來從Workfront Planning中提取資料以進行整合的資料庫關係。

您可以從Workfront自訂表單中的外部查詢欄位呼叫Planning API。

如需外部查閱欄位的詳細資訊，請參閱自訂表單中的[外部查閱欄位範例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)。

>[!NOTE]
>
>使用Planning API時，所有與使用者相關的資訊將會使用Adobe Identity Management系統(IMS)使用者ID而非Workfront使用者ID傳回。
>
>如需詳細資訊，請參閱[在Adobe Admin Console中管理使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

## Workfront Planning API版本

* 第1版 — 2024年7月發行

  如需詳細資訊，請參閱本文章的[Workfront Planning API版本1](#workfront-planning-api-version-1)一節。
  <!--
    Maybe retitle the "Workfront Planning API" section below to "Workfront Planning API Version 1" when Version 2 releases
    -->

<!--
* Version 2 - released in May 2026

    For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.
-->

## Workfront Planning API第1版

Workfront Planning API第1版已於2024年7月發行。

以下小節說明Workfront API版本1中提供的功能。

除非另有指定，否則所有未來的API版本都將包含相同的功能。

<!--
Becky had put the title of this article as"Workfront Planning API URL", but she did not document what that URL is; asking dev and hiding it for now
-->

<!--
For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).
-->

### 作業

透過傳送HTTP請求至物件的唯一URI來控制物件。 要執行的作業會由HTTP方法指定。

標準HTTP方法會對應至下列作業：

* **GET** — 依識別碼擷取物件，依查詢搜尋所有物件
* **貼文** — 插入新物件
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
        <td>傳回欄位值空白的記錄  </td>
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
..
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

請求內文：

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

`POST /v1/records/search`



請求內文：

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

<!--

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