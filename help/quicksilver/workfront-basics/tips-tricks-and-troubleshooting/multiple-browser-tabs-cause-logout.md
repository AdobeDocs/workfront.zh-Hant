---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 多個瀏覽器分頁導致Workfront登出
description: 當使用者開啟多個瀏覽器標籤時，Workfront 可能會自動登出。
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 32%

---

# 多個瀏覽器分頁導致Workfront登出

## 問題

當使用者開啟了多個瀏覽器索引標籤，並按一下進入已停用一段時間的分頁時，索引標籤工作階段已過期。 使用者看不到他們開啟的頁面，而是看到以下訊息：

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## 原因

此行為是由原則型驗證(PBA)所造成，這是貴組織所設定的安全性測量。 當索引標籤的非作用中時間超過您組織的PBA設定中所設定的時間限制時，索引標籤工作階段就會過期。

## 解決方案

解決方案取決於您是否已在登入Workfront的其他索引標籤中處於作用中狀態。

* 如果您開啟了啟用中的 Workfront 索引標籤，請重新載入過期的索引標籤。系統會返回您在索引標籤過期之前開啟的頁面。

* 如果您沒有開啟啟用中的 Workfront 索引標籤，請重新登入 Workfront。
