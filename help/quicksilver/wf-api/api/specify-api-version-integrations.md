---
content-type: api
navigation-topic: api-navigation-topic
title: 在您的整合中指定API版本
description: 在您的整合中指定API版本
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 在您的整合中指定API版本

所有Adobe Workfront URI都應該在URI的「attask/api」部分後面參照特定的API版本。 下列範例會呼叫15.0版：

`attask/api/v15.0/<objectName>/<objectId>`

請確定您的所有整合功能都會呼叫目前支援的Workfront API。

## Workfront API的發行與淘汰排程

新版本的API會定期發佈，通常每年發佈兩次。 每個版本在發行日期後三年內都受到支援，但在有版本提供但不支援的已棄用狀態下，還會額外支援一年。

如需Workfront API發行順序和淘汰排程的詳細資訊，請參閱[API版本設定和支援排程](../../wf-api/api/api-version-support-schedule.md)。

>[!IMPORTANT]
>
>* API的預設版本設定為最新版本。 任何未指定版本的API呼叫都將使用預設版本。 每當Workfront發行新版API時，預設版本都會更新至最新版本。 **因此，在發行新版本的Workfront API之後，應該檢查使用預設版本的任何API呼叫，以確定仍然支援該功能。**
>
>* 如果您的組織目前正在使用預設API，您的Workfront管理員已收到Announcement Center訊息，提供有關預設API的更多說明。
>
>若要檢視API的最新版本，請參閱[API版本設定與支援排程](../../wf-api/api/api-version-support-schedule.md)。


## 判斷您使用的API版本

您可以檢查傳送至Workfront API的HTTP請求URI，藉此判斷您使用的API版本。 以下範例顯示指定API版本15的Workfront請求URI：

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

如果URI未指定版本，則會使用API的預設版本，如下列範例所示：

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> 未在URI中指定API版本的整合會自動路由傳送到該API的預設版本。

## 更新整合以使用支援的API版本

當您建立或維護Workfront整合時，應該包含動態更新API版本和其他可變屬性（例如您的API金鑰）的方法。

若要讓更新整合更有效率，您應該考慮下列建議來記錄整合值：

* 將值儲存在您保持更新的屬性檔案中，以備將來有所變更
* 建立Web服務以即時管理屬性
* 將屬性值儲存在應用程式可讀取的資料存放區中

針對此需求設計Workfront整合，可在值不可避免地變更時，降低大量開發工作的需求。
