---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 疑難排解 —  [!DNL Workfront Proof] 校對檢視器
description: 如果您的校樣內容未載入，而您只看到空的校樣檢視器，很可能是因為本機有東西阻擋了此動作。 請嘗試下列可能的解決方案。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# 疑難排解 —  [!DNL Workfront Proof] 校對檢視器

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果您的校樣內容未載入，而您只看到空的校樣檢視器，很可能是因為本機有東西阻擋了此動作。 請嘗試下列可能的解決方案。

## 確定您的瀏覽器和 [!DNL Flash Player] 版本為最新

所有開發人員都不斷使用其應用程式，並定期為其產品發行新功能和修正。 這是為了改善使用者體驗並維持安全層級，因此只使用最新版本是最佳作法。 這也有助於避免應用程式之間的衝突。

### [!DNL Flash Player] 外掛程式版本

檢查您當前 [!DNL Flash Player] 版本造訪 [[!DNL Adobe] 網站](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

如果您的版本號碼與平台列出的版本號碼不同，請前往 [[!DNL Flash Player] 下載頁面](http://get.adobe.com/flashplayer/otherversions/) 並取得最新版本。

請注意：建議您使用原始 [!DNL Adobe] 外掛程式，因此若您的瀏覽器使用內建解決方案來停用並安裝 [!DNL Adobe] 解決方案。

### 瀏覽器版本

現在，大多數的瀏覽器都會自動更新，但如果您遇到任何問題，則需要檢查您使用的版本，並視需要執行更新。

在您的瀏覽器中，前往 [!UICONTROL 功能表] 並找到 [!UICONTROL 關於] 選項(在某些情況下，這可能顯示在 [!UICONTROL 說明] 功能表)。 在 [!UICONTROL 關於] 快顯視窗會顯示目前瀏覽器版本的相關資訊，以及更新/檢查更新的選項。

請參閱Chrome:

![ProofView_3.png](assets/proofview-3-350x206.png)

一旦您擁有最新 [!DNL Flash Player] 已安裝的外掛程式和瀏覽器版本會嘗試重新開啟您的校樣，並查看問題是否已解決。

## 確保您的本地 [!DNL Flash] 儲存可用

我們的 [!DNL Workfront Proof] 檢視器是以Flash為基礎，我們會儲存一些校樣的資料(例如，註解、校樣圖磚、 [!DNL Workfront Proof] 檢視器設定)，使用 [!DNL Flash Player]. 若 [!DNL Workfront Proof] 檢視器會開啟，但您內部沒有內容，需要確定Flash儲存可在您的電腦上使用，而且 [!DNL Workfront Proof] 允許使用它。

如果已分配某些儲存空間，但您使用的校樣較大，且有多個頁面，且有留言，會嘗試增加 [!DNL Flash] 儲存並重新載入您的校樣。

請看我們的 [檢視校樣的問題 —  [!DNL Flash] 共用對象說明](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) 以取得詳細指示。

## 確定問題所在

* 校樣會在不同的瀏覽器中開啟嗎？
* 如果您每天使用一個瀏覽器，但在檢視校樣時遇到問題，請嘗試在電腦的其他瀏覽器中開啟相同的校樣。 若要這麼做，只需從主要瀏覽器的URL列複製校樣連結，然後貼到其他瀏覽器中即可。 如果校樣在原處開啟，請檢閱主要瀏覽器組態、外掛程式和擴充功能，因為這些可能會干擾。
* 我們沒有任何偏好的瀏覽器，但如果您目前的瀏覽器出現任何效能問題，建議您切換至其他瀏覽器。
* 校樣會在您所在的不同電腦上開啟嗎？
如果您的校樣未在電腦上的任何瀏覽器中開啟，請嘗試在您所在位置的其他電腦和/或在您所在位置之外開啟。 這可讓您判斷問題是否由您的特定電腦造成，或是由您的本機網路造成。
如果您的安全級別較高，則您與 [!DNL Workfront Proof] 可能被：

   * 您的本地AV軟體
   * 您的網路安全解決方案
   * DNS、防火牆或代理配置
   * 這些是我們無法控制的設定。 有各種可用的安全解決方案，我們無法判斷哪些已在您的網路中實施，哪些可能正在阻止與 [!DNL Workfront Proof]. 也不是 [!DNL Workfront Proof] 決定您的內部安全設定。 如果您在您所在位置/網路的多個電腦上開啟校樣時遇到問題，建議您與您的IT團隊聯繫，以便他們檢查網路設定並授權或新增 [!DNL Workfront Proof] 視需要新增至允許清單。

* 連線是否 [!DNL Workfront Proof] 允許進入您的網路？
我們會在校樣檢視器內載入圖磚 — 頁面的片段。 如果此內容在您的結尾未載入正常，可能是有些連線 [!DNL Workfront Proof] 在您的網路中被阻止。 您將要確認所有連線和*.proofhq.com中的所有內容已新增至允許清單。 您的IT團隊應能協助驗證。

## 檢閱外掛程式

若您的瀏覽器和 [!DNL Flash Player] 外掛程式為最新狀態，且您的網路未封鎖至 [!DNL Workfront Proof] 瀏覽器中可能有影響校樣檢視的項目。 現在，您的瀏覽器中有多個外掛程式和擴充功能可供使用，其中有些會干擾或與其他外掛程式發生衝突。

最佳實務是移除所有未知的附加元件，並僅保留您使用和信任的附加元件。 每個瀏覽器都應提供選項來檢查/修改/刪除外掛程式和擴充功能。 我們的 [!DNL Workfront Proof] 檢視器以 [!DNL Flash] 我們會使用JavaScript來載入檢視器，因此您尤其想要檢閱可能影響這些的外掛程式。

請造訪下列頁面，以取得開發人員關於如何停用瀏覽器附加元件的詳細指示：

* 鉻黃： [外掛程式](https://support.google.com/chrome/answer/142064?hl=en-GB) / [擴充功能](https://support.google.com/chrome/answer/113907?hl=en-GB)
* Firefox: [附加元件](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer: [附加元件](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari: [附加元件](http://support.apple.com/en-gb/HT203353)

如果校樣載入中有任何特定附加元件干擾，您可以嘗試在瀏覽器主控台中檢查詳細資訊。

![ProofView_4.png](assets/proofview-4-350x57.png)

在大多數較新的瀏覽器中，有一些額外的開發人員工具可供使用，可用於更進階的疑難排解。

如果您在查看校樣時遇到問題：

* 開啟瀏覽器的主控台，然後重新載入校樣。
* 檢查主控台中是否有任何警報或訊息。 這些詳細資訊有助於識別問題的根本原因。
* 請您的IT團隊分析結果。 他們應該能夠為解決本地問題提供建議和幫助。
* 與我們的 [支援團隊](https://support.workfront.com/hc/en-us/requests/new). 我們很樂意協助。

如果您不知道如何在瀏覽器中開啟主控台，請參閱錄制的步驟：

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS)
* [Internet Explorer](http://screencast.com/t/bYzq1iQv)
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj)
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

您也可以參閱瀏覽器開發人員的檔案以取得更詳細的指示。

## 檢查混合內容設定

與 [!DNL Workfront Proof] 是透過HTTPS。 不過，在 [!DNL Workfront Proof] 檢視器會透過HTTP載入圖磚，且資料會以代號加以保護。 這會建立混合內容，供某些瀏覽器或安全解決方案封鎖（依預設或依手動設定）。

如果這是校樣未在您的電腦上開啟的原因（您應該可以在瀏覽器控制台中看到相關警報），請授權進行此類連線 [!DNL Workfront Proof] 或者修改設定，允許電腦上的被動混合內容。 您的瀏覽器、AV軟體、網路配置等可能會阻止混合內容，以確定確切原因，請與您的IT團隊/網路管理員聯繫。 他們也應該能協助在您的電腦上啟用混合的內容。

聯繫我們的 [支援團隊](https://support.workfront.com/hc/en-us/requests/new) 如果你需要我們的幫助。
