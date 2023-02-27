---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook概述
description: Webhook概述
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Webhook概述

Adobe Workfront Document Webhook定義了一組API端點，Workfront會透過此端點向外部檔案提供者發出授權API呼叫。 這可讓任何人為任何檔案儲存提供者建立中間件外掛程式。

![](assets/mceclip0-350x262.png)

網頁連結型整合的使用者體驗將類似於現有的檔案整合，例如Google Drive、Box和Dropbox。 例如，Workfront使用者將能執行下列動作：

* 導航外部文檔提供程式的資料夾結構
* 搜尋檔案
* 將檔案連結至Workfront
* 將檔案上傳到外部文檔提供程式
* 查看文檔的縮略圖

**參考實作**

為協助快速開發新Webhook實作，Workfront提供參考實作。 此項目的程式碼位於 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . 此實作以Java為基礎，可讓Workfront連線網路檔案系統上的檔案。 

## 版本

* 1.0版（發行日期 — 2015年5月）:初始規格

* 版本1.1（發行日期 — 2015年6月）。 更新/uploadInit — 新增documentId和documentVersionId

* 1.2版（發行日期 — 2015年10月）:新增/createFolder

* 即將推出的版本（發行日期 — 待定）:

   * 新增/刪除
   * 新增/重新命名
   * 新增/serviceInfo
   * 新增/customAction
   * 新增分頁和parentId至/search
