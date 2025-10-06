---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 疑難排解：使用Workfront for Outlook時發生outlookIdentityToken錯誤
description: 如果使用Outlook版Workfront時發生outlookIdentityToken錯誤，您必須為組織啟用Microsoft 365舊版權杖。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 43%

---

# 疑難排解：使用Workfront for Outlook時發生outlookIdentityToken錯誤

>[!IMPORTANT]
>
>[Microsoft已停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，這些權杖是由Workfront Outlook增益集用於驗證。 Microsoft的這項變更會分階段推出，並於2025年10月1日完成。
>
>**由於Microsoft已停用這些權杖，適用於Microsoft Outlook整合的Workfront已停止運作。**

使用Outlook適用的Workfront時，您可能會看到下列錯誤：

```
Unexpected error
Unable to get the outlookIdentityToken
```

若要解決此錯誤，您必須為組織啟用 Microsoft 365 舊版權杖。因為這必須在 Microsoft 365 中完成，所以 Workfront 無法為您的組織啟用這些權杖。

如需有關啟用 Microsoft 365 舊版權杖的說明，請參閱 Microsoft 文件中的[開啟或關閉舊版 Exchange Online 權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)。

如需有關舊版權杖的詳細資訊，請參閱 Microsoft 文件中的[我可以重新開啟 Exchange Online 舊版權杖嗎？](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)。
