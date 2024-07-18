---
content-type: api
navigation-topic: api-navigation-topic
title: 事件訂閱的傳出訊息格式
description: 事件訂閱的傳出訊息格式
author: Becky
feature: Workfront API
role: Developer
exl-id: addcf5bc-a101-4bb0-93a6-46b4af67c848
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# 事件訂閱的傳出訊息格式

隨著Adobe Workfront 2017.3的發行，事件訂閱的輸出訊息格式將會變更，以提高效能並更好地使用事件訂閱來整合。

## 更新傳出訊息格式

將對傳出訊息格式進行下列變更：

* 傳出訊息將包含Workfront資源的oldState和newState。

  這些值會顯示因Workfront中的事件而對物件所做的變更。

* eventTime中繼資料欄位將新增至所有傳出訊息。

  此欄位將以Nanoseconds和EpochSeconds表示事件發生時間。 排序由您的整合處理之事件時，請使用eventTime。

* 將會移除NOTE資源上的owner：companyID參考欄位。
* 將移除DOCU （檔案）資源上的currentVersion參考物件。

如果您目前使用Workfront活動訂閱，需在2017.3版之前更新Workfront整合，才能解決這些變更。

若要深入瞭解事件訂閱，請參閱[事件訂閱API](../../wf-api/general/event-subs-api.md)。

## 新舊訊息格式的範例

2017.3版發行後將不再使用下列舊格式CREATE訊息：

```
{
  "eventType": "CREATE",
  "subscriptionId": "8a0d839d5ef32c9a015ef33064b00001",
  "fields": {
     "ID": "59d7db3c0000014b05536251b669a3e4",
     "name": "EventSub Test 53350c27-ce58-40e9-af75-a2d45ff13046",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:36:28.722-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:36:28.785-0600",
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
     "referenceNumber": 1891,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```

2017.3版發行後將使用下列新格式CREATE訊息：

```
{
   "eventType": "CREATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef32e2cde0000",
   "eventTime": {
      "nano": 414000000,
      "epochSecond": 1507318444
   },
   "newState": {
     "ID": "59d7daab0000011b8faebf0f60d25d08",
     "name": "EventSub Test 3700e224-0ef7-4571-b200-09109712152c",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:34:03.562-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:34:04.000-0600",
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
     "referenceNumber": 1890,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   },
   "oldState": {}
```

2017.3版發行後將不再使用下列舊格式UPDATE訊息：

```
{
     "eventType": "UPDATE",
     "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
     "fields": {
     "ID": "59d7dcde000001b2330bda8ac63fee16",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:43:26.305-0600",<
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:43:49.265-0600",
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
     "referenceNumber": 1892,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   }
 }
```

2017.3版發行後將使用以下新格式UPDATE訊息：

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
     "currency": null,
     "categoryID": null,
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
     "ownerID": "544820df0000142362741fc0c368de19"
     "templateID": null,
     "priority": 0,
     "companyID": null,
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
