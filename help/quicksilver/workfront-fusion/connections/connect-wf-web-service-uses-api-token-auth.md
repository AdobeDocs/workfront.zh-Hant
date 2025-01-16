---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 將 [!DNL Adobe Workfront Fusion] 連線至使用API權杖授權的網站服務
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# 將[!DNL Adobe Workfront Fusion]連線到使用API權杖授權的網站服務

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [將Adobe Workfront Fusion連線至使用API權杖授權的Web服務](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-wf-web-service-uses-api-token-auth.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

某些服務不允許整合解決方案（例如[!DNL Adobe Workfront Fusion]）建立您可在情境中輕鬆使用的應用程式。

此情況有個因應措施。 您可以使用[!DNL Workfront Fusion]的[!UICONTROL HTTP]模組將所需的服務（應用程式）連線到[!DNL Workfront Fusion]。

本文說明如何使用API金鑰/API權杖將幾乎任何Web服務連線至[!DNL Workfront Fusion]。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## 連線到使用API權杖的網站服務

對於大多數Web服務，透過API權杖連線服務的程式都類似。

1. 在網站服務網站上建立應用程式，如本文中[建立新應用程式並取得API權杖](#create-a-new-application-and-obtain-the-api-token)一節所述。
1. 取得API金鑰或API權杖。
1. 新增[!DNL Workfront Fusion]的[!UICONTROL HTTP] > [!UICONTROL 對您的情境提出要求]模組。
1. 根據網站服務的API檔案設定模組並執行案例，如本文中[設定[!UICONTROL HTTP]模組](#set-up-the-http-module)一節所述。

>[!NOTE]
>
>我們將在整篇文章中以[!DNL Pushover]通知服務為例。

## 建立新應用程式並取得API權杖

>[!NOTE]
>
>網站服務有多種不同的方式來建立和分發API金鑰或API權杖。 如需有關取得所需Web服務的API金鑰和權杖的指示，請前往該服務的網站並搜尋「API金鑰」或「API權杖」。
>
>我們提供的說明僅包括取得Pushover API金鑰的內容，以作為您可能會找到的內容範例。

1. 登入您的[!DNL Pushover]帳戶。
1. 按一下頁面底部的&#x200B;**[!UICONTROL 建立應用程式/API權杖]**。
1. 填寫應用程式資訊，然後按一下&#x200B;**[!UICONTROL 建立應用程式]**。
1. 將提供的API權杖儲存在安全的地方。 您需要[!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL 發出要求]模組以連線到所需的Web服務（在此案例中為[!DNL Pushover]）。

## 設定[!UICONTROL HTTP]模組

若要將Web服務連線至您的[!DNL Workfront Fusion]案例，您必須使用[!UICONTROL HTTP] >[!UICONTROL 在案例中提出要求]模組，並根據Web服務的API檔案設定模組。

1. 新增[!UICONTROL HTTP] >[!UICONTROL 請求]模組至您的情境。
1. 若要使用[!DNL Workfront Fusion]推送訊息，請依照下列方式設定HTTP模組。

   >[!NOTE]
   >
   >這些模組設定對應至[!DNL Pushover] Web服務API檔案。 其他Web服務的設定可能不同。 例如，API權杖可以插入[!UICONTROL Header]，而不是[!UICONTROL Body]欄位。

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
      <td role="rowheader"> <p>[！UICONTROL Headers]</p> </td> 
      <td> <p>某些網站服務可能會使用標頭來指定API權杖驗證或其他引數。 在我們的範例中，情況並非如此，因為推播訊息的Pushover端點會針對所有請求型別使用Body （請參閱下文）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL查詢字串]</p> </td> 
      <td> <p>某些Web服務可能會使用查詢字串來指定其他引數。 在我們的範例中並非如此，因為[!DNL Pushover] Web服務對所有要求型別都使用[！UICONTROL Body] （請參閱下文）。</p> </td> 
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
      <td> <p>輸入JSON格式的[！UICONTROL Body]要求內容。 您可以使用[！UICONTROL JSON] &gt; [！UICONTROL建立JSON]模組，如本文中<a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">使用[！UICONTROL JSON] &gt; [！UICONTROL建立JSON]模組</a>對映的JSON內文所述。 或者，您可以手動輸入JSON內容，如本文中<a href="#json-body-entered-manually" class="MCXref xref">手動輸入的JSON內文</a>所述。</p> <p>請參閱網站服務的API檔案，瞭解該Web服務所需的引數。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手動輸入的JSON內文

以JSON格式指定引數和值。

>[!INFO]
>
>**範例：**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL使用者]</p> </td> 
   <td> <p>您的使用者金鑰。 您可在您的[!DNL Pushover]儀表板中找到此專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL權杖] </td> 
   <td> <p>您建立的[!DNL Pushover]應用程式是由您產生的API Token/API金鑰。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息] </td> 
   <td> <p>傳送至裝置的推播通知文字內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標題] </td> 
   <td> <p>（選用）您的訊息標題。 如果未輸入值，則會使用您的應用程式名稱。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用[!UICONTROL JSON] >[!UICONTROL 建立JSON]模組來對JSON內文

[!UICONTROL 建立JSON]模組可讓您更輕鬆地指定JSON。 它也能讓您以動態方式定義值。

如需JSON模組的詳細資訊，請參閱[JSON模組](../../workfront-fusion/apps-and-their-modules/json-modules.md)。

1. 輸入或對應您要建立JSON的值。

   ![](assets/json-values-350x288.png)

1. 將[!UICONTROL JSON] > [!UICONTROL 建立JSON]模組連線到HTTP >建立要求模組。
1. 將[!UICONTROL 建立JSON]模組的JSON字串對應至[!UICONTROL HTTP] >[!UICONTROL 提出要求]模組中的[!UICONTROL 要求內容]欄位。

   現在，當您執行情境時，推播通知會傳送至已在您的[!DNL Pushover]帳戶中註冊的裝置。
