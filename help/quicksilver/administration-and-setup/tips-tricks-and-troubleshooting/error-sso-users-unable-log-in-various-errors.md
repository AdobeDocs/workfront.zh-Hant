---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''錯誤：SSO用戶無法登錄 [!DNL Adobe Workfront] 由於各種錯誤'
description: 當您收到同盟單一登入、使用者名稱/密碼組合的登入錯誤，或您對 [!DNL Workfront], the problem might be that your [!DNL Workfront] 執行個體使用SSO，而您正嘗試使用錯誤的URL登入。 請確定您是使用正確的URL登入，且「.com」後面沒有任何項目。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 9%

---

# 錯誤：SSO用戶無法登錄 [!DNL Adobe Workfront] 由於各種錯誤

## 問題

我無法登入 [!DNL Workfront] 並收到以下錯誤之一：

* 抱歉，您無法訪問 [!DNL Workfront] 透過此登入畫面。 [!DNL Workfront] 已針對使用SAML 2.0的Federated Single Sign-On進行設定。請連絡您的 [!DNL Workfront] 管理員。
* 該使用者/密碼組合不正確。請確定大寫鎖定未開啟。
* 抱歉，您無權訪問 [!DNL Workfront]. 請連絡您的 [!DNL Workfront] 管理員，以取得使用者名稱和密碼。

## 解決方案

您的 [!DNL Workfront] 執行個體使用SSO，而您正嘗試透過錯誤的URL登入。 請確定您是使用正確的URL登入，且「.com」後面沒有任何項目

>[!TIP]
>
>移除任何具有無效URL的現有書籤。
