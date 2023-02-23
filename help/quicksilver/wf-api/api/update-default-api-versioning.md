---
content-type: api
navigation-topic: api-navigation-topic
title: 更新使用預設API版本設定的整合
description: 更新使用預設API版本設定的整合
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 889084f9a3740b40c84c658f9b0c17270b0a37d7
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 更新使用預設API版本設定的整合

<!-- This article is going to need a complete revamp or to be removed-->

<span class="preview">本頁強調顯示的資訊指的是尚未普遍提供的功能。 它僅適用於預覽沙箱環境。</span>

我們每兩年發行一次新版Adobe Workfront API。 每個版本在發行後三年內都受支援，且會在已過時狀態中再多支援一年，此時版本已可供使用但不受支援。

未在URI中指定API版本的整合會自動路由至「預設」。 如果您希望API呼叫使用特定版本的API，您必須在Workfront API請求中指定該版本。

>[!NOTE]
>
>如果貴組織目前使用預設API，您的Workfront管理員已收到公告中心訊息，其中包含有關預設API的進一步指示。


<!--
Integrations that do not specify a version of the API in the URI are automatically routed to Default, which has been deprecated. In order for your Workfront integrations to be valid, you must specify a supported API version in your Workfront API requests.
-->

若要了解如何在API請求中指定版本，請參閱 [在您的整合中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

## 使用預設API時的考量事項

使用Workfront預設API時，請考量下列事項：

* 在23.2版之後，API的預設版本將設為最新版本。 任何未指定版本的API呼叫都會使用預設版本。 每次Workfront發行新版API時，預設版本都會更新為最新版本。 **因此，在發行新版Workfront API後，應檢查使用預設版本的任何API呼叫，以確定仍支援該功能**.
* 如果貴組織目前使用已棄用的預設API，您的Workfront管理員會收到公告中心訊息，其中包含有關預設API的進一步指示。
* <span class="preview">預覽環境中的預設API目前已設為最新版本。 生產環境中的預設API將設為23.2版之後的最新版本。</span>

若要查看最新版的API，請參閱 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).

<!--

## Deprecating Default

In an effort to improve the Workfront API, we are in the process of removing older API versions that have exceeded our support window of three years. One of these versions is Version 2, to which Default is mapped. This version was released in 2010, and much of the logic supported in the Attask/Workfront application at that time either no longer exists or has substantially changed.

We deprecated Default in July 2017, and we will no longer designate a specific version of the API to be the default version. Instead, all Workfront API requests must specify a specific API version.

>[!IMPORTANT]
>
> By July 1, 2018 all of your Workfront integrations that use Default must be updated to call a specific supported API version. After that date, all of your Workfront API requests used by integrations that do not specify a version will fail.

To learn about the Workfront deprecation cadence, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

-->

## 將整合更新至支援的API版本

如果您的Workfront API請求未指定版本，則使用預設。 建議您的API請求指定支援的API版本，最好是最新支援的API。

例如，下列Workfront API請求未指定API版本：

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

提出此要求時，您會收到含有JSON編碼文字的回應，此文字會指定來自Workfront例項的資料。 由於此URI中未指定API版本，因此調用將變為預設。

若要將預設API請求轉換為版本化API請求，只需呼叫支援的API版本即可。 例如，以下URI請求版本15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

更新Workfront API請求時，您可以指定任何支援的API版本。 若要進一步了解參考特定API，請參閱 [在您的整合中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

為確保最大支援窗口，您應調用最新版本。 您可以在 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).

## API預設版本的歷史記錄

「預設API」（或「預設」）的原始目的，是將其對應至最新版的Workfront API。 這可讓具有稱為「預設」之基本整合的客戶，永遠不需要更新其API請求。

2011年，Workfront發行了API 3.0版。 預設值會自動移至3.0版，這破壞了許多太複雜而無法使用3.0版而未更新的客戶整合。 因此，Workfront復原了此變更，並將預設版本保留為第2版。

自2011年以來，Workfront已大幅提升API功能。 因此，我們已棄用舊版API。 在2017年，我們完全移除了預設版本的概念，而非更新預設版本。 這是為了鼓勵客戶使用我們穩定版本的API，並在最多三年的週期中維護其整合。

Workfront現在正在重新安裝預設API版本。 預設API設為Workfront API的最新版本，且每次發行新版本時都會更新為最新版本。

