---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 查看校樣時出現問題 — Flash共用對象說明
description: '''注意：本文中的資訊是指目前已過時且將從 [!DNL Workfront] 2018年。 建議您使用新的Web校對檢視器（如Web校對檢視器中的「檢閱校樣」所述）或案頭校對檢視器（如Desktop Pooting檢視器中的「檢閱校樣」所述）。'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f1f3561e-8660-4c1e-b48f-446eb0eaac06
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 檢視校樣的問題 —  [!DNL Flash] 共用對象說明

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>本文中的資訊是指目前已過時且將從 [!DNL Workfront] 2018年。 建議您使用新的網頁校對檢視器(如 [在網路校對檢視器中檢閱校樣](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer))或案頭打樣檢視器(如 [在案頭校對檢視器中檢閱校樣](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer))。

## [!DNL Flash] 共用物件

本機共用物件，有時稱為「[!DNL Flash] cookie，」是資料檔案，可由您造訪的網站在您的電腦上建立。 共用物件最常用來增強您的網頁瀏覽體驗。 A [!DNL Flash] cookie是 [!DNL Adobe Flash] 會從Web伺服器傳送至Web瀏覽器，然後儲存為瀏覽器中的資料檔案。

由於 [!DNL Workfront Proof] 檢視器以 [!DNL Flash]，應該檢查允許的儲存 [!DNL Flash] 應用程式。

## [!DNL Flash] 共用物件 — 已知問題

若 [!DNL Flash] 儲存設定為0 KB，或具有另一個設定，用於塊 [!DNL Flash] 應用程式無法將資料儲存在本機，可能會在 [!DNL Workfront Proof] 查看者：

* 「快速入門」導覽快顯視窗仍持續顯示，不過已選擇不再顯示的選項
* [!DNL Workfront Proof] 檢視器效能會因為校樣中新增的註解數量增加而減慢
* 校樣不會載入，而會得到「灰色畫面」，而非實際影像

## 允許 [!DNL Flash] 共用物件

確保儲存 [!DNL Flash] 電腦上允許共用對象，並且儲存限制不是0。

檢查是否允許共用對象：

1. 在 [!DNL Workfront Proof] 檢視器。
1. 選擇 **[!UICONTROL 全域設定]** 從上下文菜單。
1. 前往 **[!UICONTROL 儲存]** 標籤。
1. 確保 **[!UICONTROL 允許站點在此電腦上保存資訊]** 已選取(1)。
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## 增加 [!DNL Flash] 儲存

依預設 [!DNL Flash] 應用程式可以在用戶的驅動器上儲存多達100 KB的資料，但用戶可以輕鬆修改這些資料。 為眾人提供的解決方案 [!DNL Flash] 相關問題是增加內部 [!DNL Flash] 儲存。 您可以直接從 [!DNL Workfront Proof] 查看者：

1. 開啟校樣。
1. 開啟校樣上的滑鼠右鍵功能表。
1. 按一下 **[!UICONTROL 設定]** 開啟 [!DNL Flash] 設定快顯視窗。
1. 前往 **[!UICONTROL 本地]** 儲存標籤。
1. 將儲存量增加到100 KB(1)。
1. 關閉設定快顯視窗，然後重新開啟校樣。

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)
