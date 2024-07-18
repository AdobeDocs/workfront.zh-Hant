---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: ' [!DNL Workfront Proof]中的速度問題'
description: 此說明頁面可協助您判斷在使用 [!DNL Workfront Proof] 時可能會遇到的任何速度問題，是否與您的ISP或 [!DNL Workfront Proof]的內容傳遞網路有關。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# [!DNL Workfront Proof]中的速度問題

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

此說明頁面可協助您判斷在使用[!DNL Workfront Proof]時可能會遇到的任何速度問題，是否與您的ISP或[!DNL Workfront Proof]的內容傳遞網路有關。

速度問題通常是因為本機ISP連線或本機網際網路存取設定（例如，使用Proxy伺服器的情況）所造成，因此很遺憾，這不在[!DNL Workfront Proof]的控制範圍之內。

話雖如此，您可以採取一些步驟來檢查連線速度，以找出您遇到的問題的根本原因。 所有這些步驟對於疑難排解流程同樣重要，建議您花一些時間收集列出的所有步驟的相關資訊，以確保對問題進行最準確的診斷。

收集所有詳細資料後，建議您洽詢當地IT部門，找出任何當地問題。

## 確定系統的哪個部分速度較慢

當您使用[!DNL Workfront Proof]時，您可能會使用控制面板，例如，管理資料夾內容和使用者，或使用[!DNL Workfront Proof]檢視器：進行校訂檢閱、檢查已發表的評論等。

判斷系統哪個部分速度較慢，是疑難排解速度問題的第一步。 當您報告[!DNL Workfront Proof]速度緩慢時，請務必說明下列事項：

* 您是否在其他網頁上遇到速度變慢的問題？
* 問題是否在儀表板或[!DNL Workfront Proof]檢視器中發生？
* 系統的哪個部分速度較慢？ （例如，處理新校訂或在[!DNL Workfront Proof]檢視器中開啟評論）

## 執行traceroute和ping測試

當您遇到效能問題時，請務必執行traceroute命令以驗證連線。 若要這麼做，請在您的系統中開啟命令提示字元(Mac/Linux中的終端機)，然後執行下列步驟：

1. 輸入下列其中一項，然後等待追蹤完成：

   * Windows： **tracert app.proofhq.com**
   * Mac/Linux： **traceroute app.proofhq.com**

1. （僅限Windows）型別&#x200B;**ping app.proofhq.com**。
1. Ping完成時，在命令提示字元中按一下滑鼠右鍵，然後選取全部。
1. 將結果複製並貼到您電子郵件的回覆中。
在將結果傳送給支援團隊之前，請務必允許traceroute和ping完成。

## 使用Speedtest.net測試連線速度

1. 開啟瀏覽器並前往Speedtest.net。
1. 請依照Speedtest知識庫的指示，測試網際網路連線的速度。
1. 將結果複製並貼到我們的支援團隊的電子郵件中。

## 檢查瀏覽器主控台中的網路索引標籤

現代瀏覽器提供的Web主控台會收集任何網路延遲的實用資訊，這些資訊可協助我們判斷造成您速度問題的根本原因。

若要檢查網頁的載入時間：

1. 開啟瀏覽器的主控台和Network標籤。
1. 重新載入頁面。
1. 拍攝熒幕擷取畫面或錄製結果的熒幕擷取畫面。
1. 將結果分享給支援團隊。

請確定熒幕擷圖顯示所有資料 — 您可以在擷取熒幕擷圖時展開主控台視窗，或在熒幕擷圖中向下捲動。

您也可以檢查瀏覽器的檔案，以取得更詳細的指示。

## 檢查您在不同網路和電腦上的連線

檢查您是否在使用不同裝置或網路的連線速度方面遇到相同的問題，是疑難排解過程中的關鍵步驟。 請嘗試切換到不同的電腦或行動裝置，並嘗試使用替代網路（例如行動資料）。

比較不同組合的連線：使用相同網路上的不同電腦、使用不同網路上的相同電腦，以及同時使用其他電腦和網路，然後與支援團隊分享結果。
