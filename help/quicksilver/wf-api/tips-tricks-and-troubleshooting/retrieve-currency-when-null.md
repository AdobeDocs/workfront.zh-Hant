---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 當貨幣為null時，為項目檢索貨幣資訊
description: 當貨幣為null時，為項目檢索貨幣資訊
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# 當貨幣為null（未分配）時，為項目檢索貨幣資訊

可使用下列請求來擷取具有貨幣欄位的專案物件：

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

如果未為項目設定貨幣，則此響應將包括具有值的貨幣 `null`:

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

如果需要項目的幣種（例如計算），則可以檢索客戶的預設幣種：

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

回應包含使用者已設為預設的貨幣，而該貨幣將用於未設定該貨幣之客戶的任何專案：

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
