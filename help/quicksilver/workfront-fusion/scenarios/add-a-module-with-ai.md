---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用AI產生案例區段
description: 您可以輸入文字提示，以建立設定為提示的HTTP模組。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 7013c8a88f047c5c8e769a4d7b71f2033c767b4a
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# 使用AI產生案例區段

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>由於此功能位於Beta中，因此僅供部分Workfront使用者使用。

您可以使用AI輸入文字提示，說明您需要將情境的某個區段執行哪些操作。 然後Fusion將產生模組來執行這些動作，您可在場景中使用。

和從AI產生的任何專案一樣，我們建議您仔細檢查並測試產生的模組，以確保模組如預期般執行。

## 目前支援的AI模組應用程式

Fusion AI目前可以產生連線到以下應用程式的模組：

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Adobe Workfront規劃
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

1. 開始新增模組，並從應用程式清單中選取&#x200B;**使用AI產生**。

   或

   按一下案例編輯器頁面底部附近的「使用AI產生」圖示![使用AI產生](assets/generate-with-ai-icon-beta.png)。

   該AI助理面板隨即開啟。
1. 在方塊中輸入文字提示。

   如需提示的相關提示，請參閱本文中的[建立文字提示的提示](#tips-for-creating-text-prompts)。

   模組或模組集隨即產生。
1. （視條件而定）如有需要，請將應用程式的API Token新增至模組。
1. 檢查模組，確保針對適當的應用程式和動作來設定它們。
1. （視條件而定）如果產生的案例區段未附加至您的案例，請將其拖曳至適當位置。

我們建議測試這些模組，以確保它們按預期執行。

## 建立文字提示的提示

文字提示應至少包含下列資訊：

* 您連線到的應用程式
* 您要執行的一個或多個動作

>[!IMPORTANT]
>
>您可以一次產生多個模組，但一次只能為一個應用程式產生模組。

>[!INFO]
>
>**範例**：
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>這包括應用程式`Workfront Planning`和動作`delete records`。 此提示會建立三個模組，每個要刪除的記錄各一個。
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>這包括應用程式`Workfront Planning`和動作`change campaign summary`。
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>這包括應用程式`Workfront Planning`和動作`get field details`。
>
>下列範例不正確：
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    此範例不正確，因為它包含多個應用程式

建立文字提示時，請考量下列事項：

* 使用直接、簡單的語言。
* 檢查並測試您的模組。 如果無法如預期執行，請調整您的提示，然後再試一次。
