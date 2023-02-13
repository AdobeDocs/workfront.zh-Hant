---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 速度問題 [!DNL Workfront Proof]
description: 此說明頁面可協助您判斷使用時是否遇到任何速度問題 [!DNL Workfront Proof] 與您的ISP或 [!DNL Workfront Proof]的內容傳遞網路。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# 速度問題 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

此說明頁面可協助您判斷使用時是否遇到任何速度問題 [!DNL Workfront Proof] 與您的ISP或 [!DNL Workfront Proof]的內容傳遞網路。

速度問題通常是由於本地ISP連接或本地Internet訪問設定（例如，使用代理伺服器），因此不幸地，速度問題不在於 [!DNL Workfront Proof].

也就是說，您可以執行一些步驟來檢查連線速度，以便確定您遇到的問題的根本原因。 所有這些步驟對於故障排除過程同樣重要，我們鼓勵您花時間收集有關所列步驟的資訊，以確保對問題進行最準確的診斷。

收集所有詳細資訊後，我們建議您洽詢當地IT部門，以找出任何當地問題。 若您在此事上需要進一步協助，請聯絡我們的 [支援團隊](https://support.workfront.com/hc/en-us/requests/new).

## 確定系統的哪個部分速度慢

使用 [!DNL Workfront Proof]，您可能會使用「控制面板」，例如管理資料夾內容和使用者，或使用 [!DNL Workfront Proof] 查看者：進行證明審查、檢查已發表的評論等。

確定系統的哪個確切部分速度較慢是診斷速度問題的第一步。 報告時 [!DNL Workfront Proof] 速度緩慢，請務必說明下列內容：

* 您在其他任何網頁中都遇到速度緩慢嗎？
* 問題是否發生在控制面板或 [!DNL Workfront Proof] 觀眾？
* 系統的哪個部分確實很慢？ (例如處理新校樣或在 [!DNL Workfront Proof] 檢視器)

## 執行traceroute和ping測試

遇到效能問題時，請務必運行traceroute命令以驗證連接。 要執行此操作，請開啟系統中的命令提示符(Mac/Linux中的終端機)，然後執行以下步驟：

1. 鍵入以下選項之一，然後等待跟蹤完成：

   * 窗口： **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. （僅限Windows）類型 **ping app.proofhq.com**.
1. Ping完成後，在命令提示符中按一下右鍵，然後選擇全部。
1. 將結果複製並貼到您電子郵件的回覆中。
在將結果發送給支援團隊之前，請確保允許traceroute和ping完成。

## 使用Speedtest.net測試連線速度

1. 按一下 [此處](http://www.speedtest.net/) 來存取Speedtest.net。
1. 請按照Speedtest知識庫中的說明測試您的網際網路連線速度。
1. 將結果複製並貼到我們的支援團隊的電子郵件中。

## 在瀏覽器主控台中檢查網路標籤

現代瀏覽器中可用的Web控制台會收集有關任何網路延遲的有用資訊，這將有助於我們確定您遇到的速度問題的根本原因。

檢查網頁的載入時間：

1. 開啟瀏覽器的主控台，並開啟「網路」標籤。
1. 重新載入頁面。
1. 拍攝螢幕截圖或錄制結果的螢幕截圖。
1. 與支援團隊共用結果。

請確保螢幕截圖顯示所有資料 — 您可以在拍攝螢幕截圖時展開控制台窗口，或在螢幕截圖中向下滾動。

如果您不知道如何在瀏覽器中開啟主控台，請參閱以下錄制的步驟：

* [鉻黃](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Edge](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer](http://screencast.com/t/x5Q3eHczbc)

您也可以檢閱瀏覽器的檔案，以取得更詳細的指示。

## 在不同的網路和電腦上檢查您的連接

使用不同的設備或網路檢查連接速度是否遇到相同問題是故障排除過程中的關鍵步驟。 請嘗試切換至其他電腦或行動裝置，並嘗試使用替代網路（例如行動資料）。

比較不同組合中的連線：在同一網路上使用不同的電腦，在不同網路上使用同一台電腦，並同時使用替代電腦和網路，然後與支援團隊共用結果。
