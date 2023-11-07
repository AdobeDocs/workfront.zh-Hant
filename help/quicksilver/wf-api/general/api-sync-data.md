---
content-type: api
keywords: API，資料，同步，日誌，專案，物件
navigation-topic: general-api
title: 使用API來同步處理程式與服務的資料
description: 使用API來同步處理程式與服務的資料
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# 使用API來同步處理程式與服務的資料

以下是您運用API來同步處理程式和服務資料的常見方式。

## 近乎即時的更新

Adobe Workfront使用「事件訂閱」（通常稱為Webhook），透過API將支援物件和動作的近乎即時更新傳送至您所需的端點。 您可能會在5秒內收到有關新物件和動作的更新，但平均而言，更新大約會在1秒後送達。 如需關於支援的物件型別、支援的動作型別、技術詳細資訊，以及如何設定事件訂閱的範例，請參閱 [事件訂閱API](../../wf-api/general/event-subs-api.md) 和 [事件訂閱傳送需求](../../wf-api/general/setup-event-sub-endpoint.md).

## 批次更新

批次更新是透過定期向Workfront伺服器提出請求來設定系統以進行更新的一種方式。 有很多方法可以做到，但一般而言，程式包含讓您的服務向Workfront API伺服器提出要求，以及搜尋自上次要求呼叫以來已建立或修改的物件。 如需有關潛在請求呼叫和實用引數的資訊，請參閱 [GET行為](../../wf-api/general/api-basics.md#get-behavior) 區段來自 [API基本概念](../../wf-api/general/api-basics.md) 文章。

當您設定批次更新的服務時，請謹記以下一些重要事項：

### 輸入日期

輸入日期是使用ISO 8601格式來儲存。 此標準包含日期、時間和時區資訊。

**範例：** ISO 8601日期格式

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

建立物件的日期和上次修改物件的日期分別儲存為「entryDate」和「lastUpdateDate」。 如需Workfront物件、其關聯欄位和欄位名稱的深入資訊，請參閱 [API總管](../../wf-api/general/api-explorer.md). 請注意，任何指定Workfront物件的entryDate都不會變更，因為每次修改物件時，lastUpdatedDate都會變更。

**範例：** 問題物件的GET請求，利用 **lastUpdateDate** 欄位。 此請求將傳回自指定日期以來更新的所有問題。

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### 日誌專案物件

如果您想要取得有關物件上特定欄位的變更，則可以查詢「Journal Entry」物件。 Workfront Journal Entry物件可設定為每次修改特定物件欄位時，都記錄有關這些欄位的資訊，請參閱 [設定系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) 以取得其他詳細資訊。

將欄位設定為記錄為日誌專案物件的一部分時，每次修改該欄位時都會建立對應的日誌專案。 然後，您可以使用類似以下的API呼叫來查詢Journal Entry物件：

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot;用於檢視變更的日誌專案，而不是檢視變更的物件本身。
