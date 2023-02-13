---
content-type: api
navigation-topic: api-navigation-topic
title: 更新使用預設API版本設定的整合
description: 更新使用預設API版本設定的整合
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# 更新使用預設API版本設定的整合

我們每兩年發行一次新版Adobe Workfront API。 每個版本在發行後三年內都受支援，且會在已過時狀態中再多支援一年，此時版本已可供使用但不受支援。

未在URI中指定API版本的整合會自動路由至「預設」（已淘汰）。 您必須在Workfront API請求中指定支援的API版本，才能讓Workfront整合有效。

若要了解如何在API請求中指定版本，請參閱 [在您的整合中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

## 了解API的預設版本

「預設API」（或「預設」）的原始目的，是將其對應至最新版的Workfront API。 這可讓具有稱為「預設」之基本整合的客戶，永遠不需要更新其API請求。

2011年，Workfront發行了API 3.0版。 預設值會自動移至3.0版，這破壞了許多太複雜而無法使用3.0版而未更新的客戶整合。 因此，Workfront復原了此變更，並將預設版本保留為第2版。

很可惜，我們從未再審視此主題，而現在我們計畫大幅增加API功能時，被迫捨棄舊版API，包括預設。 我們並未更新預設版本（這無疑會破壞更多整合），而是完全移除預設版本的概念。 這是為了鼓勵客戶使用我們穩定版本的API，並在最多三年的週期中維護其整合。

## 淘汰預設值

為了改善Workfront API，我們正在移除已超過三年支援期間的舊版API。 其中一個版本是2版，預設值會對應至此版本。 此版本已於2010年發行，而Attask/Workfront應用程式當時支援的大部分邏輯已不存在或已大幅變更。

我們於2017年7月汰除「預設」，將不再指定特定版本的API為預設版本。 所有Workfront API請求都必須指定特定的API版本。

>[!IMPORTANT]
>
> 2018年7月1日前，您所有使用預設的Workfront整合都必須更新，以呼叫特定支援的API版本。 在當天以後，未指定版本的整合所使用的所有Workfront API請求都將失敗。

若要了解Workfront淘汰的過程，請參閱 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).

## 將整合更新至支援的API版本

如果您的Workfront API請求未指定版本，則使用預設。 您必須更新API請求，以指定支援的API版本，最好更新為最新支援的API。

例如，下列Workfront API請求未指定API版本：

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

提出此要求時，您會收到含有JSON編碼文字的回應，此文字會指定來自Workfront例項的資料。 由於此URI中未指定API版本，因此調用將變為預設。

若要將預設API請求轉換為版本化API請求，只需呼叫支援的API版本即可。 例如，以下URI請求版本9:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

更新Workfront API請求時，您可以指定任何支援的API版本。 若要進一步了解參考特定API，請參閱 [在您的整合中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

若要確保最大支援視窗，您應呼叫最新版本（第9版）。 您可以在 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).

您必須更新已使用預設功能的整合。 如果您目前的整合未指定版本，您可能會收到Workfront銷售人員、客戶成功經理、支援代表或公告中心訊息的通知。

請務必盡快更新您的整合，以呼叫我們API的支援版本。
