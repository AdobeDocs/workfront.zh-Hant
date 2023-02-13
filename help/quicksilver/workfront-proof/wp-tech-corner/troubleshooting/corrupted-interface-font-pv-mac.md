---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 疑難排解 — Mac上校對檢視器的介面字型損毀
description: 如果您發現校對檢視器未正確顯示介面字型，這可能是因為Mac電腦上的字型有一些問題。 要解決此問題，請嘗試下列解決方案 — 編輯我。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 疑難排解 — Mac上校對檢視器的介面字型損毀

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果您發現校對檢視器未正確顯示介面字型，這可能是因為Mac電腦上的字型有一些問題。 要解決問題，請嘗試以下解決方案：

## 刪除字型重複項

檢查系統中是否有任何重複字型。

1. 關閉您使用的瀏覽器。
1. 在「應用程式」資料夾中開啟「字型手冊」應用程式。
1. 按一下 **[!UICONTROL 所有字型]** (1)。
1. 按一下 **[!UICONTROL 編輯]** > **[!UICONTROL 查找已啟用的重複項]**.

1. 按一下 **[!UICONTROL 是]** 來解析重複項目。
1. 如果您看到有關損壞字型的警告，請按一下 **[!UICONTROL 是]**.
1. 重新啟動電腦。
1. 重試校樣。

## 清除字型快取

有時，Mac OS X中的字型快取會損毀。 例如，如果字型或字型系列重新安裝了多次，或者應用程式已更新或重新安裝。 除了作業系統的字型快取檔案外，某些應用程式可能有自己的字型快取。 刪除這些字型快取檔案可解決亂碼文字的問題。

首先，您需要啟動字型簿，選擇您遇到問題的字型或系列，然後按鍵盤上的「刪除」按鈕。 您也可以按一下滑鼠右鍵並選取 [!UICONTROL 刪除系列]. 如果您不確定導致問題的字型或系列，可以嘗試先移除重複項目，如上所述。

第二步是清除字型快取，並有數種方法可達成此目的。

第一種是，在啟動時聽到啟動響鈴時，立即按住Shift鍵，將其重新啟動到安全模式。 當此模式載入時，應會顯示進度欄，在此期間，系統將運行各種檢查和維護常式，其中一個常式是清除字型快取。

第二種方法是使用終端機，這可從管理帳戶內執行下列命令來完成： *sudo atsutil資料庫 — remove*

>[!NOTE]
>
>此命令將要求您輸入密碼，鍵入時不會顯示密碼。 建議您與IT部門諮詢，因為這可能需要您電腦的管理員權限。

另一種方法是使用字型快取實用程式（如FontNuke），並在其幫助下清除快取。

許多印前和印刷/設計工作室也使用通用類型伺服器軟體來管理字型的許可和分發。 有時，通用類型伺服器字型快取可能會發生問題，而可能導致 [!DNL Workfront Proof] 註解消失。

要修復，請清除通用類型伺服器字型快取並重新啟動通用類型伺服器。

## 修正 [!DNL Flash] 字型衝突

您可能無法存取此功能，因為受支援 [!DNL Flash]，此功能已在大部分環境中淘汰。

舊版校對檢視器以 [!DNL Flash Player] 有時，當校對檢視器中缺少文字時，OS X和之間可能會發生字型衝突 [!DNL Flash Player]. 請嘗試下列操作：

1. 開啟Finder並開啟 **[!UICONTROL 開始]** 標籤。
1. 按Option鍵(Alt⌥)開啟 [!UICONTROL 程式庫] 下拉式清單中的資料夾。
1. 按住Option鍵時，按一下 [!UICONTROL 程式庫] 檔案夾。
1. 在 [!UICONTROL 程式庫] 資料夾開啟，轉到 [!UICONTROL 字型] 檔案夾。
1. 移動位於 [!UICONTROL 字型] 資料夾放入另一個資料夾（也許在案頭上）（請勿在「字型」資料夾內建立另一個資料夾）。
1. 此動作會隱藏所有自訂字型；您仍應將標準系統字型儲存在其獨立位置。
1. 退出並重新啟動 [!DNL Safari].
1. 重新開啟校樣。

你應該看看你的字型。 如果您不需要從主目錄中刪除的任何字型，可以安全地刪除這些字型。 否則，分批逐次瀏覽，將它們複製回Library/Fonts資料夾，然後查看是哪個資料夾導致了問題。
