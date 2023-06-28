---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] 至使用API權杖授權的網站服務
description: 某些服務不允許整合解決方案，例如 [!DNL Adobe Workfront Fusion] 以建立可在情境中輕鬆使用的應用程式。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] 至使用API權杖授權的網站服務

某些服務不允許整合解決方案，例如 [!DNL Adobe Workfront Fusion] 以建立可在情境中輕鬆使用的應用程式。

此情況有個因應措施。 您可以將所需的服務（應用程式）連線至 [!DNL Workfront Fusion] 使用 [!DNL Workfront Fusion]的 [!UICONTROL HTTP] 模組。

本文說明如何將幾乎任何Web服務連線至 [!DNL Workfront Fusion] 使用API金鑰/API權杖。

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
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
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

## 連線到使用API權杖的Web服務

對於大多數Web服務，透過API權杖連線服務的程式都類似。

1. 在Web服務的網站上建立應用程式，如區段中所述 [建立新應用程式並取得API權杖](#create-a-new-application-and-obtain-the-api-token) 本文章內容。
1. 取得API金鑰或API權杖。
1. 新增 [!DNL Workfront Fusion]的 [!UICONTROL HTTP] > [!UICONTROL 提出請求] 模組至您的情境。
1. 根據網站服務的API檔案設定模組，並執行情境，如一節中所述 [設定 [!UICONTROL HTTP] 模組](#set-up-the-http-module) 本文章內容。

>[!NOTE]
>
>我們將使用 [!DNL Pushover] 通知服務作為範例。

## 建立新應用程式並取得API權杖

>[!NOTE]
>
>Web服務建立及分發API金鑰或API權杖的方式有很多種。 如需有關取得所需Web服務API金鑰和權杖的說明，請前往該服務的網站並搜尋「API金鑰」或「API權杖」。
>
>我們包含取得Pushover API金鑰的指示，僅作為您可能找到什麼的範例。

1. 登入您的 [!DNL Pushover] 帳戶。
1. 按一下 **[!UICONTROL 建立應用程式/API權杖]** 位於頁面底部。
1. 填寫應用程式資訊，然後按一下 **[!UICONTROL 建立應用程式]**.
1. 將提供的API權杖儲存在安全的地方。 您需要它用於 [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組以連線到所需的Web服務([!DNL Pushover]，在此例中為)。

## 設定 [!UICONTROL HTTP] 模組

若要將Web服務連線至您的 [!DNL Workfront Fusion] 情境，您需要使用 [!UICONTROL HTTP] >[!UICONTROL 提出要求] 模組，並根據網站服務的API檔案設定模組。

1. 新增 [!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組至您的情境。
1. 若要推送訊息，請使用 [!DNL Workfront Fusion]，請依照以下方式設定HTTP模組。

   >[!NOTE]
   >
   >這些模組設定對應至 [!DNL Pushover] 網站服務API檔案。 其他Web服務的設定可能不同。 例如，可以將API權杖插入 [!UICONTROL 頁首] 而非 [!UICONTROL 內文] 欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>URL欄位包含您可以在網站服務的API檔案中找到的端點。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL方法]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>使用的方法取決於對應的端點。 推送訊息的Pushover端點會使用POST方法。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL標頭]</p> </td> 
      <td> <p>某些網站服務可能會使用標頭來指定API權杖驗證或其他引數。 我們的範例並非如此，因為推送訊息的Pushover端點會針對所有請求型別使用Body （請參閱下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL查詢字串]</p> </td> 
      <td> <p>某些Web服務可能會使用查詢字串來指定其他引數。 在我們的範例中，情況並非如此，因為 [!DNL Pushover] Web服務對所有請求型別使用[！UICONTROL Body] （請參閱下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL主體型別]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>此設定可讓您在下方的[！UICONTROL內容型別]欄位中選取JSON內容型別。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL內容型別]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON是[！UICONTROL Pushover]應用程式所需的內容型別。 這可能與其他網站服務不同。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL要求內容]</p> </td> 
      <td> <p>以JSON格式輸入[！UICONTROL Body]要求內容。 您可以使用[！UICONTROL JSON] &gt; [！UICONTROL建立JSON]模組，如中所述 <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">使用[！UICONTROL JSON] &gt; [！UICONTROL建立JSON]模組來對JSON內文</a> 本文章內容。 或者，您也可以手動輸入JSON內容，如中所述 <a href="#json-body-entered-manually" class="MCXref xref">手動輸入的JSON內文</a> 本文章內容。</p> <p>如需該Web服務的必要引數，請參閱Web服務的API檔案。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手動輸入的JSON內文

以JSON格式指定引數和值。

>[!INFO]
>
>**範例:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>
>"token":"123459evz8aepwtxydndydgyumbfx",
>
>
>"message":"Hello World!",
>
>
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL使用者]</p> </td> 
   <td> <p>您的USER_KEY。 您可在以下網址找到此專案： [!DNL Pushover] 儀表板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL權杖] </td> 
   <td> <p>您建立的API權杖/API金鑰產生於 [!DNL Pushover] 應用程式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息] </td> 
   <td> <p>傳送至裝置的推播通知文字內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標題] </td> 
   <td> <p>（選用）您的訊息標題。 如果未輸入任何值，則會使用您的應用程式名稱。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用的JSON內文對應 [!UICONTROL JSON] >[!UICONTROL 建立JSON] 模組

此 [!UICONTROL 建立JSON] 模組可讓您更輕鬆地指定JSON。 它也能讓您以動態方式定義值。

如需JSON模組的詳細資訊，請參閱 [JSON模組](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. 輸入或對應您要建立JSON的值。

   ![](assets/json-values-350x288.png)

1. 連線 [!UICONTROL JSON] > [!UICONTROL 建立JSON] 模組到HTTP >建立請求模組。
1. 將JSON字串對應自 [!UICONTROL 建立JSON] 模組至 [!UICONTROL 要求內容] 中的欄位 [!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組。

   現在，當您執行案例時，推播通知會傳送至已在中註冊的裝置 [!DNL Pushover] 帳戶。
