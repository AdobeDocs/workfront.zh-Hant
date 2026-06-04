---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler設定可能會導致效能降低
description: 建立使用者後，您可以編輯使用者並啟用「僅允許SAML 2.0驗證」，以便其使用者和密碼由SAML系統控制。 啟用此選項後，使用者只能透過SAML登入。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
TQID: https://experienceleague.adobe.com/-3-p8fzXIiV-gnjIjhRzBmLfspAEEVAuD2lpmcsVjLA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 44%

---

# Workfront：ZScaler 設定可能導致效能下降

>[!NOTE]
>
>這是 ZScaler 的問題，並不會由 Workfront 進行修正。

ZScaler Web 服務預設使用 `http/1.1`，這可能導致 Workfront 效能下降。

若要檢查並解決此問題，請將您的ZScaler軟體設定為使用`http/2`。 您無法在 Workfront 中進行此項設定。

您可以在 ZScaler 文件中找到有關 `http/2` 的資訊。
