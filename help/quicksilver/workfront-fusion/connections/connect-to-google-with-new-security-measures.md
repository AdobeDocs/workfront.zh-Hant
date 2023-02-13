---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 更新了安全措施
description: Google最近推出限制，限制使用者使用其API的方式。 本文說明如何連線 [!DNL Adobe Workfront Fusion] 到Google，說明這些更新的安全措施。
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 更新了安全措施

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

## [!DNL Google Services] 限制

[!DNL Google] 自2020年6月1日起，已對使用者使用其API的方式實行限制。 這些安全措施 [!DNL Google] 使用者的個人資料被洩露或濫用 [!DNL Google]. 限制與 [!DNL Gmail] 和 [!DNL Google Drive] 應用程式。 如需這些限制的詳細資訊，請參閱 [[!DNL Google] API服務用戶資料策略](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

要訪問受限範圍，已連接的服務([!DNL Adobe Workfront Fusion] 或任何其他想透過API存取使用者資料的服務)，必須經過驗證，且必須有評估函，以證明服務是安全且透明的，說明其使用資料的方式。 [!DNL Workfront Fusion] 遵守所有 [!DNL Google]對訪問受限作用域的要求。 然而，大部分的協力廠商 [!DNL Workfront Fusion] 沒有評估書，因此不符合 [!DNL Google] 詞語。 因此， [!DNL Workfront Fusion] 不允許將資料傳送至這些服務。

## 例外 [!DNL Google Services] 限制

有一些例外，使得可以在不違反任何新限制的情況下，將資料發送到未批准的第三方服務，該服務沒有評估函。 不同之處在於 [!DNL G Suite] 和 [!DNL Workfront Fusion] OAuth用戶端， [!DNL G Suite] 與另一個OAuth用戶端，或 [!DNL @gmail.com] 和 [!DNL @google.mail.com].

* [使用 [!DNL Workfront Fusion] OAuth用戶端](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite]搭配另一個OAuth用戶端](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] 和 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] with [!DNL Workfront Fusion] OAuth用戶端

[!DNL Workfront Fusion] 使用 [!UICONTROL 全域安裝] 例外。 域範圍安裝適用於 [!DNL G Suite] 使用者，且可讓使用者整合未核准的服務，沒有任何限制。 如果您是G Suite使用者，則不需要執行任何其他步驟，且可直接連線至未核准的服務。

### [!DNL G suite] 與另一個OAuth用戶端

[!DNL G Suite] 偏好使用自己的OAuth用戶端，而非使用 [!DNL Workfront Fusion] OAuth用戶端可連線至 [!DNL Google Services] 通過 [!UICONTROL 內部] 使用方法。 此選項適用於進階使用者。 如需指示，請參閱 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] 和 [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

存取 [!DNL Google Services] through [!DNL @gmail.com] 或 [!DNL @googlemail.com] 可連線至 [!DNL Google Services] 透過個人使用方法。 此選項適用於進階使用者。 如需指示，請參閱 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## 常見問題集

* [中的應用程式 [!DNL Adobe Workfront Fusion] 是否受影響？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [我是否有[!DNL G Suite]帳戶？](#do-i-have-a-g-suite-account)
* [如果我 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 使用者？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [如果我是[!DNL G Suite]使用者，該怎麼辦？](#what-should-i-do-if-im-a-g-suite-user)

### 中的應用程式 [!DNL Adobe Workfront Fusion] 是否受影響？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]，以及電子郵件(已連線至 [!DNL Gmail] 帳戶)。

### 我有 [!DNL G Suite] 帳戶？ {#do-i-have-a-g-suite-account}

如果您的電子郵件地址結尾是 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您的帳戶不是 [!DNL G Suite] 帳戶。 若您的 [!DNL Google] 帳戶以自訂網域(例如@my-company.com)結尾，則為 [!DNL G Suite] 帳戶。

### 如果我 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 使用者？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

只有在您整合 [!DNL Google Drive] 或 [!DNL Gmail]. 如果您想連線至 [!DNL Google Drive] 或 [!DNL Gmail]，您可以

* 切換至 [!DNL G Suite]

   或

* 建立自訂OAuth用戶端。 此選項適用於進階使用者。

   如需指示，請參閱 [Connect [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自訂OAuth用戶端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

如果您想整合以外的任何其他服務 [!DNL Google Drive] 或 [!DNL Gmail]，則不適用這些限制。

有關連接其他 [!DNL Google Services] to [!DNL Workfront Fusion]，請參閱 [將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 在文章中 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 如果我是 [!DNL G Suite] 使用者？ {#what-should-i-do-if-im-a-g-suite-user}

沒有必要的動作。
