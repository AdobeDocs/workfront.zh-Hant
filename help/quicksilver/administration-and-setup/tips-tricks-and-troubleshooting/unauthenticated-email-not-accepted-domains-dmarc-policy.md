---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 因網域的DMARC原則而不接受已驗證的電子郵件時
description: 如果從 [!DNL Workfront] 由於域的DMARC策略，系統未被接受，因此您的電子郵件管理員可以通過配置電子郵件系統以允許來自workfront.com的所有電子郵件來解決此問題。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 由於網域的DMARC原則，未驗證的電子郵件不會接受

## 問題

[測試] 我收到以下退信電子郵件：

550-5.7.1來自「customer domain.com」的未驗證電子郵件由於\
550-5.7.1域的DMARC政策。 請聯繫「customer domain.com」的管理員\
550-5.7.1域（如果這是合法郵件）。 請造訪\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) 了解DMARC\
550 5.7.1倡議。

## 解決方案

DMARC是在您公司的電子郵件系統中設定，且不屬於 [!DNL Adobe Workfront]. 如果您收到此電子郵件，則需要聯絡您的電子郵件管理員。

您的電子郵件管理員應將您的電子郵件系統配置為允許/信任來自noreply@workfront.com的電子郵件，或最好是所有來自workfront.com的電子郵件。

有關DMARC的詳細資訊，請參見 [https://support.google.com/mail/answer/2451690。](https://support.google.com/mail/answer/2451690)
