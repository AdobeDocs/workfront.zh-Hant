---
filename: api-changes-search
content-type: api
keywords: 對象，狀態，搜索，最佳，實踐，響應
navigation-topic: api-navigation-topic
title: 「核心API變更：狀態搜索響應
description: 變更Workfront儲存狀態物件的方式。
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# 核心API變更：狀態搜索響應

已變更Workfront儲存狀態物件的方式。 這些變更不會影響狀態搜尋請求的提出方式，但會透過傳回不完整的群組狀態清單，而影響API請求傳回的回應，這些請求包含對狀態物件的搜尋。

## 最佳實務

為了可靠地擷取群組可用狀態的完整清單，以下請求被視為最佳實務。

>[!NOTE]
>
>無論是否已對您的叢集進行狀態搜尋變更，建議所有使用者使用這些請求結構。

對於項目組狀態：

>**範例:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

對於任務組狀態：

>**範例:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

對於問題組狀態：

>**範例:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

這三個端點都接受 **includeHidden=true** 參數，以擷取指定群組的隱藏專案/工作/問題狀態。 在這些最佳實務範例之後為狀態搜尋查詢建立模型，將可確保所有群組狀態資訊都包含在每個回應中。

以下是對任務組進行狀態搜索查詢（包括系統級鎖定狀態）的示例 **Custom_1** 和未鎖定狀態 **Custom_2**:

>**範例:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

使用此格式可確保您的回應將包含下列所有項目：

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## 了解對舊版狀態搜索查詢所做的更改

在舊式系統下，狀態搜索查詢將複製查詢中包含的所有組可用的所有系統狀態。 之後，舊式回應將包含查詢中每個群組可用的所有系統狀態和群組層級狀態。

例如，此查詢（不遵循目前建議的最佳實務）:

>**範例:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

在舊版系統下會有下列回應，其中包含所有物件狀態：

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

但是，在對狀態的儲存和使用方式進行更新後，狀態不會為組複製，而是由系統級別的每個組繼承。 因此，搜尋API查詢只會讀取與特定群組直接相關聯的狀態，因此回應會包含系統鎖定和解除鎖定狀態，但只會針對新增相關狀態後所建立的群組。

更新舊版系統後，若未使用更新後的最佳實務方法進行狀態搜尋查詢，將會導致回應中傳回的群組狀態清單不完整。

以下是舊版系統更新後，此過時的請求結構傳回的範例：

>**範例:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

請注意，此回應僅包含群組特定狀態，並排除在系統層級宣告的狀態：

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
