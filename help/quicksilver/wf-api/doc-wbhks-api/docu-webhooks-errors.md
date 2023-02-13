---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文檔Webhook錯誤處理
description: 文檔Webhook錯誤處理
author: John
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# 文檔Webhook錯誤處理

處理API請求時可能會產生問題。 這應在所有API端點間以一致的方式處理。 發生錯誤時，Webhook提供程式應在回應標題中包含錯誤代碼。 錯誤代碼包括：

* 403 — 禁止。 指出要求Token遺失或無效，或與Token相關聯的認證無權存取指定的資源。 針對OAuth型網頁連結提供者，Adobe Workfront會嘗試擷取新的存取權杖。

* 404 — 找不到。 指示指定的檔案或資料夾不存在。

* 500 — 內部伺服器錯誤。 任何其他類型的錯誤。

* 回應內文中錯誤的說明，使用下列格式：

   ```
   {status: “error”
    error: “Sample error message”}
   ```
