---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '錯誤：由於各種錯誤，SSO使用者無法登入 [!DNL Adobe Workfront] '
description: 當您收到有關同盟單一登入的登入錯誤時，您的使用者名稱/密碼組合或您對 [!DNL Workfront], the problem might be that your [!DNL Workfront] 執行個體的存取使用SSO，而您嘗試使用不正確的URL登入。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# 錯誤：由於各種錯誤，SSO使用者無法登入[!DNL Adobe Workfront]

## 問題

我無法登入[!DNL Workfront]，並收到下列其中一個錯誤：

* 很抱歉，您無法透過登入畫面存取[!DNL Workfront]。 [!DNL Workfront]已設定為同盟單一登入搭配SAML 2.0。請連絡您的[!DNL Workfront]管理員。
* 該使用者名稱/密碼組合不正確。 請確定大寫鎖定未開啟，然後再試一次。
* 很抱歉，您沒有[!DNL Workfront]的存取權。 請連絡您的[!DNL Workfront]管理員以取得使用者名稱和密碼。

## 解決方案

您的[!DNL Workfront]執行個體使用SSO，而您正嘗試透過不正確的URL登入。 請確定您使用URL登入，且未使用「.com」之後的任何內容

>[!TIP]
>
>移除具有無效URL的任何現有書籤。
