---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: http-modules
title: 在Adobe Workfront Fusion的HTTP模組中使用相互TLS
description: 您可以在Adobe Workfront Fusion HTTP模組中使用Mutual TLS，允許資訊交易的兩側驗證對方的身份。
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: e67e6b6d3baf9f17a0a451fa4e1dbc365340f76e
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# 在的HTTP模組中使用相互TLS [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion需要 [!DNL Adobe Workfront Fusion] 授權，以及Adobe Workfront授權。

## 相互TLS概述

當您透過網際網路傳送資料時，請務必確保資料移至或來自正確位置，而且只有目標收件者才能讀取。 啟用TLS後，客戶端（請求資訊的電腦）將使用證書來驗證伺服器（提供資訊的電腦）的身份。 這可讓安全的HTTP連線。

相互TLS可讓此身分確認以兩種方式進行。 當伺服器將其證書發送到客戶端驗證其身份時，它也請求客戶端的證書。 這可確保伺服器不會將資訊傳送給會濫用資訊的網站或使用者。

>[!INFO]
>
>**範例:**
>
>* **TLS**:當某人在瀏覽器中鍵入「MyGreatBank.com」時，他們希望確保他們會訪問「我的Great Bank」，而不是可能濫用或出售其銀行資訊的網站。 他們還希望確保其銀行賬戶資訊被加密。
   >
   >   當瀏覽器（客戶端）連接到MyGreatBank.com（伺服器）時，TLS需要MyGreatBank.com的證書來驗證其身份。 憑證由憑證機構提供，例如 [!DNL DigiCert] 或 [!DNL Thawte]. 因為瀏覽器信任憑證授權機構，所以允許連線。
>
>* **相互TLS**:MySoftware.com是軟體客戶端，需要MyGreatBank.com API提供的資訊。 MyGreatBank僅允許受信任的客戶連接到其伺服器。 因此，除了驗證MyGreatBank.com身份的常規TLS外，TLS/證書頒發機構進程還驗證來自MySoftware.com的請求。


## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

&#42;&#42;如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 提供 [!DNL Workfront Fusion] 公開憑證


當您使用HTTP要求連線至Web服務時，Web服務通常需要 [!DNL Workfront Fusion] 供驗證的公開證書。 這可讓Web服務將HTTP要求中呈現的憑證與檔案上的憑證進行比較，以確保憑證位於Web服務的允許清單中。

如需上傳 [!DNL Adobe Workfront Fusion] 向Web服務發放公共證書，請參閱Web服務的文檔。

>[!NOTE]
>
>除了憑證外，您可能需要提供其他資訊。 如需網站服務需要的相關資訊，請參閱網站服務的API檔案。

您可以使用下列連結來下載Workfront Fusion公開憑證：

### 2023年5月25日至2024年6月9日的證明

>[!IMPORTANT]
>
>* 這些 [!DNL Workfront Fusion] 公開證書將於2024年6月9日到期。 您的過期後，您需要將新憑證上傳至網站服務。 建議您：
   >
   >   * 記下到期日，並為您自己設定提醒，將憑證上傳至您的網站服務。
   >   * 將此頁面加入書籤，以輕鬆找到新憑證。
>
* 這些是非萬用字元mTLS憑證。
>

* [下載 [!DNL Workfront Fusion] 證書2023](assets/fusion-prod-us-mtls-certificate.pem)
* [下載 [!DNL Workfront Fusion] 2023年歐盟證書](assets/fusion-prod-eu-mtls-certificate.pem)

   供歐盟使用

### 2022年11月14日至2023年7月15日的證明

>[!IMPORTANT]
>
>* 這些 [!DNL Workfront Fusion] 公開證書將於2023年7月15日到期。
>* 這些是萬用字元mTLS憑證。


* [下載 [!DNL Workfront Fusion] 證書2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [下載 [!DNL Workfront Fusion] 2023年歐盟證書](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   供歐盟使用

## 在中啟用相互TLS [!DNL Workfront Fusion] HTTP模組

全部 [!DNL Workfront Fusion] [!UICONTROL HTTP] 要求模組可以選擇啟用相互TLS。

若要在 [!UICONTROL HTTP] 要求模組：

1. 新增 [!UICONTROL HTTP] 請求模組至您的案例。
1. 開始配置模組。

   如需設定 [!UICONTROL HTTP] 要求模組，請參閱 [[!UICONTROL HTTP] 模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. 啟用 **[!UICONTROL 顯示高級設定]** 接近模組底部。
1. 啟用 **[!UICONTROL 使用相互TLS]**.
