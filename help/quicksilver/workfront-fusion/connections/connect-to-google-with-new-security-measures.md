---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: connections-annd-webhooks
title: '使用更新的安全性措施連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] '
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# 使用更新的安全性措施將[!DNL Adobe Workfront Fusion]連線到[!DNL Google Services]

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [使用更新的安全性措施將Adobe Workfront Fusion連線到Google服務](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-to-google-with-new-security-measures.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

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

## [!DNL Google Services]個限制

自2020年6月1日起，[!DNL Google]已引進使用者如何使用其API的限制。 這些安全性措施可保護[!DNL Google]使用者不會在[!DNL Google]上洩漏或濫用其個人資料。 限制與[!DNL Gmail]和[!DNL Google Drive]應用程式有關。 如需這些限制的詳細資訊，請參閱[[!DNL Google] API服務使用者資料原則](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)中的「特定API範圍的其他需求」

若要存取受限制的範圍，必須驗證連線的服務（[!DNL Adobe Workfront Fusion]或要透過API存取使用者資料的任何其他服務），並且必須有評估信件，以證明服務在使用資料的方式上安全且透明。 [!DNL Workfront Fusion]符合[!DNL Google]所有存取受限制範圍的要求。 但是，[!DNL Workfront Fusion]中大部分的協力廠商連線服務沒有評定函，因此不符合[!DNL Google]條款。 因此，不允許[!DNL Workfront Fusion]傳送資料給這些服務。

## [!DNL Google Services]限制的例外

有一些例外情況可能會將資料傳送至未核准的第三方服務，該服務沒有評定函，但不會違反任何新限制。 兩者差異在於具有[!DNL Workfront Fusion] OAuth使用者端的[!DNL Google Workspace]、具有其他OAuth使用者端的[!DNL Google Workspace]或[!DNL @gmail.com]與[!DNL @google.mail.com]。

* [[!DNL Google Workspace]具有 [!DNL Workfront Fusion] OAuth使用者端](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace]與其他OAuth使用者端](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com]和 [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### 具有[!DNL Workfront Fusion] OAuth使用者端的[!DNL Google Workspace]

[!DNL Workfront Fusion]使用[!UICONTROL 全網域安裝]例外狀況。 全網域安裝適用於[!DNL Google Workspace]位使用者，可讓使用者整合未經核准的服務，沒有任何限制。 如果您是Google Workspace使用者，不必執行任何其他步驟，可以直接連線至未核准的服務。

### [!DNL Google Workspace]與其他OAuth使用者端

[!DNL Google Workspace]使用者若偏好使用自己的OAuth使用者端而不使用[!DNL Workfront Fusion] OAuth使用者端，可以透過[!UICONTROL 內部]使用方法連線至[!DNL Google Services]。 此選項適用於進階使用者。 如需指示，請參閱[使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 。

### [!DNL @gmail.com]和[!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

透過[!DNL @gmail.com]或[!DNL @googlemail.com]存取[!DNL Google Services]的使用者可以透過「個人使用」方法連線到[!DNL Google Services]。 此選項適用於進階使用者。 如需指示，請參閱[使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 。

## 常見問題集

* [ [!DNL Adobe Workfront Fusion] 中的哪些應用程式會受到影響？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [我是否有 [!DNL Google Workspace] 帳戶？](#do-i-have-a-g-suite-account)
* [如果我是 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 使用者，怎麼辦？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [如果我是 [!DNL Google Workspace] 使用者，怎麼辦？](#what-should-i-do-if-im-a-g-suite-user)

### [!DNL Adobe Workfront Fusion]中的哪些應用程式會受到影響？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive]、[!DNL Gmail]和電子郵件（已連線至[!DNL Gmail]帳戶）。

### 我是否有[!DNL Google Workspace]帳戶？ {#do-i-have-a-g-suite-account}

如果您的電子郵件地址結尾是[!DNL @gmail.com]或[!DNL @googlemail.com]，則您的帳戶不是[!DNL Google Workspace]帳戶。 如果您的[!DNL Google]帳戶以自訂網域(例如@my-company.com)結尾，則它是[!DNL Google Workspace]帳戶。

### 如果我是[!DNL @gmail.com]或[!DNL @googlemail.com]使用者，怎麼辦？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

這些新限制只適用於整合[!DNL Google Drive]或[!DNL Gmail]的情況。 如果您想要連線到[!DNL Google Drive]或[!DNL Gmail]，您可以

* 切換至[!DNL Google Workspace]

  或

* 建立自訂OAuth使用者端。 此選項適用於進階使用者。

  如需指示，請參閱[使用自訂OAuth使用者端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)連線 [!DNL Adobe Workfront Fusion] 至 [!DNL Google Services] 。

如果您想要整合[!DNL Google Drive]或[!DNL Gmail]以外的任何服務，則這些限制不適用。

如需有關將其他[!DNL Google Services]連線到[!DNL Workfront Fusion]的說明，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立情境[將模組的應用程式或Web服務連線到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect)。

### 如果我是[!DNL Google Workspace]使用者，怎麼辦？ {#what-should-i-do-if-im-a-g-suite-user}

沒有必要的動作。
