---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 疑難排解 — Mac上校訂檢視器中的介面字型損毀
description: Mac上的校訂檢視器中的通訊錄已損毀的介面字型
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 疑難排解 — Mac上校訂檢視器中的介面字型損毀

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果您發現校訂檢視器未正確顯示介面字型，可能是因為Mac電腦的字型有一些問題。 若要解決問題，請嘗試下列解決方案：

## 移除字型重複專案

檢查系統中是否有任何重複的字型。

1. 關閉您正在使用的瀏覽器。
1. 在「應用程式」資料夾中開啟「字型簿」應用程式。
1. 按一下&#x200B;**[!UICONTROL 所有字型]** (1)。
1. 按一下&#x200B;**[!UICONTROL 編輯]** > **[!UICONTROL 尋找啟用的重複專案]**。

1. 按一下&#x200B;**[!UICONTROL 是]**&#x200B;以解決重複專案。
1. 如果您看到有關損毀字型的警告，請按一下&#x200B;**[!UICONTROL 是]**。
1. 重新啟動電腦。
1. 重試校訂。

## 清除字型快取

有時，Mac OS X中的字型快取會損毀。 例如，當字型或字型系列重新安裝數次，或應用程式已更新或重新安裝時。 除了作業系統的字型快取檔案之外，有些應用程式可能有自己的字型快取。 刪除這些字型快取檔案可以解決亂碼文字的問題。

首先，您必須啟動「字型書」，選取您遇到問題的字型或系列，然後按鍵盤上的「刪除」按鈕。 您也可以按一下滑鼠右鍵並選取[!UICONTROL 移除系列]。 如果您不確定造成問題的字型或系列，建議您先移除重複專案，如上所述。

第二個步驟是清除字型快取，有幾種方法可以達成此目的。

第一個是在啟動時聽到開機鈴聲時，只要按住Shift鍵，即可重新開機進入安全模式。 當此模式載入時，應該會出現進度列，在此期間系統將執行各種檢查和維護常式，其中一個是清除字型快取。

第二種方法是使用「終端機」，可以從管理帳戶中執行下列命令來完成： *sudo atsutil databases -remove*

>[!NOTE]
>
>這個命令會要求您輸入密碼，輸入密碼時不會顯示。 建議您洽詢您的IT部門，因為這可能需要您電腦的管理員許可權。

另一種方法是使用字型快取公用程式（例如FontNuke）並透過其說明清除快取。

許多印前和圖稿/設計工作室也使用Universal Type Server軟體來管理字型的授權和分發。 有時候，Universal Type Server字型快取可能會發生問題，這可能導致[!DNL Workfront Proof]註解消失。

若要修正，請清除Universal Type Server字型快取，然後重新啟動Universal Type Server。

## 修正[!DNL Flash]字型衝突

您可能無法存取此功能，因為它受[!DNL Flash]支援，而大部分環境中已棄用此功能。

舊版校訂檢視器是以[!DNL Flash Player]為基礎，有時當校訂檢視器中遺漏文字時，OS X和[!DNL Flash Player]之間可能會發生字型衝突。 請嘗試下列步驟：

1. 開啟Finder並開啟&#x200B;**[!UICONTROL 執行]**&#x200B;標籤。
1. 按Option鍵( ⌥Alt)以開啟下拉式清單中的[!UICONTROL 資料庫]資料夾。
1. 按住Option鍵的同時，按一下[!UICONTROL 資料庫]資料夾。
1. 在[!UICONTROL 資料庫]資料夾開啟後，移至其中的[!UICONTROL 字型]資料夾。
1. 將[!UICONTROL Fonts]資料夾中的所有字型移至另一個資料夾，也許是在您的案頭上（請勿在Fonts資料夾中建立其他資料夾）。
1. 這個動作會隱藏所有自訂字型；您仍應將標準系統字型儲存在其獨立位置。
1. 結束並重新啟動[!DNL Safari]。
1. 重新開啟校訂。

您現在應該會看到您的字型。 如果您不需要從主目錄移除的任何字型，您可以安全地刪除它們。 否則，請批次處理這些檔案，將其複製回「元件庫/字型」資料夾，然後檢視是哪個檔案造成問題。
