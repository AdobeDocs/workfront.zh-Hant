---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS登出URL無法運作
description: 本頁所述的程式僅適用於尚未加入Adobe Admin Console的組織。
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
TQID: https://experienceleague.adobe.com/RRaLL70JcSBcvoS6EUFuWj5Ejwljekt4QuQ3kXDx-44
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 250
ht-degree: 6%

---

# ADFS登出URL無法運作

<!-- Audited: 1/2024 -->

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>此頁面上說明的程式僅適用於尚未加入[!UICONTROL Adobe Admin Console]的組織。
>
>由於所有組織現在都已上線至Adobe Admin Console，本文不久將會移除。
>
>如果您的組織已加入[!UICONTROL Adobe Admin Console]，請參閱[平台式管理差異([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

## 問題

使用ADFS登出URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)時，您會收到一個訊息頁面，其中包含錯誤：「存取網站時發生問題。 請再次嘗試瀏覽網站。」

如果問題仍然存在，請連絡此網站的系統管理員，並提供下列參考號碼以識別問題： **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront]套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront]授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td>  
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解決方案

1. 在您的ADFS管理員伺服器中，移至&#x200B;**[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信任]** > `<your party trust>`屬性。

1. 在&#x200B;**[!UICONTROL 端點]**&#x200B;標籤下，按一下&#x200B;**[!UICONTROL 新增]**。

1. **[!UICONTROL 端點型別]** = SAML登出，繫結= POST，URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   如果您想要將回應URL重新導向至其他頁面，可設定回應URL。 但是我們建議您使用ADFS網站，因為它會警告您已經登出，但您仍應關閉瀏覽器。
