---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用AI產生模組
description: 您可以輸入文字提示，以建立設定為提示的HTTP模組。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 1%

---

# 使用AI產生模組

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>由於此功能仍處於開發初期，因此僅供內部Workfront使用者使用。

您可以使用AI輸入文字提示，說明您需要模組做什麼。 然後Fusion將產生HTTP模組，該模組將連線到所需API的正確端點。

和從AI產生的任何專案一樣，我們建議您仔細檢查並測試產生的模組，以確保模組如預期般執行。

## 目前支援的AI模組應用程式

Fusion AI目前可以產生連線到以下應用程式的模組：

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Adobe大師
* Adobe Analytics
* Adobe PDF服務
* AdobeMarketo
* AdobeFrame.io
* Dropbox
* NetSuite
* Google 日曆
* 阿特拉斯大Jira
* GitLab
* Spotify
* 位元貯體
* OpenAI
* Slack

## 產生模組

1. 新增模組並從應用程式清單中選取&#x200B;**使用AI產生**。

   或

   在案例編輯器的空白區域上按一下滑鼠右鍵，然後選取&#x200B;**使用AI產生**。
1. 在方塊中輸入文字提示。

   如需提示的相關提示，請參閱本文中的[建立文字提示的提示](#tips-for-creating-text-prompts)。
1. 將應用程式的API Token新增至模組。
1. 檢查模組，確保模組已針對適當的應用程式和動作進行設定。
1. （視條件而定）如果模組未附加至您的案例，請將其拖曳至適當位置。

我們建議測試模組，以確保產生的模組如預期般執行。

## 建立文字提示的提示

文字提示應至少包含下列資訊：

* 您連線到的應用程式
* 您要執行的動作

>[!INFO]
>
>**範例**：
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   這包括應用程式`Google Calendar`和動作`Retrieve a list of my calendars`。
>
>* `Retrieve popular songs from Spotify`
>
>   這包括應用程式`Spotify`和動作`Retrieve popular songs`。

建立文字提示時，請考量下列事項：

* 由於每個Fusion模組會執行單一動作，因此您的文字提示應說明一個特定動作。
* 使用直接、簡單的語言。
* 檢查並測試您的模組。 如果無法如預期執行，請調整您的提示，然後再試一次。
