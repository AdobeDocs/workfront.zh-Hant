---
product-area: documents
navigation-topic: documents-navigation-topic
title: Adobe Workfront中的C2PA中繼資料
description: 瞭解什麼是C2PA中繼資料，以及Adobe Workfront如何將其保留在您上傳、儲存和下載的檔案上。
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 3510218fb179a0852ad22abe2a753ccdb261205a
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 0%

---

# Adobe Workfront中的C2PA中繼資料

C2PA中繼資料是安全、容易被篡改的資訊，會隨內容一起移動。 當使用generative AI (GenAI)建立或變更影像、視訊或音訊檔案時，C2PA中繼資料會記錄該事實，以便收到檔案的任何人都可以檢視其製作方式。

C2PA中繼資料是以開啟的[C2PA](https://c2pa.org/)標準為基礎。

## C2PA中繼資料包含什麼

C2PA中繼資料包括：

* 提供GenAI工具的提供者名稱。
* 用來建立或更改內容的GenAI系統的名稱和版本號。
* 建立或修改內容的日期和時間。
* 唯一識別碼。

C2PA中繼資料不包含任何個人識別資訊(PII)。

## Workfront如何處理C2PA中繼資料

Adobe Workfront不會修改您使用之檔案的中繼資料。 當您上傳已載入C2PA中繼資料的檔案時，Workfront會保留該資訊，因為檔案儲存在Workfront中並從下載。

由於中繼資料內嵌在檔案本身中，透過Workfront工作流程保持不變，因此當其離開Workfront時，來源資訊會與內容一併保留。
