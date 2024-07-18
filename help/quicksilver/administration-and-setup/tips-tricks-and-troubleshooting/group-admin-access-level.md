---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 群組管理員的存取權必須高於其管理的群組
description: 如果群組管理員的存取層級許可權低於其管理的許可權，他們將無法檢視、修改或指派較低的存取層級。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: 0ca335bf0db934d23f607d3f8ce7cfb67e629053
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# 群組管理員的存取權必須高於其管理的群組

如果群組管理員的存取層級許可權低於其管理的許可權，他們將無法檢視、修改或指派較低的存取層級。

## 問題

如果群組管理員被指派了具有團隊檢視許可權的修改規劃者存取層級，但某些使用者被指派了具有團隊編輯許可權的工作者存取層級，則群組管理員將無法與修改的工作者存取層級互動。

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>此邏輯也適用於微調您的設定下拉式選單。 這兩個存取層級都可以擁有「編輯」存取權，但「微調您的設定」下拉式選單中的設定值對群組管理員而言必須更高。
> ![](assets/fine-tune-your-settings.png)

## 解決方案

群組管理員在存取層級中所有區域的許可權必須高於其管理的許可權。
