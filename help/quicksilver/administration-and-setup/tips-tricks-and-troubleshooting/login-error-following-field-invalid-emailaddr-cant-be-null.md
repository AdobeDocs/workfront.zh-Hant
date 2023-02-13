---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '登錄錯誤：下列欄位無效：emailAddr不能為null'
description: 當我嘗試登入 [!DNL Adobe Workfront] 網域的URL會重新導向至SAML登入入口網站，然後重新導向回 [!DNL Workfront] emailAddr欄位不能為null的錯誤。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# 登錄錯誤：下列欄位無效：emailAddr不能為null

## 問題

當我嘗試登入 [!DNL Adobe Workfront] 透過URL(https://customerdomain.my.workfront.com)，系統會將我重新導向至SAML登入入口網站，然後重新導向回 [!DNL Workfront] 錯誤：

「請再試一次。下列欄位無效：emailAddr不能為null。」

## 原因

此錯誤是由SAML 2.0設定的「對應使用者屬性」區域中的錯誤項目所造成。 如需有關對應SAML 2.0使用者屬性的詳細資訊，請參閱 [使用SAML 2.0設定Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## 解決方案

更新電子郵件地址的屬性映射，然後按一下 **[!UICONTROL 儲存]**.
