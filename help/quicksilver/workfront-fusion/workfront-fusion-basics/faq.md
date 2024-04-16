---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion常見問題集
description: 本文會介紹以下專案的相關常見問題： [!DNL Adobe Workfront Fusion]，包括有關Fusion工作流程中常用物件的資訊
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 1%

---

# Adobe Workfront Fusion常見問題集

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
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 工作自動化與整合]，請參閱[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 什麼是情境？

### 解答

案例會定義要執行的步驟序列 [!DNL Adobe Workfront Fusion]. 對於每個案例，您都可以指定資料來源、資料的處理方式、要使用的資料以及要忽略的資料。 [!DNL Workfront Fusion] 可讓您視需要建立最複雜的情境；甚至是最複雜的情境也是有可能的。

如需詳細資訊，請參閱 [在中建立實務整合情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## 我可以在一個案例中使用多個模組嗎？ 還是僅僅是個觸發器和動作？

### 解答

您可以在情境中使用任意數量的模組。 您可以建立獨立的路由，並指定哪些資料應流經路由。 您也可以使用個別動作傳回的結果，然後將其傳遞至下一個動作。

## 可以 [!DNL Workfront Fusion] 使用檔案？

### 解答

是。使用 [!DNL Workfront Fusion]，即可接收、儲存、轉換、轉換、加密等檔案。 此外， [!DNL Workfront Fusion] 提供各式各樣的內建功能，協助使用者有效且創造性地處理檔案中包含的資料。

如需詳細資訊，請參閱 [關於對應檔案於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## 如果我讓 [!DNL Workfront Fusion] 是否處理包含多個附件的電子郵件？

### 解答

如果您使用 [!UICONTROL 電子郵件] 模組 [!UICONTROL 擷取附件]，每個附件會透過情境中的其餘模組個別傳送。 類似的模組也可用於同時接收多個檔案的其他應用程式。

如需詳細資訊，請參閱 [[!UICONTROL 電子郵件] 模組](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## 有些觸發器允許立即執行情境。 「即時」是什麼意思？

### 解答

常見情境會根據您指定的排程定期執行（例如，每小時、每5分鐘、每月一次，等等）。 有一些特殊的觸發器，稱為即時觸發器(webhook)，可在從指定服務收到資料後立即啟動您的情境。 即時觸發程式可能非常有用。 建議儘可能使用。 它們有助於減少操作次數。 收到的資料會立即處理，不會等候下一次排程的執行。 例如， [!DNL Google Sheets] 模組 [!UICONTROL 觀看變更] 在更新儲存格後立即開始案例。

## 什麼是彙總？

### 解答

一個 [!UICONTROL 彙總] 將資料合併至單一集合。 例如，將檔案壓縮為zip封存檔並作為電子郵件附件傳送。

如需詳細資訊，請參閱 [[!UICONTROL 彙總] 中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 什麼是作業？

### 解答

作業是指模組執行的任何工作。 例如，每次執行觸發程式時，以及每次動作執行工作時，都會發生作業。

## 什麼是資料傳輸？

### 解答

資料傳輸是指透過您的情境傳輸的資料量。 例如，假設您的案例從FTP擷取100KB的影像，並將其大小縮減至50KB，然後將兩個影像儲存至 [!DNL Dropbox]. 此情境中使用的資料量為250KB。

## 什麼是連線？

### 解答

連線是您與網站之間 [!DNL Workfront Fusion] 帳戶和您要使用的第三方服務。 編輯情境時，可輕鬆建立連線。 若要新增連線，請按一下 **[!UICONTROL 新增]** 按鈕，並依照逐步指示操作。

如需詳細資訊，請參閱 [連線總覽](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
