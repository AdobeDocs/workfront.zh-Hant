---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion常見問題集
description: 本文探討與 [!DNL Adobe Workfront Fusion]，包括關於Fusion工作流程中常用物件的資訊
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Adobe Workfront Fusion常見問題集

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 什麼情況？

### 回答

案例會定義要執行的步驟順序 [!DNL Adobe Workfront Fusion]. 您可以針對每個案例指定資料來源、資料的處理方式，以及要使用哪些資料以及要忽略哪些資料。 [!DNL Workfront Fusion] 可讓您視需要建立複雜的情境；即使是最複雜的情景也是可能的。

如需詳細資訊，請參閱 [在中建立實務整合案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## 我可以在案例中使用多個模組嗎？ 還是只是觸發和行動？

### 回答

您可以在案例中使用任意數量的模組。 您可以建立獨立的路由，並指定應通過這些路由傳輸的資料。 您也可以使用個別動作傳回的結果，然後傳遞至下一個動作。

## 可 [!DNL Workfront Fusion] 使用檔案？

### 回答

是. 使用 [!DNL Workfront Fusion]、可接收、儲存、轉換、轉換、加密等。 此外， [!DNL Workfront Fusion] 提供多種內建功能，旨在讓使用者能夠有效且創造性地處理檔案中包含的資料。

如需詳細資訊，請參閱 [關於在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## 如果我讓 [!DNL Workfront Fusion] 處理包含多個附件的電子郵件？

### 回答

如果您使用 [!UICONTROL 電子郵件] 模組 [!UICONTROL 檢索附件]，則每個附件會透過案例中的其餘模組個別傳送。 同時接收多個檔案的其他應用程式也提供類似模組。

如需詳細資訊，請參閱 [[!UICONTROL 電子郵件] 模組](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## 有些觸發器可讓情境立即執行。 「立即」是什麼意思？

### 回答

常見情況會根據您指定的排程（例如，每小時、每5分鐘、每月一次等）以間隔執行。 有些特殊觸發(稱為即時觸發(Webhook))，在您從指定服務收到資料後，就會立即啟動您的案例。 即時觸發器可能非常有用。 建議您盡可能使用。 它們有助於減少操作的數量。 接收的資料會立即處理，而不等待下次排程執行。 例如， [!DNL Google Sheets] 模組 [!UICONTROL 監看變更] 在儲存格更新後立即開始案例。

## 什麼是整合器？

### 回答

安 [!UICONTROL 匯總器] 將資料合併為單一集合。 例如，檔案會壓縮為zip封存，並以電子郵件附件的形式傳送。

如需詳細資訊，請參閱 [[!UICONTROL 匯總器] 模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 什麼是操作？

### 回答

操作是模組執行的任何任務。 例如，每次觸發器執行時，以及每次動作執行任務時，都會執行操作。

## 什麼是資料傳輸？

### 回答

資料傳輸是指透過您的案例傳輸的資料量。 例如，假設您的案例是從FTP擷取100KB的影像，並將其大小縮小至50KB，並將兩個影像儲存至 [!DNL Dropbox]. 此情境中使用的資料量為150KB。

## 什麼是連線？

### 回答

連線是您 [!DNL Workfront Fusion] 帳戶和您要使用的第三方服務。 編輯案例時可輕鬆建立連線。 若要新增連線，請按一下 **[!UICONTROL 新增]** 按鈕，並依照逐步指示操作。

如需詳細資訊，請參閱 [關於連接 [!DNL Adobe Workfront Fusion] 至應用程式或服務](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
