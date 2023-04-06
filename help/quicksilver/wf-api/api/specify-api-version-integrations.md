---
content-type: api
navigation-topic: api-navigation-topic
title: 在您的整合中指定API版本
description: 在您的整合中指定API版本
author: Becky
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 在您的整合中指定API版本

所有Adobe Workfront URI應在URI的「attask/api」部分之後參照API的特定版本。 下列範例呼叫15.0版：

`attask/api/v15.0/<objectName>/<objectId>`

請確認您目前支援的所有整合呼叫Workfront API。

## Workfront API的發行及淘汰排程

新版API會定期發行，通常每年兩次。 每個版本在發行日期後三年內都受支援，且會以過時的狀態再支援一年，雖然有版本提供但不支援。

如需Workfront API的發行順序及淘汰排程的詳細資訊，請參閱 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* API的預設版本已設為最新版本。 任何未指定版本的API呼叫都會使用預設版本。 每次Workfront發行新版API時，預設版本都會更新為最新版本。 **因此，在發行新版Workfront API後，應檢查使用預設版本的任何API呼叫，以確定仍支援該功能。**
>
>* 如果貴組織目前使用預設API，您的Workfront管理員已收到公告中心訊息，其中包含有關預設API的進一步指示。
>
>若要查看最新版的API，請參閱 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).


## 決定您使用的API版本

您可以檢查傳送至Workfront API之HTTP要求的URI，以判斷您使用的API版本。 下列範例顯示指定API 15版的Workfront請求URI:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

如果URI未指定版本，則使用API的預設版本，如以下示例所示：

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> 未在URI中指定API版本的整合會自動路由至API的預設版本。

## 更新整合以使用支援的API版本

當您建立或維護Workfront整合時，應包含可動態更新API版本和其他可能變更的屬性（例如您的API金鑰）的方法。

若要讓更新整合更有效率，您應考慮下列記錄整合值的建議：

* 將值儲存在您持續更新的屬性檔案中，以視未來變更而定
* 建立Web服務以即時管理屬性
* 將屬性值儲存在應用程式可讀取的資料儲存中

在設計Workfront與此整合時，當這些值不可避免地改變時，您便不需要進行大量的開發工作。
