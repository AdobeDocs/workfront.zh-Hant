---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront使用者認證與SAML使用者認證的比較
description: 建立使用者後，您可以編輯使用者並啟用「僅允許SAML 2.0驗證」，以便其使用者和密碼由SAML系統控制。 啟用此選項後，使用者只能透過SAML登入。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Adobe Workfront使用者認證與SAML使用者認證

本文專注於[!DNL Adobe Workfront]和SAML，並未涵蓋其他SSO驗證方法。

在資料庫中，[!DNL Workfront]會將eawch使用者的電子郵件地址儲存為其[!DNL Workfront]使用者名稱，以及其[!DNL Workfront]密碼。 這些憑證會在「預覽」和「自訂重新整理沙箱」中復寫。

在建立使用者期間，如果[!DNL Workfront]偵測到已設定SAML 2.0，則會預設為使用者「僅允許SAML 2.0驗證」。 如果已啟用[傳送邀請電子郵件給此人]方塊，[!DNL Workfront]會停用[僅允許SAML 2.0驗證]並隱藏此選項。 啟用「傳送邀請電子郵件給此人」後，使用者會成為非SAML [!DNL Workfront]使用者。

建立使用者之後，您可以編輯使用者並啟用&#x200B;**[!UICONTROL 僅允許SAML 2.0驗證]**，以便其使用者和密碼由SAML系統控制。

完成後，使用者只能透過SAML登入。 當他們前往[!DNL Workfront] URL時，系統會自動將他們重新導向至SAML系統，並提示您輸入SAML使用者名稱和密碼。

SAML憑證儲存在外部SAML系統(例如Microsoft的ADFS)中，而不是儲存在Workfront中。
