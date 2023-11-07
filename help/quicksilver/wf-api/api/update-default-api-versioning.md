---
content-type: api
navigation-topic: api-navigation-topic
title: 更新使用預設API版本設定的整合
description: 更新使用預設API版本設定的整合
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# 更新使用預設API版本設定的整合

我們每半年發佈新版本的Adobe Workfront API。 每個版本在發行後三年內都受到支援，但在有版本提供但不支援的過時狀態下，還會額外支援一年。

未在URI中指定API版本的整合會自動路由到預設值。 如果您希望API呼叫使用特定版本的API，必須在Workfront API請求中指定該版本。

>[!NOTE]
>
>如果您的組織目前正在使用預設API，您的Workfront管理員已收到Announcement Center訊息，提供有關預設API的更多說明。

若要瞭解如何在API要求中指定版本，請參閱 [在您的整合中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

## 使用預設API時的注意事項

使用Workfront預設API時，請考量下列事項：

* API最新版本的預設版本。 任何未指定版本的API呼叫都將使用預設版本。 每當Workfront發行新版API時，預設版本都會更新至最新版本。 **因此，在發行新版本的Workfront API後，應檢查使用預設版本的任何API呼叫，以確定仍支援該功能**.
* 如果您的組織目前正在使用先前已棄用的預設API，您的Workfront管理員已收到Announcement Center訊息，提供有關預設API的更多說明。

若要檢視最新版的API，請參閱 [API版本設定和支援排程](../../wf-api/api/api-version-support-schedule.md).

## 將您的整合更新至支援的API版本

如果您的Workfront API請求未指定版本，則使用預設值。 建議您提出API請求，指定支援的API版本，最好使用最新支援的API。

例如，下列Workfront API請求未指定API版本：

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

提出此要求時，您會收到包含JSON編碼文字的回應，其中指定來自Workfront執行個體的資料。 由於此URI中未指定API版本，因此呼叫會移至「預設」。

若要將預設API請求轉換為已設定版本API請求，只需呼叫支援的API版本即可。 例如，以下URI請求版本15：

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

更新Workfront API請求時，您可以指定我們的API的任何支援版本。 若要進一步瞭解參照特定API，請參閱 [在您的整合中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

若要確保支援視窗上限，您應呼叫最新版本。 如需支援的API清單，請參閱 [API版本設定和支援排程](../../wf-api/api/api-version-support-schedule.md).

## API預設版本的歷程記錄

「預設API」或「預設」的原始用途是將它對應至最新版本的Workfront API。 這樣可讓具有基本整合（稱為預設）的客戶永遠不必更新其API請求。

2011年，Workfront發行了API 3.0版。 預設自動移至3.0版，這中斷了許多客戶整合，這些整合過於複雜，以致於無法在不更新的情況下使用3.0版。 因此，Workfront復原此變更，並將預設版本保留為版本2。

自2011年以來，Workfront已大幅增加API功能。 因此，我們已淘汰舊版的API。 2017年，我們完全移除預設版本的概念，而非更新「預設」。 這是為了鼓勵客戶使用穩定版本的API，並在最多三年的週期內維持他們的整合。

Workfront現在正在恢復預設API版本。 預設API設定為Workfront API的最新版本，並會在每次發行新版本時更新至最新版本。

