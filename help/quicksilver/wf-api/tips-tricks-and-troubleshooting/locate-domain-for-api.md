---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API呼叫的網域格式
description: 找出您的網域以用於Adobe Workfront API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: e9a9e45720c8b9ad25e3fa9340c813a73989fb4a
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 1%

---

# Adobe Workfront API呼叫的網域格式

當您對Workfront API進行API呼叫時，您會在呼叫中使用組織的網域。 此網域URL的格式會根據您的組織是否已上線到Adobe Unified Shell而不同。

若要知道您的組織是否位在Adobe Unified Shell上，請檢查檢視Workfront頁面時顯示的URL。

| Workfront URL開頭為： | API呼叫的URL： |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


若要尋找您的網域：

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 選取&#x200B;**系統**，然後選取&#x200B;**客戶資訊**。

   您的網域會列在畫面的右側。

   ![網域](assets/domain.png)

