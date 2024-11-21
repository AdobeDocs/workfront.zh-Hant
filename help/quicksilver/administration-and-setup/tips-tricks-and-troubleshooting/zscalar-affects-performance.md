---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScalar設定可能會導致效能降低
description: 建立使用者後，您可以編輯使用者並啟用「僅允許SAML 2.0驗證」，以便其使用者和密碼由SAML系統控制。 啟用此選項後，使用者只能透過SAML登入。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront： ZScalar設定可能會導致效能降低

>[!NOTE]
>
>這是ZScalar的問題，Workfront將不會修正。

ZScalar的Web服務預設使用`http/1.1`，這會導致Workfront中的效能降低。

若要檢查並解決此問題，請將您的ZScalar軟體設定為使用`http/2`。 無法在Workfront中設定此專案。

您可以在ZScalar檔案中找到有關`http/2`的資訊。
