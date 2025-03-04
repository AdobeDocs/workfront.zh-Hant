---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 疑難排解：使用Workfront for Outlook時發生outlookIdentityToken錯誤
description: 如果使用Outlook版Workfront時發生outlookIdentityToken錯誤，您必須為組織啟用Microsoft 365舊版權杖。
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 571ed00f44322d73183323c4d4154284cd028301
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# 疑難排解：使用Workfront for Outlook時發生outlookIdentityToken錯誤

使用Outlook適用的Workfront時，您可能會看到下列錯誤：

```
Unexpected error
Unable to get the outlookIdentityToken
```

若要解決此錯誤，您必須為組織啟用Microsoft 365舊版代號。 由於此工作必須在Microsoft 365中完成，Workfront無法為您的組織啟用這些代號。

如需啟用Microsoft 365舊版權杖的指示，請參閱Microsoft檔案中的[開啟或關閉舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)。

如需舊版權杖的詳細資訊，請參閱[我可以重新開啟Exchange Online舊版權杖嗎？Microsoft檔案中的](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)。
