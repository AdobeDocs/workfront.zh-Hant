---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 當已驗證的電子郵件因網域的DMARC原則而不被接受時
description: 如果由於網域的DMARC原則而無法接受從 [!DNL Workfront] 系統傳送的電子郵件，您的電子郵件管理員可以設定您的電子郵件系統以允許來自workfront.com的所有電子郵件，以修正此問題。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 由於網域的DMARC原則，未驗證的電子郵件不被接受

## 問題

[測試]我收到下列退回電子郵件：

550-5.7.1不接受來自「customer domain.com」未經驗證的電子郵件，原因如下\
550-5.7.1網域的DMARC原則。 請聯絡「customer domain.com」的管理員\
550-5.7.1網域（如果這是合法郵件）。 請造訪\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690)瞭解DMARC\
550 5.7.1方案。

## 解決方案

DMARC是在您公司的電子郵件系統中設定的，不是[!DNL Adobe Workfront]的一部分。 如果您收到這封電子郵件，則需要連絡您的電子郵件管理員。

您的電子郵件管理員應將您的電子郵件系統設定為允許/信任來自noreply@workfront.com的電子郵件，或最好是所有來自workfront.com的電子郵件。

如需有關DMARC的詳細資訊，請參閱[https://support.google.com/mail/answer/2451690。](https://support.google.com/mail/answer/2451690)
