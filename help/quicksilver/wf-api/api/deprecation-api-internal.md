---
content-type: api
navigation-topic: api-navigation-topic
title: 棄用API — 內部
description: 棄用API — 內部
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 棄用API — 內部

API — 內部API是Adobe Workfront API的版本，由於其設計和用途不受支援。 雖然它包含Workfront API的最新更新，但可能會有所變更，恕不另行通知，因此在生產整合中應謹慎使用。 Workfront強烈建議將所有API內部整合更新至已設定版本API。

若要深入瞭解Workfront API的支援版本，請參閱 [API版本設定和支援排程](../../wf-api/api/api-version-support-schedule.md).

**使用API — 不支援**

如果您的整合需要已建立版本API中不提供的功能，Workfront建議使用「不支援API」。 與API內部類似，不支援API不支援。 「不支援API」也包含Workfront API的最新變更，且可能隨時變更，恕不另行通知。 Workfront鼓勵您使用測試環境中不支援的API，以便探索新功能並確保API沒有錯誤。

**判斷您使用的API版本**

您可以使用REST來建構URI，以透過HTTPS將呼叫傳送至Workfront，然後傳回JSON回應，藉此判斷整合功能所使用的API版本。

以下範例顯示呼叫API-Internal的URI：

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

以下範例顯示呼叫API — 不支援的URI：

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

以下範例顯示呼叫15.0版API的URI：

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
