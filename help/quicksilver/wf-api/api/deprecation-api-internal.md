---
content-type: api
navigation-topic: api-navigation-topic
title: 棄用API — 內部
description: 棄用API — 內部
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
TQID: https://experienceleague.adobe.com/LGyk8MIATMQj6JHqKmjkeL2pXW-b6xtxo2heMd4h0y4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 241
ht-degree: 0%

---

# 棄用API — 內部

API — 內部API是Adobe Workfront API的版本，由於其設計和用途不受支援。 雖然它包含Workfront API的最新更新，但可能會有所變更，恕不另行通知，因此在生產整合中應謹慎使用。 Workfront強烈建議將所有API內部整合更新至已設定版本API。

若要深入瞭解Workfront API的支援版本，請參閱[API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md)。

**使用API — 不支援**

如果您的整合需要已建立版本API中不提供的功能，Workfront建議使用「不支援API」。 與API內部類似，不支援API不支援。 「不支援API」也包含Workfront API的最新變更，且可能隨時變更，恕不另行通知。 Workfront鼓勵您使用測試環境中不支援的API，以便探索新功能並確保API沒有錯誤。

**決定您正在使用的API版本**

您可以使用REST來建構URI，以透過HTTPS將呼叫傳送至Workfront，然後傳回JSON回應，藉此判斷整合功能所使用的API版本。

以下範例顯示呼叫API-Internal的URI：

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

以下範例顯示呼叫API — 不支援的URI：

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>API不支援的呼叫會省略URL的`/api`區段。

以下範例顯示呼叫15.0版API的URI：

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
