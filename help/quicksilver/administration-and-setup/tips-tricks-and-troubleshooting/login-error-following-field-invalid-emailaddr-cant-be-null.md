---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 登入錯誤：下列欄位無效： emailAddr不可為空
description: 當我嘗試登入 [!DNL Adobe Workfront] 網域的URL時，系統會將我重新導向至SAML登入入口網站，然後再重新導向回 [!DNL Workfront] ，錯誤為emailAddr欄位不可為空。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 4%

---

# 登入錯誤：下列欄位無效： emailAddr不可為空

## 問題

當我嘗試使用我的URL (https://customerdomain.my.workfront.com)登入[!DNL Adobe Workfront]時，我被重新導向到SAML登入入口網站，然後重新導向回[!DNL Workfront]，並出現以下錯誤：

「請再試一次。 下列欄位無效： emailAddr不可以是Null。」

## 原因

此錯誤是由於SAML 2.0設定的「對應使用者屬性」區域中不正確的專案所導致。 如需有關對SAML 2.0的使用者屬性的詳細資訊，請參閱[使用SAML 2.0設定Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)。

## 解決方案

更新電子郵件地址的屬性對應，然後按一下&#x200B;**[!UICONTROL 儲存]**。
