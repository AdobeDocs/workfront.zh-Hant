---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 案例，績效
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion效能護欄
description: 除了Adobe Workfront授權，Adobe Workfront Fusion還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 8c25835525cc58db0dbe9b22d4f286330e3cb001
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]效能護欄

>[!NOTE]
>
>除了[!DNL Adobe Workfront license]之外，[!DNL Adobe Workfront Fusion]還需要[!DNL Adobe Workfront Fusion]授權。

工作自動化需要快速處理，因此[!DNL Adobe Workfront Fusion]是專為高效能所設計。 由於長期執行情境可能會減慢您工作的速度，因此我們已設計[!DNL Workfront Fusion]搭配保留效能的護欄，以限制執行時間、資料大小和其他情境引數。 [!DNL Workfront Fusion]設計人員應該注意這些護欄，並將它們納入其設計實務中。

## 瀏覽器

* Workfront Fusion僅支援Chrome瀏覽器。

## 情境

* 預設案例執行逾時為&#x200B;**40分鐘**。 當執行達到此逾時時，[!DNL Workfront Fusion]會在下一個週期或作業之後中斷案例執行，視案例而定。 這會在達到40分鐘限制後不久強制停止情境
* 情境藍圖的大小上限為&#x200B;**5 MB**，但建議將情境大小維持在&#x200B;**3 MB**&#x200B;以下。

  使用大量欄位建立或更新資料的應用程式模組可能會產生非常大的藍圖。

   * 使用[!DNL Workfront]應用程式時，請確定僅選取建立或更新使用案例所需的欄位。
   * 使用其他應用程式時，請使用自訂API模組與任何具有大量欄位的記錄型別互動。

* 雖然案例中的模組數量沒有上限，但超過150個模組的案例會對您的[!DNL Workfront Fusion]系統效能產生負面影響。 因此，我們不建議建立超過150個模組的情境。

## 營運

* 預設作業逾時通常為&#x200B;**40秒**。

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 檔案

* Fusion的檔案總處理容量為&#x200B;**1 GB**。 此限制是以總記憶體成本為基礎。 每項作業都會產生該成本。 如果下載並上傳400 MB的單一檔案，則檔案容量的總成本為800 MB。

## 伺服器記憶體使用量

* 單一執行的伺服器記憶體使用量限製為&#x200B;**1 GB**。

  許多因素（例如大型檔案或複雜模組）可能會以難以預測或控制的方式影響伺服器記憶體使用率。 因此，即使案例遵循所有其他效能護欄，您的案例執行仍可能超過1 GB記憶體限制。 超過記憶體限制會導致執行失敗。

## Webhook

* 承載的預設大小上限為&#x200B;**5 MB**。
* Webhook限製為每秒&#x200B;**100個要求**。 達到此限制時，Workfront Fusion會傳送429 （[!UICONTROL 太多請求]）狀態。
* [!DNL Workfront Fusion]儲存webhook裝載30天。 在收到webhook裝載超過30天後存取該裝載會導致錯誤&quot;[!UICONTROL 無法從儲存體讀取檔案。]&quot;
* 如果符合下列任一條件，Webhook就會自動停用：

   * webhook已超過5天未連線至任何案例
   * webhook僅用於非使用中情況，這些情況已非使用中超過30天。

* 如果停用的Webhook未連線至任何情境且處於停用狀態超過30天，則會自動刪除和取消註冊。

## 執行歷史記錄

* 執行記錄檔的大小限製為&#x200B;**100 MB**。 如果執行歷程記錄超過此大小，則只會顯示前100 MB。

## 未完成的執行

* 未完成的執行限製為&#x200B;**500 MB**&#x200B;的總大小。 如果達到500 MB限制，則不會再儲存不完整的執行。

## 重試次數

* 使用Break模組並指定Retry指示詞時，如果案例在2分鐘的時間範圍內連續失敗10次，則案例將自動停用。

