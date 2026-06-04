---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks概觀
description: Webhooks概觀
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
TQID: https://experienceleague.adobe.com/5bBLva-jIjwc953MVjAnwo4y0nABq1N0HGDTIurXk40
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 193
ht-degree: 1%

---

# Webhooks概觀

Adobe Workfront Document Webhooks定義了一組API端點，Workfront會透過這些端點向外部檔案提供者發出授權的API呼叫。 這可讓任何人為任何檔案儲存提供者建立中介外掛程式。

![Webhooks](assets/mceclip0-350x262.png)

webhook型整合的使用者體驗將與現有檔案整合類似，例如Google Drive、Box和Dropbox。 例如，Workfront使用者將能夠執行下列動作：

* 瀏覽外部檔案提供者的檔案夾結構
* 搜尋檔案
* 將檔案連結至Workfront
* 將檔案上傳到外部檔案提供者
* 檢視檔案的縮圖

**參考實作**

為協助快速開始開發新的Webhook實作，Workfront提供參考實作的範例。您可以在[https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app)找到這些範例。範例以Java為基礎，可讓Workfront在網路檔案系統上連線檔案。 

>[!NOTE]
>
>GitHub上的資源僅為範例，無法執行實作。

## 版本

* 1.0版（發行日期 — 2015年5月）：初始規格

* 1.1版（發行日期 — 2015年6月）。 更新/uploadInit — 新增documentId和documentVersionId

* 1.2版（發行日期 — 2015年10月）：新增/createFolder

* 即將發行的版本（發行日期 — 待定）：

   * 已新增/delete
   * 新增/rename
   * 新增/serviceInfo
   * 新增/customAction
   * 將分頁與parentId新增至/search
