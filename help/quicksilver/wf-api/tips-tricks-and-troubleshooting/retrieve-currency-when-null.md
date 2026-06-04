---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 當貨幣為空值時擷取專案的貨幣資訊
description: 當貨幣為空值時擷取專案的貨幣資訊
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
TQID: https://experienceleague.adobe.com/fWBcEeqoJFK6WzcEE2Ajqv6cdxk0J9IN1CiPPGU6pIg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 0%

---

# 當貨幣為空值（未指派）時，擷取專案的貨幣資訊

具有貨幣欄位的專案物件可使用以下請求來擷取：

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

這會傳回下列回應內文：

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

如果未設定專案的貨幣，此回應將包含值為`null`的貨幣：

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

如果您需要專案的貨幣（例如計算），可以擷取客戶的預設貨幣：

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

回應包含使用者已設定為預設的貨幣，該貨幣將用於該客戶未設定貨幣的任何專案：

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
