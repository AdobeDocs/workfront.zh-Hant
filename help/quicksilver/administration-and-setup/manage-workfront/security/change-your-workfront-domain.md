---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 變更您的Adobe Workfront網域
description: 身為Adobe Workfront管理員和授權的Workfront支援聯絡人，您可以向Workfront支援團隊請求協助，以變更貴組織的Workfront網域。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
TQID: https://experienceleague.adobe.com/g9H5AYcIdsVccGIU9U97QPa37J9Y3pXziZRQR7pvjpQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 11%

---

# 變更您的Adobe Workfront網域

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未加入Admin Console的組織。 因為所有組織現在都已加入Adobe Admin Console，**無法變更您的Workfront網域**。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱[Adobe Workfront與Adobe商務平台之間的管理差異](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。
>
>此文章將在不久的將來移除。

身為Adobe Workfront管理員和授權的Workfront支援聯絡人，您可以向Workfront支援團隊請求協助，以變更貴組織的Workfront網域。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 要求網域變更

1. 開始在Experience League上建立支援票證。
1. 在&#x200B;**說明**&#x200B;方塊中，加入您想要的新網域，以及您想要新網域上線的時間範圍。
1. 完成填寫支援案例的方塊，然後按一下&#x200B;**提交**。

您也可以聯絡Workfront支援，取得變更網域的協助。

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
