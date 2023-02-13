---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 依IP位址限制Adobe Workfront的存取權
description: 您可以設定Adobe Workfront IP允許清單，限制對您指定之45個IP位址或IP位址範圍的存取。 這為Workfront應用程式提供額外的安全層。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 依IP位址限制Adobe Workfront的存取權

您可以設定Adobe Workfront IP允許清單，限制對您指定之45個IP位址或IP位址範圍的存取。 這為Workfront應用程式提供額外的安全層。

網路管理員應提供這些IP地址或IP地址範圍。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>企業</p> </td> 
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

## 其他允許清單

如果防火牆或郵件伺服器配置為僅允許訪問某些供應商，則必須將某些IP地址添加到允許清單中。 這會開啟您的環境與Adobe Workfront伺服器之間的通訊。 如需相關資訊，請參閱 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

此外，如果貴組織使用企業計畫，您可以設定Workfront電子郵件允許清單，控制哪些電子郵件網域可以接受來自Workfront的電子郵件，以及哪些電子郵件網域可以位於使用者在其Workfront使用者設定檔中指定的電子郵件地址中。 如需詳細資訊，請參閱 [設定您的電子郵件允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## 將IP位址新增至允許清單

將IP位址新增至Workfront允許清單後，僅可使用這些IP位址來存取Workfront。 嘗試從其他IP位址存取Workfront的使用者會收到錯誤訊息，指出其IP位址已遭封鎖。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **客戶資訊。**

1. 在 **IP允許清單** 部分，選擇 **啟用IP允許清單。**

   預設會停用此選項。

1. 指定您目前用來存取Workfront系統的IP位址。

   或

   指定IP位址範圍，包含您目前用來存取Workfront系統的位址。

   您用來存取Workfront的IP位址必須新增至允許清單，才能啟用允許清單。

1. 按一下 **新增IP範圍、** 然後指定您要能夠存取Workfront的IP位址或IP位址範圍。
1. （可選）重複上一步，新增其他IP位址或IP位址範圍。

   您最多可以新增45個地址或範圍。

1. 按一下 **儲存。**
