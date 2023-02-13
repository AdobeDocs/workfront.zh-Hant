---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 方案，效能
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront融合效能護欄
description: Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 效能護欄

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 要求 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront license].

工作自動化需要快速處理，因此 [!DNL Adobe Workfront Fusion] 專為高效能而設計。 由於長期的情況會減慢您的工作速度，我們設計了 [!DNL Workfront Fusion] 具有效能保護護欄，可限制執行時間、資料大小和其他方案參數。 [!DNL Workfront Fusion] 設計人員應該注意這些護欄，並將它們納入其設計實踐。

## 情景

* 預設方案執行逾時為 **40分鐘**. 執行達到此逾時時， [!DNL Workfront Fusion] 根據情境，在下一個週期或操作之後中斷情境執行。 這會強制在達到40分鐘限制後不久停止情境
* 藍圖的最大大小為 **5 MB**，但建議將藍本大小保持在 **3 MB**.

   用大量欄位建立或更新資料的應用程式模組可能會造成非常大的藍圖。

   * 使用 [!DNL Workfront] 應用程式時，請務必僅選取建立或更新使用案例所需的欄位。
   * 使用其他應用程式時，請使用自訂API模組與任何具有大量欄位的記錄類型互動。

* 雖然案例中的模組數量沒有上限，但超過150個模組的案例會對您的效能造成負面影響 [!DNL Workfront Fusion] 系統。 因此，我們不建議建立超過150個模組的案例。

## 作業

* 預設操作逾時通常為 **40秒**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 檔案

* Fusion對檔案的總處理能力是 **1 GB**. 該限制基於總記憶體成本。 每個行動都造成了這一成本。 如果下載並上載一個400 MB的檔案，則檔案容量的總成本為800 MB。

## 伺服器記憶體使用量

* 單次執行的伺服器記憶體使用量限制為 **1 GB**.

   許多因素（如大型檔案或複雜的模組）都可能以難以預測或控制的方式影響伺服器記憶體的使用。 因此，即使方案遵守所有其他效能護欄，您的方案執行可能超過1 GB記憶體限制。 超過記憶體限制會導致執行失敗。

## Webhook

* 有效負載的預設最大大小為 **5 MB**.
* Webhook限於 **每秒100個請求**. 達到此限制時，Workfront Fusion會傳送429([!UICONTROL 請求太多])狀態。
* [!DNL Workfront Fusion] 儲存webhook負載30天。 在收到Webhook裝載超過30天後存取該裝載會導致錯誤「[!UICONTROL 無法從儲存讀取檔案。]&quot;
* 如果下列任一情況適用，Webhook就會自動停用：

   * Webhook已超過5天未連接到任何情況
   * Webhook僅用於已停用超過30天的非作用中案例。

* 如果停用的WebHook未連線至任何案例，且已停用30天以上，系統就會自動刪除並取消註冊。
