---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 上傳後檔名稱已變更，且包含無效字元
description: 某些檔案無法轉換為校樣。
author: Courtney
source-git-commit: a01c2e42dad1a7c00ac73fcaeb1202c56238a8bb
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# 上傳後檔名稱已變更，且包含無效字元

## 問題

某些檔案無法轉換為校樣。

## 原因

上傳至Workfront的檔案無法在檔案名稱中包含某些字元。 如果檔案在檔案名稱中包含下列任一字元，則上傳檔案時，會從檔案名稱中移除這些字元： `! # % * \ | ' " / ? < > { } [ ]`.

如果檔名稱在初始上傳後更新為包含無效字元，則校樣產生將失敗。

## 解決方案

移除檔名稱中的無效字元：

1. 選取檔案，然後按一下 **檔案詳細資訊**.
1. 按一下檔名稱並移除無效字元，然後按Enter鍵。

   無效的字元： `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. 重新整理頁面並產生校訂。