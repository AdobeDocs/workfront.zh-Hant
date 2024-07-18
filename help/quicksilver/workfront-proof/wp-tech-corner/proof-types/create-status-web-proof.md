---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: 使用 [!DNL Workfront Proof]建立靜態網站校訂
description: 您可以從您的網頁建立靜態校樣。 此外，您可以定義擷取的熒幕解析度來模擬各種裝置。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 使用[!DNL Workfront Proof]建立靜態網站校訂

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

您可以從您的網頁建立靜態校樣。 此外，您可以定義擷取的熒幕解析度來模擬各種裝置。

## 建立靜態網站校訂

1. 開啟[!UICONTROL 新校訂]頁面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校訂中所述。
1. 在&#x200B;**www.shareyourlink.com**&#x200B;方塊中貼上或輸入您的URL。
1. 您可以重複此步驟以新增多個URL。
1. 在此方塊正下方，按一下解析度（預設為1366x768），然後在&#x200B;**[!UICONTROL 熒幕解析度]**方塊中選取您要的任何解析度。
如果您想要校訂行動裝置的設計，請選取較小的解析度。 一般而言，設計會根據熒幕/瀏覽器視窗解析度來載入。

1. 如果您想要包含與輸入的URL位於相同網域/子網域的已連線頁面，請按一下&#x200B;**[!UICONTROL 尋找子頁面]**。
   [!DNL Workfront Proof]會掃描連線的頁面，並在&#x200B;**[!UICONTROL 尋找子頁面]**&#x200B;選項下方列出這些頁面。 您可以選取要包含的頁面。

1. 透過[!UICONTROL 結合校訂]功能，您可以提交所有網頁作為單一多頁校訂。
1. 按一下&#x200B;**[!UICONTROL 完成]**，然後完成設定校訂，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校訂。

## 關於受密碼保護的頁面和需要授權的頁面

[!DNL Workfront Proof]無法擷取受密碼保護的網站做為靜態校訂。

為了從需要授權的頁面建立校樣，您的IT團隊必須將下列URL之一新增到您公司的允許清單，我們的網頁擷取工具即會透過該清單進行連線：

美國&#x200B;**AWS叢集**： webcapture.proofhq.com

在美國&#x200B;**GCP叢集**： webcapture.gcp.proofhq.com

**EMEA叢集**： webcapture.proofhq.eu

>[!NOTE]
>
>我們建議對於需要授權和密碼保護網站的內部頁面，使用互動式校訂，而非靜態校訂。 如需詳細資訊，請參閱[互動式內容校訂總覽](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

## 關於處理靜態網站校樣

* 動畫、內嵌影片、指令碼和互動不能包含在靜態網站校樣中。 如果您想要校訂互動式內容，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校訂中的[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校訂。

* 校樣頁面通常是以每頁約20秒的速率擷取準備。 不過，整體準備時間也取決於託管頁面的伺服器。 工具會等待60秒載入每個提交的URL。 如果超過此等待時間，則校訂失敗。
* 針對合併校樣，如果任何URL未回應擷取工具，校樣就會失敗。
* 點陣化之後，[!DNL Workfront Proof]會擷取長度高達195英吋的網頁。 如果網頁超過此長度，則校訂失敗。
* 文字擷取可用於所有文字元素，但置入為影像的文字不會擷取。
* 校樣上可點選文字超連結，而且連結的頁面會在新的瀏覽器分頁中開啟。
* 如果在`<a>`標籤內使用了style=&quot;display：block&quot;元素，則無法點選影像上的超連結。 我們建議您調整頁面設計的這些部分。
* 為獲得最佳結果，我們建議使用最佳編碼實務和公認的標準來建立頁面。
