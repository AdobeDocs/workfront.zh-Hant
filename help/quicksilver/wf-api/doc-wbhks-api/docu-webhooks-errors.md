---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 檔案Webhooks錯誤處理
description: 檔案Webhooks錯誤處理
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
TQID: https://experienceleague.adobe.com/KoMJXXZbDdywLGIwYTu7o8GigPxQ5RG6sNQpOTMHWY0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 0%

---

# 檔案Webhooks錯誤處理

處理API請求時可能會出現問題。 所有API端點都應以一致的方式處理此問題。 發生錯誤時，webhook提供者應在回應標頭中包含錯誤代碼。 錯誤碼包括：

* 403 — 禁止。 指出要求權杖遺失或無效，或是與權杖關聯的認證無權存取指定的資源。 對於以OAuth為基礎的webhook提供者，Adobe Workfront將嘗試擷取新的存取權杖。

* 404 — 找不到。 表示指定的檔案或資料夾不存在。

* 500 — 內部伺服器錯誤。 任何其他型別的錯誤。

* 回應本文中的錯誤說明，格式如下：

  ```
  {status: "error"
   error: "Sample error message"}
  ```
