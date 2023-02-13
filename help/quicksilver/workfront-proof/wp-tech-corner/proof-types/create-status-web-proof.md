---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: 使用建立靜態網站校樣 [!DNL Workfront Proof]
description: 您可以從網頁建立靜態校樣。 此外，您可定義擷取的螢幕解析度，以模擬各種裝置。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 使用建立靜態網站校樣 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

您可以從網頁建立靜態校樣。 此外，您可定義擷取的螢幕解析度，以模擬各種裝置。

## 建立靜態網站校樣

1. 開啟 [!UICONTROL 新校樣] 頁面，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. 在 **www.shareyourlink.com** 框。
1. 您可以重複此步驟以新增多個URL。
1. 在此框的正下方，按一下解析度（預設為1366x768），然後在 **[!UICONTROL 螢幕解析度]** 框。
如果您想要校樣行動裝置的設計，請選取較小的解析度。 一般而言，設計會根據螢幕/瀏覽器視窗解析度載入。

1. 按一下 **[!UICONTROL 尋找子頁面]** 如果您想要包含與輸入URL位於相同網域/子網域的已連線頁面。
   [!DNL Workfront Proof] 會掃描已連接的頁面，並將其列於 **[!UICONTROL 尋找子頁面]** 選項。 您可以選取要包含的頁面。

1. 使用 [!UICONTROL 合併校樣] 功能，您可以以單一多頁校樣形式提交所有網頁。
1. 按一下 **[!UICONTROL 完成]**，然後完成校樣的設定，如 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 關於需要授權的受密碼保護的頁面和頁面

[!DNL Workfront Proof] 無法將受密碼保護的網站捕獲為靜態校樣。

若要從需要授權的頁面建立校樣，您的IT團隊必須將下列其中一個URL新增至貴公司的允許清單，我們的網頁擷取工具便會透過該允許清單連線：

**AWS在美國的集群**:webcapture.proofhq.com

**美國GCP集群**:webcapture.gcp.proofhq.com

**EMEA集群**:webcapture.proofhq.eu

>[!NOTE]
>
>對於需要授權和受密碼保護的網站的內部頁面，建議進行互動式校對，而非靜態校對。 如需詳細資訊，請參閱 [互動式內容校樣概觀](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## 關於處理靜態網站校樣

* 動畫、內嵌影片、指令碼和互動無法包含在靜態網站校樣中。 如果您想要校樣互動式內容，請參閱 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* 校樣頁面通常以每頁約20秒的速率擷取。 不過，整體準備時間也取決於托管頁面的伺服器。 工具會等待60秒，才載入每個提交的URL。 如果超過此等待時間，校樣會失敗。
* 針對合併校樣，如果任何URL未回應擷取工具，校樣會失敗。
* [!DNL Workfront Proof] 在模擬後擷取長達195英吋的網頁。 如果網頁長度超過此值，校樣會失敗。
* 所有文字元素上都提供文字擷取功能，但置入影像的文字則無法擷取。
* 校樣上可以點選文字超連結，而連結的頁面會在新的瀏覽器分頁中開啟。
* 如果在 `<a>` 標籤。 建議您調整頁面設計的這些部分。
* 為獲得最佳結果，我們建議使用最佳編碼實務和公認的標準來建立頁面。
