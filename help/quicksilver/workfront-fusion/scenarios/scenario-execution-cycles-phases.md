---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在 [!DNL Adobe Workfront Fusion]中的案例執行、週期和階段
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的案例執行、週期和階段

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [案例執行、週期和階段](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/scenario-execution-cycles-phases.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

[!DNL Adobe Workfront Fusion]是交易式系統，類似於關聯式資料庫。 每個案例執行從初始化階段開始，接著至少包含一個由作業和認可/復原階段組成的週期，然後結束最終化階段：

>[!INFO]
>
>**範例**
>
>初始化
>
>循環#1
>
>作業（讀取或寫入）
>
>認可或回覆
>
>循環#2
>
>作業（讀取或寫入）
>
>認可或回覆
>
>...
>
>循環#N
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
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 初始化

在初始化階段，會建立所有必要的連線（連線到資料庫、電子郵件服務等）。 此外，也會檢查每個模組是否能夠執行其預期操作。

## 週期

每個週期代表不可分割的工作單位，由一系列操作組成。 可以在[!UICONTROL 案例設定]面板中設定最大循環數。 預設數字為1。

如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[案例設定面板。

## 營運

在作業階段期間執行讀取和/或寫入作業：

* 讀取作業包含從服務取得資料，然後由其他模組根據預先定義的案例加以處理。 例如，[!UICONTROL Dropbox] >[!UICONTROL 監看檔案]模組會傳回自上次案例執行以來建立的新組合（檔案）。
* 寫入作業包含傳送資料至指定服務以供進一步處理。 例如，[!DNL Dropbox] >[!UICONTROL 上傳檔案]模組會將檔案上傳至[!DNL Dropbox]資料夾。

## 認可

如果所有模組的操作階段都成功，則認可階段會開始，在此期間模組執行的所有操作都會被認可。 這表示[!DNL Workfront Fusion]會傳送其成功相關資訊給所有參與作業階段的服務。

## 復原

如果任何模組的作業或認可階段發生錯誤，該階段會中止，而倒回階段會啟動，使指定週期中的所有作業失效。 某些模組不支援回覆，且無法取回這些模組執行的作業。 如需詳細資訊，請參閱[ACID模組](#acid-modules)區段。

## 最終處理

在最終確定階段，會關閉開啟的連線（例如FTP連線、資料庫連線等），並完成情境。

## ACID模組

所有支援回覆（也稱為異動）的[!DNL Workfront Fusion]模組都會標示ACID標籤。

![](assets/acid-modules-350x189.png)

當其他模組發生錯誤時，未標示此標籤的模組無法回覆為初始狀態。 非ACID模組的典型範例是[!UICONTROL 電子郵件] >[!UICONTROL 傳送電子郵件]動作。 傳送電子郵件後，您無法復原傳送。
