---
content-type: api
navigation-topic: wf-api
title: 取得使用者可用的時間API
description: 取得使用者可用的時間API
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
TQID: https://experienceleague.adobe.com/JPvalH2RQRfMeqbYyWXyjyXCx-bdaZwRoR6WDRerZ5U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 95
ht-degree: 4%

---

# 使用者可用時間API

**URI： attask/api/v15.0/user/getUsersAvailableTime**

使用者可用時間端點會擷取有關使用者可用時間的資料。 這允許根據使用者屬性和時間間隔整合資料。

## 範例請求

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## 要求引數

* **userIDs**：字串陣列。 必填。 範例：`"61a9cc0500002f9fdaa7a6f824f557e1"`。

* **fromDate**： datetime。 字串。 必填。 範例： `"2022-07-10T00:00:00"`。

* **toDate**： datetime。 字串。 必填。 範例`"2022-07-20T23:59:59"`。

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

## 回應引數

* **AVL**：實際可用時數。 數字陣列。
* **PAVL**：排程的純可用時數，不包含非工作日或使用者休假。 字串。
