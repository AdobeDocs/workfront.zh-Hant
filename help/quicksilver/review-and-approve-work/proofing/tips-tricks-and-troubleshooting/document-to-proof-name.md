---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 上傳後檔名稱已變更，且包含無效字元
description: 某些檔案無法轉換為校樣。
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

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
