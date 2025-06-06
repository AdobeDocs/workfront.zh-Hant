---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 疑難排解：使用Workfront for Outlook時發生outlookIdentityToken錯誤
description: 如果使用Outlook版Workfront時發生outlookIdentityToken錯誤，您必須為組織啟用Microsoft 365舊版權杖。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# 疑難排解：使用Workfront for Outlook時發生outlookIdentityToken錯誤

>[!IMPORTANT]
>
>[Microsoft正在停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，Workfront Outlook增益集目前使用這些權杖進行驗證。 Microsoft的這項變更已開始影響客戶，並將在2025年10月前持續分階段推出。
>
>* **在Microsoft完全停用這些Token後，適用於Microsoft Outlook整合的Workfront將無法繼續運作。**
>
>在這次變更中，Microsoft已決定變更代號重新啟用的方式。 在&#x200B;**2025年6月30日**&#x200B;之後，管理員將無法再自行重新啟用權杖 — 只有Microsoft支援可授予例外狀況。 **在2025年10月1日，所有租使用者的舊版代號將會關閉。 將不會授與例外。**


使用Outlook適用的Workfront時，您可能會看到下列錯誤：

```
Unexpected error
Unable to get the outlookIdentityToken
```

若要解決此錯誤，您必須為組織啟用 Microsoft 365 舊版權杖。因為這必須在 Microsoft 365 中完成，所以 Workfront 無法為您的組織啟用這些權杖。

如需有關啟用 Microsoft 365 舊版權杖的說明，請參閱 Microsoft 文件中的[開啟或關閉舊版 Exchange Online 權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)。

如需有關舊版權杖的詳細資訊，請參閱 Microsoft 文件中的[我可以重新開啟 Exchange Online 舊版權杖嗎？](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)。
