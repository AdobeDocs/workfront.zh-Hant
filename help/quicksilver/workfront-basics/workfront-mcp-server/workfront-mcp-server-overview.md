---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP伺服器概述
description: 瞭解Adobe Workfront MCP伺服器的功用，以及它如何讓您透過AI代理平台中的自然語言對話使用Workfront。
author: Courtney
feature: Get Started with Workfront
source-git-commit: f96afd17e9f4e726ac545a9cb0c54ace5a4fcffe
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Adobe Workfront MCP伺服器概述

{{highlighted-preview-article-level}}

[!DNL Adobe Workfront] MCP伺服器將您的Workfront執行個體連線到AI代理平台，例如[!DNL Claude]或[!DNL ChatGPT]。 從AI代理平台，您可以透過提出自然語言請求來尋找、建立、更新和管理Workfront專案。

例如，您可以詢問：

* *顯示品牌行銷團隊的所有使用中專案。*
* *更新「設計評論」任務，使其於4月18日完成。*
* *傳送提醒給資產「Spring Campaign影片」上尚未回應的核准者。*

您不需要知道Workfront API或MCP伺服器如何運作，就能使用Workfront MCP伺服器。

>[!IMPORTANT]
>
>目前，Workfront MCP伺服器僅開放美國地區的客戶使用，供使用AWS的客戶使用。

## MCP伺服器是什麼

MCP伺服器是連線點，可讓AI代理平台與其他系統搭配運作。 Workfront MCP伺服器是您的AI代理平台所連線的伺服器，因此可代表您讀取和操作您的Workfront資料。

MCP代表「模型內容通訊協定」。 這是定義AI代理平台和外部系統如何相互交談的標準。

## 設定連線

Workfront MCP伺服器可與任何MCP相容的AI代理程式平台搭配使用，例如[!DNL Claude]或[!DNL ChatGPT]。 在可以使用它之前，需要發生以下情況：

* Workfront管理員必須在您的Workfront執行個體中啟用MCP伺服器存取權。
* 您（或您的管理員）必須將AI代理平台連線至Workfront。

如需詳細資訊，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。

## 開始使用Workfront MCP伺服器

設定後，您可以要求AI代理平台尋找、建立、更新和管理自然語言的Workfront專案。

如需詳細資訊，包括範例要求、注意事項，以及資料與安全性的相關資訊，請參閱[使用Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。