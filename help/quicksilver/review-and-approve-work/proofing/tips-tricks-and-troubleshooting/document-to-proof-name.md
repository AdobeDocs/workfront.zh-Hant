---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 上傳後檔名稱已變更，且包含無效字元
description: 某些檔案無法轉換為校樣。
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
ht-degree: 1%

---

# 上傳後檔名稱已變更，且包含無效字元

## 問題

某些檔案無法轉換為校樣。

## 原因

上傳至Workfront的檔案無法在檔案名稱中包含某些字元。 如果檔案在檔案名稱中包含下列任何字元，則檔案上傳時這些字元會從檔案名稱中移除： `! # % * \ | ' " / ? < > { } [ ]`。

如果檔名稱在初始上傳後更新為包含無效字元，則校樣產生將失敗。

## 解決方案

移除檔名稱中的無效字元：

1. 選取檔案，然後按一下&#x200B;**檔案詳細資料**。
1. 按一下檔名稱並移除無效字元，然後按Enter鍵。

   無效的字元： `! # % * \ | ' " / ? < > { } [ ]`

   ![檔名稱](assets/doc-name.png)

1. 重新整理頁面並產生校訂。
