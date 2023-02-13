---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion案例概觀
description: Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 方案概觀

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 要求 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] 不應將情況與 [!DNL Workfront Scenario Planner] 方案。 如需有關 [!DNL Workfront Scenario Planner] 方案，請參閱 [此 [!DNL Scenario Planner] 概述](../../scenario-planner/scenario-planner-overview.md).

角色 [!DNL Adobe Workfront Fusion] 是讓流程自動化，以便您能夠專注於新任務，而不是反複重複相同的任務。 其運作方式是連結應用程式與服務內及之間的動作，以建立可自動傳輸和轉換資料的案例。 您建立的案例會監視應用程式或服務中的資料，並處理該資料以提供您想要的結果。

案例由一系列模組組成，這些模組指出應如何在應用程式內轉換資料，或在應用程式與網站服務之間傳輸資料。

## 範例：在內自動化流程 [!DNL Adobe Workfront]

>[!NOTE]
>
>此功能適用於下列授權：
>
>* [!UICONTROL [!DNL Workfront Fusion] 工作自動化]
>* [!UICONTROL [!DNL Workfront Fusion] 工作自動化和整合]
>


[!DNL Workfront Fusion] 可讓您在 [!DNL Workfront]，可節省時間並確保程式執行一致。

在此範例中，當中的指定欄位在「任務」或「問題」中變更時，情境就會觸發 [!DNL Workfront]. 觸發時，情境會取得相關專案中的資訊，並為指派給專案上特定角色的人員建立自訂更新。

![](assets/fusion-template-example-350x102.png)

## 範例：連接 [!DNL Workfront] 至其他應用程式或網站服務

>[!NOTE]
>
>此功能適用於下列授權：
>
>* [!UICONTROL [!DNL Workfront Fusion] 工作自動化和整合]
>


[!DNL Workfront Fusion] 也可以連線至其他應用程式和網站服務。 您可以存取、匯入、操控或從其他應用程式匯出資料，將其與Workfront或彼此整合。 許多應用程式都有專用 [!DNL Workfront Fusion] 連接器。 如果沒有要訪問的應用程式的專用連接器，則可以使用 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] 或 [!UICONTROL SOAP] 模組，透過其API連線至應用程式。

在此範例中，當使用者新增至 [!DNL Excel] 試算表。 案例會檢查使用者是否位於 [!DNL Workfront]. 若非如此，藍本會在 [!DNL Workfront] 並將其Workfront使用者ID新增至試算表。

![](assets/fusion-integration-example--350x171.png)

如需專用連接器的清單，請參閱 [應用程式及其模組](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] 幾乎可以連線至任何web服務。 如果您要使用的應用程式沒有專用 [!DNL Workfront Fusion] 連接器中，您可以使用下列模組直接連線至web服務：
>
>* [[!UICONTROL HTTP] 模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] 模組](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] 模組](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

