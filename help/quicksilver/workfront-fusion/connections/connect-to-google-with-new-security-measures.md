---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 包含更新的安全性措施
description: Google最近對使用者使用其API的方式進行了限制。 本文會說明如何連線 [!DNL Adobe Workfront Fusion] Google，請注意這些更新安全性措施。
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 包含更新的安全性措施

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

## [!DNL Google Services] 限制

[!DNL Google] 自2020年6月1日起，使用者已引入其API的使用方式限制。 這些安全性措施可保護 [!DNL Google] 使用者個人資料洩漏或誤用 [!DNL Google]. 這些限制與 [!DNL Gmail] 和 [!DNL Google Drive] 應用程式。 如需這些限制的詳細資訊，請參閱 [[!DNL Google] API服務使用者資料原則](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

若要存取受限制的範圍，連線的服務([!DNL Adobe Workfront Fusion] 或任何想要透過API存取使用者資料的其他服務)都必須經過驗證，且必須具備評估函，以證明服務在使用資料方面的安全性與透明度。 [!DNL Workfront Fusion] 符合所有 [!DNL Google]的限制範圍存取要求。 然而，中大部分的協力廠商連線服務 [!DNL Workfront Fusion] 沒有評估函，因此不符合 [!DNL Google] 辭彙。 因此， [!DNL Workfront Fusion] 不允許傳送資料給這些服務。

## 例外狀況至 [!DNL Google Services] 限制

有一些例外情況，可能會將資料傳送至沒有評定書的未經核准第三方服務，而不違反任何新限制。 兩者的差異主要在於 [!DNL G Suite] 使用 [!DNL Workfront Fusion] OAuth使用者端， [!DNL G Suite] 與其他OAuth使用者端，或 [!DNL @gmail.com] 和 [!DNL @google.mail.com].

* [[！DNL G suite]，搭配 [!DNL Workfront Fusion] Oauth使用者端](#g-suite-with-workfront-fusion-oauth-client)
* [使用其他OAuth使用者端的[！DNL G suite]](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] 和 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] 替換為 [!DNL Workfront Fusion] Oauth使用者端

[!DNL Workfront Fusion] 使用 [!UICONTROL 全網域安裝] 例外。 全網域安裝適用於 [!DNL G Suite] 允許使用者整合未核准的服務，沒有任何限制。 如果您是G Suite使用者，就不必執行任何其他步驟，且可以直接連線至未核准的服務。

### [!DNL G suite] 與其他OAuth使用者端

[!DNL G Suite] 偏好使用自己的OAuth使用者端而不使用 [!DNL Workfront Fusion] OAuth使用者端可以連線到 [!DNL Google Services] 透過 [!UICONTROL 內部] 使用方法。 此選項適用於進階使用者。 如需指示，請參閱 [Connect [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] 和 [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

具有存取權的使用者 [!DNL Google Services] 到 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 可以連線到 [!DNL Google Services] 透過「個人使用」方法。 此選項適用於進階使用者。 如需指示，請參閱 [Connect [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## 常見問題集

* [使用哪些應用程式 [!DNL Adobe Workfront Fusion] 是否會受到影響？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [我是否有[！DNL G Suite]帳戶？](#do-i-have-a-g-suite-account)
* [如果我是，怎麼辦 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 使用者？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [如果我是[！DNL G Suite]使用者，該怎麼辦？](#what-should-i-do-if-im-a-g-suite-user)

### 使用哪些應用程式 [!DNL Adobe Workfront Fusion] 是否會受到影響？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive]， [!DNL Gmail]，和電子郵件(已連線至 [!DNL Gmail] account)。

### 我是否有 [!DNL G Suite] 帳戶？ {#do-i-have-a-g-suite-account}

如果您的電子郵件地址結尾為 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您的帳戶不是 [!DNL G Suite] 帳戶。 若您的 [!DNL Google] 帳戶以自訂網域結尾，例如@my-company.com ，然後它就是 [!DNL G Suite] 帳戶。

### 如果我是，怎麼辦 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 使用者？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

這些新限制僅適用於整合時 [!DNL Google Drive] 或 [!DNL Gmail]. 如果您想要連線到 [!DNL Google Drive] 或 [!DNL Gmail]，您可以

* 切換至 [!DNL G Suite]

  或

* 建立自訂OAuth使用者端。 此選項適用於進階使用者。

  如需指示，請參閱 [Connect [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

如果您想要整合任何其他服務，但 [!DNL Google Drive] 或 [!DNL Gmail]，這些限制不適用。

如需關於連線其他裝置的說明 [!DNL Google Services] 至 [!DNL Workfront Fusion]，請參閱 [將模組的應用程式或Web服務連線至 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 在文章中 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 如果我是 [!DNL G Suite] 使用者？ {#what-should-i-do-if-im-a-g-suite-user}

沒有必要的動作。
