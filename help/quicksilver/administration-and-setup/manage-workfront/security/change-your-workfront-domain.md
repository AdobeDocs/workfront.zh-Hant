---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 變更您的Adobe Workfront網域
description: 身為Adobe Workfront管理員和授權的Workfront支援聯絡人，您可以向Workfront支援團隊請求協助，以變更貴組織的Workfront網域。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: 22ea9b623d7bc7b216511538cf88e4d020529bd3
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 變更您的Adobe Workfront網域

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於尚未加入Admin Console的組織。 如果您的組織已上線Adobe Admin Console，則無法變更您的Workfront網域。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

身為Adobe Workfront管理員和授權的Workfront支援聯絡人，您可以向Workfront支援團隊請求協助，以變更貴組織的Workfront網域。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 要求網域變更

1. 在Experience League時開始建立支援票證。
1. 在&#x200B;**說明**&#x200B;方塊中，加入您想要的新網域，以及您想要新網域上線的時間範圍。
1. 完成填寫支援案例的方塊，然後按一下&#x200B;**提交**。

您也可以聯絡Workfront支援，取得變更網域的協助。

## 如果您是SSO客戶，請更新新網域

如果您的公司使用SSO，在您變更Workfront網域後需要下列步驟。

>[!NOTE]
>
>如果您組織的Workfront執行個體已啟用Adobe IMS，便無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側邊欄中，按一下&#x200B;**系統** > **客戶資訊**，並確定您的網域已更新至客戶資訊頁面。

1. 在左側邊欄中，按一下&#x200B;**系統** > **單一登入(SSO)**。

1. 按一下&#x200B;**下載SAML 2.0中繼資料**。
1. 下載檔案後，請開啟檔案並確認下列事項：

   1. **entityID**&#x200B;正在指向新網域。
   1. **`<md:AssertionConsumerService>`**&#x200B;內的所有位置都指向新網域。

1. 將下載的中繼資料檔案提供給您的身分提供者，以便他們可以在自己的終端進行更新。
1. 請確定您的組織使用的所有Workfront整合的網域都已更新。
