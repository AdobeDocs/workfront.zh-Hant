---
filename: api-changes-search
content-type: api
keywords: 物件，狀態，搜尋，最佳，實務，回應
navigation-topic: api-navigation-topic
title: 核心API變更：狀態搜尋回應
description: 變更Workfront儲存狀態物件的方式。
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# 核心API變更：狀態搜尋回應

已變更Workfront儲存狀態物件的方式。 這些變更不會影響進行狀態搜尋請求的方式，但會影響API請求傳回的回應，這些API請求會傳回不完整的群組狀態清單，以搜尋狀態物件。

## 最佳實務

為了可靠地擷取適用於群組的完整狀態清單，下列請求被視為最佳實務。

>[!NOTE]
>
>建議所有使用者使用這些要求結構，不論叢集是否已變更狀態搜尋。

針對專案群組狀態：

>**範例：**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

任務群組狀態：

>**範例：**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

對於問題群組狀態：

>**範例：**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

這三個端點都接受&#x200B;**includeHidden=true**&#x200B;引數，以擷取指定群組的隱藏專案/任務/問題狀態。 在這些最佳實務範例之後建立狀態搜尋查詢的模型，將確保每個回應中都包含所有群組狀態資訊。

以下是正在對工作群組進行狀態搜尋查詢的範例，該工作群組包含系統層級的鎖定狀態&#x200B;**Custom_1**&#x200B;和解除鎖定狀態&#x200B;**Custom_2**：

>**範例：**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

使用此格式可確保您的回應包含下列所有內容：

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

## 瞭解對舊版狀態搜尋查詢所做的變更

在舊式系統下，狀態搜尋查詢會複製查詢中包含的所有群組可用的所有系統狀態。 然後，舊版回應將包含查詢中每個群組可用的所有系統狀態和群組層級狀態。

例如，此查詢（未遵循目前建議的最佳實務）：

>**範例：**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

在舊版系統中會有以下回應，包括所有物件狀態：

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

但是，在對儲存和使用狀態的方式進行更新後，狀態不會為群組複製，而是由系統層級的每個群組繼承。 因此，搜尋API查詢只會讀取與特定群組直接關聯的那些狀態，所以回應會包含系統鎖定和未鎖定狀態，但僅限於在相關狀態新增後建立的群組。

更新舊版系統後，若未使用更新後的最佳實務方法進行狀態搜尋查詢，將導致回應中傳回的群組狀態清單不完整。

以下是更新舊版系統後，此過時請求結構傳回的範例：

>**範例：**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

請注意，此回應僅包含群組特定狀態，而省略了在系統層級宣告的狀態：

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
