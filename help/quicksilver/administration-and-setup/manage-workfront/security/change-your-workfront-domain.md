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
source-git-commit: b9e088a0cdb32f3e8c565ea17f4613dda104bd7b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# 變更您的Adobe Workfront網域

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於尚未加入Admin Console的組織。 如果貴組織已上線Adobe Admin Console，則無法變更您的Workfront網域。
>
>如需根據貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台式管理差異(Adobe Workfront/Adobe商務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請洽詢Workfront管理員，瞭解他們是否對您的存取層級設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 要求網域變更

1. 按一下 **支援** 索引標籤上的「 Workfront One 」頁面，然後開始建立支援案例。
1. 在 **說明** 方塊中，加入您想要的新網域，以及您想要新網域上線的時間範圍。
1. 完成填寫支援案例的方塊，然後按一下 **提交**.

您也可以致電Workfront支援，取得變更網域的協助。

## 如果您是SSO客戶，請更新新網域

如果您的公司使用SSO，在您變更Workfront網域後，需要執行下列步驟。

>[!NOTE]
>
>如果您組織的Workfront執行個體已啟用Adobe IMS，則無法使用此選項。 如需詳細資訊，請洽詢您的網路或IT管理員。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側邊欄中，按一下 **系統** > **客戶資訊** 並確保您的網域已更新至客戶資訊頁面。

1. 在左側邊欄中，按一下 **系統** > **單一登入(SSO)**.

1. 按一下 **下載SAML 2.0中繼資料**.
1. 下載檔案後，請開啟檔案並確認以下事項：

   1. **entityid** 指向新網域。
   1. 內的所有位置 **`<md:AssertionConsumerService>`** 指向新領域。

1. 將下載的中繼資料檔案提供給您的身分提供者，以便他們可以在身分提供者端更新該檔案。
1. 請確定您的組織使用的所有Workfront整合的網域已更新。
