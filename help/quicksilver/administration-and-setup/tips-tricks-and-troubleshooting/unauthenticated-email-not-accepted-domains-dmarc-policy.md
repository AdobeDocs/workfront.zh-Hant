---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 由於網域的DMARC原則，未驗證的電子郵件不被接受
description: 如果因為網域的DMARC原則而不接受從 [!DNL Workfront] 系統傳送的電子郵件，您的電子郵件管理員可以設定您的電子郵件系統以允許來自workfront.com的所有電子郵件，以修正問題。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 177
ht-degree: 1%

---

# 由於網域的DMARC原則，未驗證的電子郵件不被接受

## 問題

[測試]我收到下列退回電子郵件：

550-5.7.1不接受來自「customer domain.com」未經驗證的電子郵件，原因如下\
550-5.7.1網域的DMARC原則。 請聯絡「customer domain.com」的管理員\
550-5.7.1網域（如果這是合法郵件）。 請造訪\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690)以瞭解DMARC\
550 5.7.1方案。

## 解決方案

DMARC已在您公司的電子郵件系統中設定，不是[!DNL Adobe Workfront]的一部分。 如果您收到這封電子郵件，則需要連絡您的電子郵件管理員。

您的電子郵件管理員應將您的電子郵件系統設定為允許/信任來自noreply@workfront.com的電子郵件，或最好是所有來自workfront.com的電子郵件。

如需DMARC的詳細資訊，請參閱[https://support.google.com/mail/answer/2451690。](https://support.google.com/mail/answer/2451690)
