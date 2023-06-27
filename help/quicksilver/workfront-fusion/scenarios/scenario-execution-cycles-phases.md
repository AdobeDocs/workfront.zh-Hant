---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 中的案例執行、週期和階段 [!DNL Adobe Workfront Fusion]
description: 本文會說明當客戶收到電子郵件時 [!DNL Adobe Workfront Fusion] 案例正在執行，例如，初始化、操作、認可和回覆。
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# 中的案例執行、週期和階段 [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] 是交易式系統，類似於關聯式資料庫。 每個案例執行都從初始化階段開始，接著是至少一個由作業和認可/復原階段組成的週期，最後是完成階段：

>[!INFO]
>
>**範例**
>
>初始化
>
>週期#1
>
>作業（讀取或寫入）
>
>認可或回覆
>
>週期#2
>
>作業（讀取或寫入）
>
>認可或回覆
>
>...
>
>週期#N
>
>作業（讀取或寫入）
>
>認可或回覆
>
>最終處理

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 若為工作自動化與整合]，[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 初始化

在初始化階段，會建立所有必要的連線（連線到資料庫、電子郵件服務等）。 此外，也會檢查每個模組是否能夠執行其預期操作。

## 週期

每個週期代表不可分割的工作單位，由一系列作業組成。 可以設定中的最大循環數 [!UICONTROL 案例設定] 面板。 預設數字為1。

如需詳細資訊，請參閱 [中的案例設定面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 作業

在操作階段期間，執行讀取和/或寫入操作：

* 讀取作業包含從服務取得資料，然後由其他模組根據預先定義的案例進行處理。 例如， [!UICONTROL Dropbox] >[!UICONTROL 觀看檔案] 模組會傳回自上次案例執行以來建立的新組合（檔案）。
* 寫入作業包含傳送資料給指定服務以供進一步處理。 例如， [!DNL Dropbox] >[!UICONTROL 上傳檔案] 模組將檔案上傳至 [!DNL Dropbox] 資料夾。

## 認可

如果所有模組的操作階段都成功，則認可階段會開始，在此期間模組執行的所有操作都會被認可。 這表示 [!DNL Workfront Fusion] 會傳送其成功的相關資訊給作業階段中涉及的所有服務。

## 復原

如果任何模組的作業或認可階段發生錯誤，該階段會中止，而倒回階段會啟動，使得指定週期中的所有作業都無效。 某些模組不支援復原，且這些模組執行的作業無法恢復。 如需詳細資訊，請參閱 [ACID模組](#acid-modules) 區段。

## 最終處理

在最終確定階段，會關閉開啟的連線（例如FTP連線、資料庫連線等），並完成情境。

## ACID模組

全部 [!DNL Workfront Fusion] 支援回覆（也稱為異動）的模組會標示ACID標籤。

![](assets/acid-modules-350x189.png)

當其他模組發生錯誤時，未標示此標籤的模組無法回覆為初始狀態。 非ACID模組的典型範例為 [!UICONTROL 電子郵件] >[!UICONTROL 傳送電子郵件] 動作。 傳送電子郵件後，您無法復原傳送。
