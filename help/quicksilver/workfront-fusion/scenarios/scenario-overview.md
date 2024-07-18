---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion案例概觀
description: 除了Adobe Workfront授權，Adobe Workfront Fusion還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 27158301e491d4ff45ce7987a81f841fb4525b2a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]個情境總覽

>[!NOTE]
>
>除了[!DNL Adobe Workfront license]之外，[!DNL Adobe Workfront Fusion]還需要[!DNL Adobe Workfront Fusion]授權。

>[!IMPORTANT]
>
>[!DNL Workfront Fusion]案例不應與[!DNL Workfront Scenario Planner]案例混淆。 如需[!DNL Workfront Scenario Planner]個案例的相關資訊，請參閱[ [!DNL Scenario Planner] 概觀](../../scenario-planner/scenario-planner-overview.md)。

[!DNL Adobe Workfront Fusion]的角色是自動化您的程式，以便您可以專注於新任務，而不是一遍又一遍地重複相同的任務。 其運作方式是連結應用程式和服務內外的動作，以建立自動傳輸和轉換資料的情境。 您建立的案例會監視應用程式或服務中的資料，並處理該資料以提供您想要的結果。

案例由一系列模組組成，這些模組會指出應如何在應用程式內轉換資料，或在應用程式和Web服務之間傳輸資料。

## 範例：在[!DNL Adobe Workfront]內自動化處理序

>[!NOTE]
>
>此功能適用於下列授權：
>
>* 工作自動化的[!UICONTROL [!DNL Workfront Fusion]]
>* 工作自動化與整合的[!UICONTROL [!DNL Workfront Fusion]]

[!DNL Workfront Fusion]可讓您在[!DNL Workfront]內自動處理簡單或複雜的工作流程，節省時間並確保程式一致地執行。

在此範例中，當[!DNL Workfront]中的任務或問題中的指定欄位變更時，就會觸發案例。 觸發時，情境會取得相關專案中的資訊，並為專案上特定角色指派的人員建立量身打造的更新。

![](assets/fusion-template-example-350x102.png)

## 範例：正在將[!DNL Workfront]連線至其他應用程式或Web服務

>[!NOTE]
>
>此功能適用於下列授權：
>
>* 工作自動化與整合的[!UICONTROL [!DNL Workfront Fusion]]
>

[!DNL Workfront Fusion]也可以連線到其他應用程式和網頁服務。 您可以存取、匯入、操作或匯出其他應用程式的資料，並將這些資料與Workfront或彼此整合。 許多應用程式都有專用的[!DNL Workfront Fusion]聯結器。 如果您要存取的應用程式沒有專用聯結器，您可以使用[!DNL Workfront Fusion]的[!UICONTROL HTTP]或[!UICONTROL SOAP]模組透過其API連線至應用程式。

在此範例中，將使用者新增到[!DNL Excel]試算表時會觸發此案例。 案例會檢查使用者是否在[!DNL Workfront]中。 如果沒有，情境會在[!DNL Workfront]中建立使用者，並將其Workfront使用者ID新增回試算表。

![](assets/fusion-integration-example--350x171.png)

如需專用聯結器的清單，請參閱[應用程式及其模組](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md)。

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion]可以連線到幾乎任何網路服務。 如果您要使用的應用程式沒有專用的[!DNL Workfront Fusion]聯結器，您可以使用下列模組直接連線至Web服務：
>
>* [[!UICONTROL HTTP]模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP]模組](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON]模組](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
