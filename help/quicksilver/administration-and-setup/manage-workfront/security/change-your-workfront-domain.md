---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 變更Adobe Workfront網域
description: 身為Adobe Workfront管理員和授權Workfront支援連絡人，您可以向Workfront支援團隊要求協助，以變更組織的Workfront網域。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b413ffc2416439629e073b32b5e9828df2f5de90
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 變更Adobe Workfront網域

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>若要在您的組織已上線至Adobe Workfront時變更Adobe Admin Console網域，請參閱 [設定網域](https://helpx.adobe.com/enterprise/using/set-up-identity.html#setup-domains).
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

身為Adobe Workfront管理員和授權Workfront支援連絡人，您可以向Workfront支援團隊要求協助，以變更組織的Workfront網域。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 請求網域變更

1. 按一下 **支援** 標籤，然後開始建立支援案例。
1. 在 **說明** 框中，包括所需的新域以及希望新域上線的時間範圍。
1. 完成為支援案例填寫框，然後按一下 **提交**.

您也可以呼叫Workfront支援，以取得變更網域的協助。

## 如果您是SSO客戶，請更新新網域

如果貴公司採用SSO，變更Workfront網域後，需執行下列步驟。

>[!NOTE]
>
>如果貴組織的Workfront執行個體已透過Adobe IMS啟用，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側邊欄中，按一下 **系統** > **客戶資訊** 並確認「客戶資訊」頁面上已更新您的網域。

1. 在左側邊欄中，按一下 **系統** > **單一登入(SSO)**.

1. 按一下 **下載SAML 2.0中繼資料**.
1. 下載檔案後，請開啟它，並確認下列事項：

   1. **entityID** 指向新域。
   1. 內的所有位置 **`<md:AssertionConsumerService>`** 指向新域。

1. 將下載的中繼資料檔案提供給您的身分提供者，讓對方能在結尾更新。
1. 請確定貴組織所使用所有Workfront整合的網域均已更新。
