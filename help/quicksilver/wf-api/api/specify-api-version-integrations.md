---
content-type: api
navigation-topic: api-navigation-topic
title: 在您的整合中指定API版本
description: 在您的整合中指定API版本
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 在您的整合中指定API版本

在URI的「attask/api」部分之後，所有Adobe Workfront URI都必須參考API的特定版本。 下列範例呼叫7.0版：
`attask/api/v7.0/<objectName>/<objectId>` 請確認您目前支援的所有整合呼叫Workfront API。

## Workfront API的發行及淘汰排程

API的新版本每兩年發行一次，每六至八個月發行一次。 每個版本在發行日期後三年內都受支援，且會以過時的狀態再支援一年，雖然有版本提供但不支援。

如需Workfront API的發行順序及淘汰排程的詳細資訊，請參閱 [API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md).

Workfront自2017年7月起已停用API的預設版本。 這表示Workfront不再指定特定版本的API為預設版本。 所有未來的API URI都必須指定API的版本才能有效。

>[!IMPORTANT]
>
> 任何使用預設API版本的整合都必須在2018年7月1日前更新，以呼叫特定支援的API版本。

## 決定您使用的API版本

您可以檢查傳送至Workfront API之HTTP要求的URI，以判斷您使用的API版本。 下列範例顯示指定API第7版的Workfront請求URI:

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

如果URI未指定版本，則使用API的預設版本，如以下示例所示：

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> 未在URI中指定API版本的整合會自動路由至API的預設版本，並在2018年7月1日後無法運作。

## 更新整合以使用支援的API版本

當您建立或維護Workfront整合時，應包含可動態更新API版本和其他可能變更的屬性（例如您的API金鑰）的方法。

若要讓更新整合更有效率，您應考慮下列記錄整合值的建議：

* 將值儲存在您持續更新的屬性檔案中，以視未來變更而定
* 建立Web服務以即時管理屬性
* 將屬性值儲存在應用程式可讀取的資料儲存中

在設計Workfront與此整合時，當這些值不可避免地改變時，您便不需要進行大量的開發工作。
