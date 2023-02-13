---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]
description: 本文說明在 [!DNL Adobe Workfront Fusion] 方案正在運行，如初始化、操作、提交和回滾。
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] 是交易式系統，類似於關係資料庫。 每個方案執行從初始化階段開始，繼續進行由操作和提交/回滾階段組成的至少一個週期，並結束於定稿階段：

>[!INFO]
>
>**範例**
>
>初始化
>
>週期#1
>
>操作（讀或寫）
>
>提交或回滾
>
>週期#2
>
>操作（讀或寫）
>
>提交或回滾
>
>...
>
>週期#N
>
>操作（讀或寫）
>
>提交或回滾
>
>最後確定

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 初始化

在初始化階段，會建立所有必要的連線（連線至資料庫、電子郵件服務等）。 如果每個模組能夠執行其預定操作，也會檢查它們。

## 循環

每個週期表示由一系列操作組成的不可分割的工作單位。 您可以在 [!UICONTROL 藍本設定] 中。 預設數字為1。

如需詳細資訊，請參閱 [中的藍本設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 作業

在操作階段執行讀取和/或寫入操作：

* 讀取操作包括從服務中獲取資料，然後由其它模組根據預先定義的方案進行處理。 例如， [!UICONTROL Dropbox] >[!UICONTROL 監看檔案] 模組會傳回自上次執行案例後建立的新套件組合（檔案）。
* 寫入操作包括將資料發送到給定服務以進行進一步處理。 例如， [!DNL Dropbox] >[!UICONTROL 上傳檔案] 模組將檔案上傳至 [!DNL Dropbox] 檔案夾。

## 認可

如果所有模組的操作階段均成功，則提交階段將在提交模組執行的所有操作期間開始。 這表示 [!DNL Workfront Fusion] 會傳送有關其成功的資訊給操作階段涉及的所有服務。

## 回復

如果在任何模組的操作或提交階段期間發生錯誤，則該階段被中止，並且回滾階段被啟動，從而使給定循環撤消期間的所有操作都無效。 某些模組不支援回滾，並且無法恢復由這些模組執行的操作。 如需詳細資訊，請參閱 [酸模組](#acid-modules) 區段。

## 最後確定

在最終處理階段期間，開啟的連線（例如FTP連線、資料庫連線等）會關閉，而案例會完成。

## 酸模組

全部 [!DNL Workfront Fusion] 支援回滾的模組（也稱為交易性）會以ACID標籤標籤。

![](assets/acid-modules-350x189.png)

當其他模組中發生錯誤時，未標示此標籤的模組無法還原回其初始狀態。 非ACID模組的典型範例為 [!UICONTROL 電子郵件] >[!UICONTROL 傳送電子郵件] 動作。 傳送電子郵件後，您無法還原傳送。
