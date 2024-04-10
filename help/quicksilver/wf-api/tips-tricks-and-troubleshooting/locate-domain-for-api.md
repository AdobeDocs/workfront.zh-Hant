---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API呼叫的網域格式
description: 找出您的網域以用於Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# Adobe Workfront API呼叫的網域格式

當您對Workfront API進行API呼叫時，您會在呼叫中使用組織的網域。 此網域URL的格式會根據您的組織是否已上線到AdobeUnified Shell而不同。

若要知道您的組織是否位在AdobeUnified Shell上，請檢查您檢視Workfront頁面時顯示的URL。

| Workfront URL開頭為： | API呼叫的URL： |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

若要尋找您的網域：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 選取 **系統**，然後選取 **客戶資訊**.

   您的網域會列在畫面的右側。

   ![網域](assets/domain.png)

