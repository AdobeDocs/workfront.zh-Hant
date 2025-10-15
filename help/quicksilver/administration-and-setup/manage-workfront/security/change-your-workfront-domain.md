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
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# 變更您的Adobe Workfront網域

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未加入Admin Console的組織。 如果您的組織已上線Adobe Admin Console，則無法變更您的Workfront網域。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

身為Adobe Workfront管理員和授權的Workfront支援聯絡人，您可以向Workfront支援團隊請求協助，以變更貴組織的Workfront網域。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
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

## 如果您是SSO客戶，請更新新網域

如果您的公司使用SSO，在您變更Workfront網域後需要下列步驟。

>[!NOTE]
>
>如果您組織的Workfront執行個體已啟用Adobe IMS，便無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

{{step-1-to-setup}}

1. 在左側邊欄中，按一下&#x200B;**系統** > **客戶資訊**，並確定您的網域已更新至客戶資訊頁面。

1. 在左側邊欄中，按一下&#x200B;**系統** > **單一登入(SSO)**。

1. 按一下&#x200B;**下載SAML 2.0中繼資料**。
1. 下載檔案後，請開啟檔案並確認下列事項：

   1. **entityID**&#x200B;正在指向新網域。
   1. **`<md:AssertionConsumerService>`**&#x200B;內的所有位置都指向新網域。

1. 將下載的中繼資料檔案提供給您的身分提供者，以便他們可以在自己的終端進行更新。
1. 請確定您的組織使用的所有Workfront整合的網域都已更新。
