---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] 使用API代號授權的網站服務
description: 有些服務不允許整合解決方案，例如 [!DNL Adobe Workfront Fusion] 建立可輕鬆在案例中使用的應用程式。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] 使用API代號授權的網站服務

有些服務不允許整合解決方案，例如 [!DNL Adobe Workfront Fusion] 建立可輕鬆在案例中使用的應用程式。

有因應措施。 您可以將所需的服務（應用程式）連結至 [!DNL Workfront Fusion] 使用 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] 模組。

本文說明如何將幾乎任何Web服務連接至 [!DNL Workfront Fusion] 使用API金鑰/API代號。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 連線至使用API代號的網站服務

透過API代號連線服務的程式，在大部分的網站服務中都類似。

1. 在網站服務的網站上建立應用程式，如 [建立新應用程式並取得API代號](#create-a-new-application-and-obtain-the-api-token) 這篇文章。
1. 取得API金鑰或API代號。
1. 新增 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] > [!UICONTROL 提出請求] 模組至您的案例。
1. 根據網站服務的API檔案設定模組並執行案例，如一節中所述 [設定 [!UICONTROL HTTP] 模組](#set-up-the-http-module) 這篇文章。

>[!NOTE]
>
>我們將使用 [!DNL Pushover] 通知服務，做為本文的範例。

## 建立新應用程式並取得API代號

>[!NOTE]
>
>網站服務建立和分發API金鑰或API權杖的方式有許多不同。 如需取得所需網站服務之API金鑰和代號的指示，請前往服務的網站，並搜尋「API金鑰」或「API代號」。
>
>我們提供取得Pushover API金鑰的指示，僅供您找到的範例之用。

1. 登入 [!DNL Pushover] 帳戶。
1. 按一下 **[!UICONTROL 建立應用程式/API代號]** 頁面底部。
1. 填寫應用程式資訊，然後按一下 **[!UICONTROL 建立應用程式]**.
1. 將提供的API代號儲存在安全的位置。 您需要它 [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL 提出請求] 連接到所需Web服務的模組([!DNL Pushover]，在此案例中為)。

## 設定 [!UICONTROL HTTP] 模組

將Web服務連接到 [!DNL Workfront Fusion] 情境中，您需要使用 [!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組，並根據網站服務的API檔案來設定模組。

1. 新增 [!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組至您的案例。
1. 若要推送訊息，請使用 [!DNL Workfront Fusion]，請依照下列方式設定HTTP模組。

   >[!NOTE]
   >
   >這些模組設定對應至 [!DNL Pushover] 網站服務API檔案。 其他網站服務的設定可能不同。 例如，API代號可插入至 [!UICONTROL 標題] 而不是 [!UICONTROL 主體] 欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>URL欄位包含您可在網站服務API檔案中找到的端點。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL方法]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>使用的方法取決於對應的端點。 推送訊息的Pushover端點使用POST方法。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL標題]</p> </td> 
      <td> <p>某些網站服務可能會使用標題來指定API代號驗證或其他參數。 在本例中並非如此，因為推送訊息的Pushover端點會對所有請求類型使用Body（請參閱下方）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL查詢字串]</p> </td> 
      <td> <p>某些網站服務可能會使用查詢字串來指定其他參數。 在我們的範例中並非如此，因為 [!DNL Pushover] Web服務會對所有請求類型使用[!UICONTROL Body]（請參閱下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL主體類型]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>此設定可讓您在下方的[!UICONTROL內容類型]欄位中選取JSON內容類型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL內容類型]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON是[!UICONTROL Pushover]應用程式所需的內容類型。 這可能與其他網站服務不同。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL要求內容]</p> </td> 
      <td> <p>以JSON格式輸入[!UICONTROL Body]要求內容。 您可以使用[!UICONTROL JSON] &gt; [!UICONTROL建立JSON]模組，如 <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">使用[!UICONTROL JSON] &gt; [!UICONTROL建立JSON]模組對應JSON內文</a> 這篇文章。 或者，您可以手動輸入JSON內容，請參閱 <a href="#json-body-entered-manually" class="MCXref xref">手動輸入JSON內文</a> 這篇文章。</p> <p>如需該網站服務的必要參數，請參閱網站服務的API檔案。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手動輸入JSON內文

以JSON格式指定參數和值。

>[!INFO]
>
>**範例:**
>
>
```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>
"token":"123459evz8aepwtxydndydgyumbfx",
>
>
"message":"Hello World!",
>
>
"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL用戶]</p> </td> 
   <td> <p>您的USER_KEY。 您可在 [!DNL Pushover] 控制面板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL令牌] </td> 
   <td> <p>您建立的API代號/API金鑰 [!DNL Pushover] 應用程式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息] </td> 
   <td> <p>傳送至裝置之推播通知的文字內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題] </td> 
   <td> <p>（選用）您的訊息標題。 如果未輸入任何值，則會使用您應用程式的名稱。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用 [!UICONTROL JSON] >[!UICONTROL 建立JSON] 模組

此 [!UICONTROL 建立JSON] 模組可讓指定JSON變得更輕鬆。 您也可以動態定義值。

如需JSON模組的詳細資訊，請參閱 [JSON模組](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. 輸入或對應您要從中建立JSON的值。

   ![](assets/json-values-350x288.png)

1. 連接 [!UICONTROL JSON] > [!UICONTROL 建立JSON] 模組至HTTP >提出要求模組。
1. 從 [!UICONTROL 建立JSON] 模組 [!UICONTROL 要求內容] 欄位 [!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組。

   現在，當您執行案例時，推播通知會傳送至已在 [!DNL Pushover] 帳戶。
