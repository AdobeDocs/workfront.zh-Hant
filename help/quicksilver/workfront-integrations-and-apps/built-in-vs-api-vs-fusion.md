---
content-type: reference
product-area: workfront-integrations
keywords: 原生，ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront整合方法
description: 您可以整合 [!DNL Adobe Workfront] 協力廠商應用程式。 這些整合可擴充 [!DNL Workfront] 並根據貴組織的需求量身打造。 您可以使用任何或所有這些整合，視哪些功能對指定任務最有用而定。
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Adobe Workfront整合方法

您可以整合 [!DNL Adobe Workfront] 協力廠商應用程式，以及其他 [!DNL Adobe] 產品。 這些整合可擴充 [!DNL Workfront] 並根據貴組織的需求量身打造。 您可以使用任何或所有這些整合，視哪些功能對指定任務最有用而定。

## 內建整合

Workfront提供多種整合功能，您可以直接從Workfront，或透過安裝該應用程式的Workfront增益集，從其他應用程式進行設定。 這些內建整合涵蓋許多常見的使用案例案例，並著重於為使用者擴充和連接使用者體驗。

Workfront內建的整合主要專注於個人生產力和協作。 這些整合可減少個別使用者工作流程中的中斷，讓他們可接收Workfront通知、存取資訊，以及在Workfront工作項目上執行作業，而不需離開整合式應用程式。

內建整合的優點可能包括：

* 許多內建整合功能均免費提供。 （其他則需要額外購買。）
* 內建整合涵蓋許多企業最常使用的應用程式，例如 [!DNL Slack], [!DNL Google Drive]，或 [!DNL Adobe] 產品，例如 [!DNL Adobe Creative Cloud] 或 [!DNL Adobe Experience Manager] 資產。 如果貴公司已使用這些應用程式，整合將順利進入使用者的現有工作流程。
* 整合 [!DNL Workfront] 使用常用的應用程式可提高使用者的採用率。

>[!INFO]
>
>**範例:**
>
>使用 [!DNL Workfront for Microsoft Teams integration]，您可在 [!DNL Microsoft Teams] 關於 [!DNL Workfront] 工作項目。 不離開 [!DNL Microsoft Teams]，您可以執行批准、注釋或更改工作項目狀態等操作。 您對工作項目所做的任何變更 [!DNL Microsoft Teams] 反映於 [!DNL Workfront] 還有。

如需內建整合的詳細資訊，包括目前可用的內建整合清單，請參閱 [[!DNL Adobe Workfront] 內建整合概觀](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## 自訂OAuth2應用程式

Adobe [!DNL Workfront] 管理員可以為您的執行個體建立OAuth2應用程式 [!DNL Workfront]，允許其他應用程式存取 [!DNL Workfront]. 然後，您的使用者就可以授予其他應用程式存取其 [!DNL Workfront] 資料。 如此一來，您就能將Workfront與您所選擇的應用程式整合，包括您自己的內部應用程式。

>[!NOTE]
>
>在OAuth2的內容中，「建立應用程式」是指在應用程式和伺服器(例如Workfront)之間建立此類存取連結的程式。

建立 [!UICONTROL OAuth2] 申請可包括下列內容：

* 使用者可直接在 [!DNL Workfront]，類似內建整合。
* 設定或使用 [!UICONTROL OAuth2] 應用程式不需要額外的技術知識，例如熟悉 [!DNL Workfront] API。
* 貴組織可能會使用未提供 [!DNL Workfront] 內建應用程式。 您仍可將此軟體與 [!DNL Workfront] 使用 [!UICONTROL OAuth2] 應用程式，即使軟體是貴組織的專有軟體。

如需詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] 提供公用API（應用程式程式設計介面），可讓您擴充及增強Workfront體驗。 目標 [!DNL Workfront] API可簡化建立您與 [!DNL Workfront] 通過HTTP運行的REST風格體系結構。 此 [!DNL Workfront] API確實需要一些技術知識，但是它是一種非常強大的工具，可用於擷取、建立和修改資料。 您可以自訂API呼叫，以執行非常特定的功能。

此外， [!DNL Workfront] 提供事件訂閱API。 當在 [!DNL Workfront] 事件訂閱支援的物件，您可以設定 [!DNL Workfront] 以傳送回應至您想要的端點。 這表示第三方應用程式可接收來自 [!DNL Workfront] 透過 [!DNL Workfront] API發生之後不久。

使用的優點 [!DNL Workfront] API可能包括下列項目：

* 您可以使用 [!DNL Workfront] API，可連線至幾乎任何其他提供公用API的網站服務或應用程式。 因此，可以整合 [!DNL Workfront] 使用您想要使用的幾乎任何網站服務或應用程式。
* 此 [!DNL Workfront] API的彈性也延伸至您企業的專屬軟體。 您可以使用和修改 [!DNL Workfront] 從您自己的軟體內取得資料。
* 由於API在軟體中是如此常見，因此您的內部開發人員很可能熟悉它們。 [!DNL Workfront] 使用最常見的API類型RESTful API，讓開發人員更容易快速上手。

>[!INFO]
>
>**範例:**
>
>下列API呼叫會以指定ID將註解放入任務的更新資料流中。
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

如需 [!DNL Workfront] API，請參閱 [API基本介紹](../wf-api/general/api-basics.md).

如需事件訂閱的詳細資訊，請參閱 [事件訂閱API](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] 可讓您自動化工作流程。 使用 [!DNL Workfront Fusion for Work Automation and Integration] 許可證，您可以跨多個應用程式和web服務建立這些自動化，從而建立應用程式協同工作以執行任務的情況。 案例是使用模組構建的任務或工作流的可視化表示，這些模組是離散任務，如「下載文檔」或「建立項目」。 您可以將模組連結在一起以定義工作流程，然後在符合觸發條件時自動執行工作流程。

優勢 [!DNL Workfront Fusion] 可能包括下列項目：

* [!DNL Workfront Fusion] 不需要像API那麼多的技術知識，因為視覺化介面有助於了解和設定工作流程。 這表示開發團隊以外的個人可以使用它，這樣可以節省組織的時間和金錢。
* 自 [!DNL Workfront Fusion] 可透過API運作，存取大部分應用程式和網站服務。 許多應用程式都有可進行API呼叫的模組，或者您可以使用HTTP、SOAP或JSON模組，來與沒有專用的網站服務互動 [!DNL Workfront Fusion] 連接器。

>[!INFO]
>
>**範例:**
>
>以下 [!DNL Workfront] 模組 [!DNL Workfront Fusion] 已設定，以將註解新增至選取的專案。 執行模組後，註解會顯示在Workfront中專案的更新資料流中。
>
>![](assets/fusion-example-comment-350x416.png)

如需 [!DNL Workfront Fusion]，請參閱 [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
