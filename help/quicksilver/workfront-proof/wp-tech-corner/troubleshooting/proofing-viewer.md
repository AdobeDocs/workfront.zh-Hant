---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 疑難排解 —  [!DNL Workfront Proof] 校訂檢視器
description: 如果您的校訂內容未載入，而您只能看到空白的校訂檢視器，則很可能是因為有某些專案在本機阻止了此動作。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 39fdf5c2c2114a82c48f515c4a9f088596394045
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# 疑難排解 — [!DNL Workfront Proof]校訂檢視器

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果您的校訂內容未載入，而您只能看到空白的校訂檢視器，則很可能是因為有某些專案在本機阻止了此動作。 嘗試下列可能的解決方案。

## 確保您的瀏覽器<!--and [!DNL Flash Player]-->版本為最新版本

所有開發人員都會持續開發應用程式，並定期發佈產品的新功能和修正專案。 這是為了改善使用者體驗並維持安全性等級，所以最佳實務是隻使用最新版本。 這也有助於避免應用程式之間的衝突。

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### 瀏覽器版本

通常大部分的瀏覽器都會自動更新，但如果您遇到任何問題，則應檢查您使用的版本，並在需要時執行更新。

在瀏覽器中，移至[!UICONTROL 功能表]並找到[!UICONTROL 關於]選項（在某些情況下，這可能顯示在[!UICONTROL 說明]功能表下）。 在[!UICONTROL 關於]快顯視窗中，您可以找到有關目前瀏覽器版本的資訊，以及更新/檢查更新的選項。

例如，在Chrome中：

![Chrome瀏覽器版本](assets/proofview-3.png)

安裝最新瀏覽器版本後，請嘗試重新開啟校樣，並檢視問題是否已解決。

<!--

## Ensure Your Local [!DNL Flash] Storage is Available

Our [!DNL Workfront Proof] Viewer is based on Flash, and we store some data about the proofs (i.e., comments, proof tiles, [!DNL Workfront Proof] Viewer settings) on your computer using [!DNL Flash Player]. If the [!DNL Workfront Proof] Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that [!DNL Workfront Proof] is allowed to use it.

If there is some storage allocated, but you're working with the bigger proofs with multiple pages and comments try to increase the [!DNL Flash] Storage and re-load your proof.

-->

## 找出問題所在

* 校樣會在不同的瀏覽器中開啟嗎？
* 如果您每天使用一個瀏覽器，並且無法在該處檢視校訂，請嘗試在電腦上的不同瀏覽器中開啟相同的校訂。 若要這麼做，只要從主要瀏覽器的URL列複製校樣連結，然後貼到其他瀏覽器中即可。 如果校樣在此處開啟，請檢閱您的主要瀏覽器設定、外掛程式和擴充功能，因為這些可能會造成干擾。
* 我們沒有任何偏好的瀏覽器，但如果您目前瀏覽器發生任何效能問題，建議您切換至其他瀏覽器。
* 校樣會在您所在位置的不同電腦上開啟嗎？
如果您的校訂未在電腦上的任何瀏覽器中開啟，請嘗試在您所在位置和/或您所在位置之外的其他電腦上開啟校訂。 這可讓您判斷您的特定電腦上是否有問題，或問題是否位於您的本機網路中。
如果您的安全性等級較高，您與[!DNL Workfront Proof]的連線可能會遭到下列封鎖：

   * 您的本機AV軟體
   * 您的網路安全性解決方案
   * DNS、防火牆或Proxy設定
   * 這些設定超出我們的控制範圍。 有多種可用的安全性解決方案，我們無法辨別哪些方案在您的網路中實作，哪些方案可能封鎖與[!DNL Workfront Proof]的連線。 決定您內部安全性設定的條件也不是[!DNL Workfront Proof]。 如果您在位置/網路中的多部電腦上開啟校訂時發生問題，建議您連絡您的IT團隊，以便他們檢查網路設定並視需要授權或將[!DNL Workfront Proof]新增至允許清單。

* 您的網路是否允許連線至[!DNL Workfront Proof]？
在校訂檢視器內，我們載入圖磚 — 頁面片段。 若此內容在您的終端未正確載入，您的網路中可能會封鎖某些與[!DNL Workfront Proof]的連線。 請確定所有連線和來自*.proofhq.com的內容均已新增至允許清單。 您的IT團隊應能協助確認此事項。

## 檢閱外掛程式

如果您的瀏覽器是最新版本，且您的網路未封鎖與[!DNL Workfront Proof]的連線，則您的瀏覽器中可能會出現影響檢視校樣的問題。 您的瀏覽器通常有多個可用的外掛程式和擴充功能，其中有些可能會干擾或與其他外掛程式衝突。

最佳實務是移除所有未知的附加元件，僅保留您使用且您信任的附加元件。 每個瀏覽器都應提供選項，讓您檢查/修改/刪除外掛程式和擴充功能。 我們使用JavaScript載入[!DNL Workfront Proof]檢視器，因此您特別想要檢閱可能影響該檢視器的外掛程式。

如果載入校樣有任何特定的附加元件干擾，可以嘗試在瀏覽器的主控台中檢視詳細資訊。

![瀏覽器主控台](assets/proofview-4.png)

在大多數較新的瀏覽器中，有一些其他可用的開發人員工具，可用於更進階的疑難排解。

如果您無法檢視校樣：

* 開啟瀏覽器的主控台，然後重新載入校訂。
* 檢查主控台中是否有任何警示或訊息。 這些詳細資訊有助於確定問題的根本原因。
* 請您的IT團隊分析結果。 他們應該能夠提出建議並幫助解決本機問題。
* 請與我們的支援團隊分享結果。 我們很樂意提供協助。

## 檢查混合內容設定

所有與[!DNL Workfront Proof]的連線都是透過HTTPS進行。 不過，在[!DNL Workfront Proof]檢視器中，我們會透過HTTP載入圖磚，且資料會受權杖保護。 這會建立混合式內容，而有些瀏覽器或安全性解決方案可能會封鎖此內容（根據預設或手動設定）。

如果這是電腦上未開啟校訂的原因（您應該可以在瀏覽器的主控台中看到相關警示），請授權[!DNL Workfront Proof]的此類連線，或修改您的設定，以允許電腦上的被動混合式內容。 您的瀏覽器、AV軟體或網路組態可能會封鎖混合式內容，以判斷確切的原因。 您應該連絡您的IT團隊/網路管理員。 他們應該還能協助在您的電腦上啟用混合式內容。


