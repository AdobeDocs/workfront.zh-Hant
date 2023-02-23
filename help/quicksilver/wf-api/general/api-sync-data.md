---
content-type: api
keywords: API，資料，同步，日誌，條目，對象
navigation-topic: general-api
title: 使用API來同步方案和服務的資料
description: 使用API來同步方案和服務的資料
author: John
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# 使用API來同步方案和服務的資料

這些是您運用API來同步方案和服務資料的一些常見方式。

## 近乎即時更新

Adobe Workfront使用「事件訂閱」（通常稱為webhook），透過API將支援物件和動作的近乎即時更新傳送至您所需的端點。 您可以預期在5秒內收到有關新物件和動作的更新，但平均大約1秒後會收到更新。 有關支援的對象類型、支援的操作類型、技術詳細資訊以及如何設定事件訂閱的示例的詳細資訊，請參見 [事件訂閱API](../../wf-api/general/event-subs-api.md) 和 [事件訂閱傳送需求](../../wf-api/general/setup-event-sub-endpoint.md).

## 批次更新

批次更新可定期向Workfront伺服器要求，以設定您的系統以進行更新。 有許多方法可做到，但一般而言，程式包含讓服務向Workfront API伺服器提出要求，以及搜尋自上次要求呼叫以來已建立或修改的物件。 如需潛在請求呼叫和實用參數的相關資訊，請參閱 [GET行為](../../wf-api/general/api-basics.md#get-behavior) 區段 [API基本介紹](../../wf-api/general/api-basics.md) 文章。

在您設定批次更新服務時，請謹記以下幾點重要事項：

### 參加日期

使用ISO 8601格式設定來儲存登入日期。 此標準包含日期、時間和時區資訊。

**範例：** ISO 8601日期格式

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

建立對象的日期和修改對象的最後日期都分別儲存為「entryDate」和「lastUpdateDate」。 如需Workfront物件、其相關欄位和欄位名稱的詳細資訊，請參閱 [API Explorer](../../wf-api/general/api-explorer.md). 請注意，任何指定Workfront物件的entryDate不會變更，因為每次修改物件時，lastUpdatedDate都會變更。

**範例：** GET對問題物件的要求，利用 **lastUpdateDate** 欄位。 此請求會傳回自指定日期以來更新的所有問題。

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### 日記帳分錄對象

如果您希望獲取有關對象上特定欄位的更改，則可以查詢「日記帳分錄」對象。 可以設定「Workfront日記帳分錄」對象以在每次修改這些欄位時記錄有關特定對象欄位的資訊，請參閱 [配置系統更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) 以取得其他詳細資訊。

將欄位設定為作為日記帳分錄對象的一部分進行記錄時，每次修改該欄位時都將建立相應的日記帳分錄。 然後，您可以使用類似以下的API調用來查詢日記帳分錄對象：

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot;用於查看更改的日記帳分錄，而不是查看更改的對象本身。
