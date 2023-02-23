---
content-type: api
navigation-topic: api-navigation-topic
title: 不再使用API — 內部
description: 不再使用API — 內部
author: John
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 不再使用API — 內部

API-Internal是Adobe Workfront API的版本，由於其設計和用途而不受支援。 雖然包含Workfront API的最新更新，但如有變更，恕不另行通知，因此應在生產整合中小心使用。 Workfront強烈建議將所有API — 內部整合更新至版本控制API。

若要進一步了解Workfront API的支援版本，請參閱 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).

**不支援使用API**

如果您的整合需要版本控制API中未提供的功能，Workfront建議您使用不支援的API。 與API — 內部類似，不支援API — 不支援。 API — 不支援的也包括Workfront API的最新變更，且可能會有所變更，恕不另行通知。 Workfront鼓勵您使用測試環境中不支援的API，以探索新功能並確保API沒有錯誤。

**決定您使用的API版本**

您可以使用REST來建構URI，透過HTTPS傳送呼叫至Workfront，然後傳回JSON回應，以判斷整合使用的API版本。

下列範例顯示呼叫API-Internal的URI:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

以下示例顯示調用API不受支援的URI:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

以下範例顯示呼叫API 15.0版的URI:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
