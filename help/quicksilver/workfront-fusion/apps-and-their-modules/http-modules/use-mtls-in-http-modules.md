---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: http-modules
title: 在Adobe Workfront Fusion的HTTP模組中使用雙向TLS
description: 您可以在Adobe Workfront Fusion HTTP模組中使用Mutual TLS，讓資訊交易的兩端都能驗證對方的身分。
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 790f5da3af32ffdfcbb596f467f882a7408e3f28
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# 在HTTP模組中使用雙向TLS [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion需要 [!DNL Adobe Workfront Fusion] 除了Adobe Workfront授權之外，還附加授權。

## 雙向TLS總覽

透過網際網路傳送資料時，請務必確保資料能前往或來自正確位置，且只有指定收件者才能讀取。 啟用TLS後，使用者端（要求資訊的電腦）會使用憑證來驗證伺服器的身分（提供資訊的電腦）。 如此可建立安全的HTTP連線。

雙向TLS可讓此身分確認雙向進行。 當伺服器傳送其憑證以驗證其身分給使用者端時，也會要求使用者端的憑證。 這可確保伺服器不會將資訊傳送給可能誤用的網站或使用者。

>[!INFO]
>
>**範例:**
>
>* **TLS**：當使用者在瀏覽器中輸入「MyGreatBank.com」時，他們想要確保自己會前往My Great Bank，而不是會誤用或出售其銀行資訊的網站。 他們還想確認自己的銀行帳戶資訊已加密。
   >
   >   瀏覽器（使用者端）連線至MyGreatBank.com （伺服器）時，TLS會需要MyGreatBank.com的憑證來驗證其身分。 憑證由憑證授權單位提供，例如 [!DNL DigiCert] 或 [!DNL Thawte]. 因為瀏覽器信任憑證授權單位，所以允許連線。
>
>* **雙向TLS**： MySoftware.com是軟體使用者端，需要MyGreatBank.com API的資訊。 MyGreatBank只允許受信任的客戶連線到他們的伺服器。 因此，除了驗證MyGreatBank.com身分的常規TLS之外，TLS/憑證授權程式也會驗證MySoftware.com的請求。


## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td> <p>[！UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

&#42;&#42;有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 提供您的 [!DNL Workfront Fusion] 公開憑證


當您使用HTTP要求連線至Web服務時，Web服務通常需要 [!DNL Workfront Fusion] 公開憑證以供驗證。 這可讓Web服務比較HTTP要求中提供的憑證與檔案上的憑證，藉此確保憑證位於Web服務的允許清單上。

如需上傳的指示， [!DNL Adobe Workfront Fusion] Web服務的公開憑證，請參閱Web服務的檔案。

>[!NOTE]
>
>除了憑證外，您可能需要提供其他資訊。 如需有關Web服務需求的資訊，請參閱Web服務的API檔案。

您可以使用以下連結下載Workfront Fusion公開憑證：

### 2023年5月25日至2024年6月9日的憑證

>[!IMPORTANT]
>
>* 這些 [!DNL Workfront Fusion] 公開憑證將於2024年6月9日到期。 您的憑證過期後，您需要將新的憑證上傳到Web服務。 建議您：
   >
   >   * 記下到期日並設定提醒，讓您自己將憑證上傳到您的Web服務。
   >   * 將此頁面加入書籤，即可輕鬆找到新憑證。
>
>* 這些是非萬用字元mTLS憑證。


* [下載 [!DNL Workfront Fusion] 2023年憑證](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)
* [下載 [!DNL Workfront Fusion] 2023年歐盟認證](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

   於歐盟使用

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## 在中啟用雙向TLS [!DNL Workfront Fusion] http模組

全部 [!DNL Workfront Fusion] [!UICONTROL HTTP] 請求模組可以選擇啟用雙向TLS。

若要在中啟用雙向TLS [!UICONTROL HTTP] 要求模組：

1. 新增 [!UICONTROL HTTP] 向情境要求模組。
1. 開始設定模組。

   如需設定的說明， [!UICONTROL HTTP] 請求模組，請參閱下方的適當文章 [[!UICONTROL HTTP] 模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. 啟用 **[!UICONTROL 顯示進階設定]** 靠近模組底部。
1. 啟用 **[!UICONTROL 使用雙向TLS]**.
