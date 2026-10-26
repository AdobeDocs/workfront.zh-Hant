---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 登入錯誤：下列欄位無效： emailAddr不可為空
description: 當我嘗試登入[!DNL Adobe Workfront]我的網域的URL時，我被重新導向到SAML登入入口網站，然後重新導向回[!DNL Workfront]，錯誤是emailAddr欄位不能為null。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: 'https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: e7123179a59cd7ed9c76f4718b3b8019854cbfe1
workflow-type: tm+mt
source-wordcount: '77'
ht-degree: 0%
---
# 登入錯誤：下列欄位無效： emailAddr不可為空

>[!IMPORTANT]
>
>由於登入現在透過Adobe IMS （Identity Management系統）處理，因此已移除本文中的資訊。

<!--

## Problem

When I try to log into [!DNL Adobe Workfront] with my URL (https://customerdomain.my.workfront.com), I am redirected to the SAML login portal and then redirected back to [!DNL Workfront] with the following error:

"Let's try that again. The following fields are invalid: emailAddr cannot be null."

## Cause

This error is caused by an incorrect item in the Map User Attributes area of the SAML 2.0 configuration. For more information about mapping user attributes for SAML 2.0, see [Configure Adobe Workfront with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solution

Update the Attribute Mapping for the email address, and click **[!UICONTROL Save]**.

-->
