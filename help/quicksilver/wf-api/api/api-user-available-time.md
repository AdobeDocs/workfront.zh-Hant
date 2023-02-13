---
content-type: api
navigation-topic: wf-api
title: 使用可用時間API
description: 使用可用時間API
author: John
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: aea37c1d200dfadf9ccbb7b36145eb04d5ab4b6d
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 7%

---

# 可用時間API的用戶

**URI:attask/api/v15.0/user/getUsersAvailableTime**

可用時間端點會擷取使用者可用時間上的資料。 這可讓整合根據使用者屬性和時間間隔來匯總資料。

## 範例要求

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## 要求參數

* **userIDs**:字串的陣列。 必要. 範例: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**:datetime。 字串。 必要. 範例:  `"2022-07-10T00:00:00"`.

* **toDate**:datetime。 字串。 必要. 範例 `"2022-07-20T23:59:59"`.

## 範例回應：

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## 回應參數

* **AVL**:實際可用小時數。 數字陣列。
* **帕夫爾**:不包括非工作日或用戶休假時間的純可用時間。 字串.
