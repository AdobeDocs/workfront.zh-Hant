---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 多個瀏覽器分頁導致Workfront登出
description: 當使用者開啟多個瀏覽器標籤時，Workfront 可能會自動登出。
feature: Get Started with Workfront
source-git-commit: ef85b267b3417dddd0c9cc4a2b916b83dc416e14
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 7%

---

# 多個瀏覽器分頁導致Workfront登出

>[!IMPORTANT]
>
>只有已上線Adobe IMS的組織才會出現此問題。

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

* 如果您有作用中的Workfront標籤開啟，請重新載入過期的標籤。 它會傳回至您過期前開啟的頁面。

* 如果您沒有開啟作用中的Workfront索引標籤，請重新登入Workfront。