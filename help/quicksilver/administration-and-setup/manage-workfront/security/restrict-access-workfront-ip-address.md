---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: 依IP位址限制對Adobe Workfront的存取
description: 您可以設定Adobe Workfront IP允許清單，將對Workfront的存取限製為您指定的45個IP位址或IP位址範圍。 這為Workfront應用程式提供額外的安全層。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---

# 依IP位址限制對Adobe Workfront的存取

您可以設定Adobe Workfront IP允許清單，將對Workfront的存取限製為您指定的45個IP位址或IP位址範圍。 這為Workfront應用程式提供額外的安全層。

這些IP位址或IP位址範圍應由您的網路管理員提供。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 其他允許清單

如果您的防火牆或郵件伺服器設定為僅允許特定廠商存取，則必須將特定IP位址新增至其允許清單。 這可在您的環境與Adobe Workfront伺服器之間開啟通訊。 如需相關資訊，請參閱[設定防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

此外，如果您的組織使用企業計畫，您可以設定Workfront電子郵件允許清單，以控制允許哪些電子郵件網域接受來自Workfront的電子郵件，以及哪些電子郵件網域可以在使用者在其Workfront使用者設定檔中指定的電子郵件地址中。 如需詳細資訊，請參閱[設定您的電子郵件允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)。

## 將IP位址新增至允許清單

將IP位址新增至Workfront允許清單後，只能使用這些IP位址來存取Workfront。 嘗試從其他IP位址存取Workfront的使用者會收到錯誤訊息，指出其IP位址遭到封鎖。

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **客戶資訊。**

1. 在&#x200B;**IP允許清單**&#x200B;區段中，選取&#x200B;**啟用IP允許清單。**

   此選項預設為停用。

1. 指定您目前用來存取Workfront系統的IP位址。

   或

   指定IP位址範圍，包括您目前用來存取Workfront系統的IP位址。

   您用來存取Workfront的IP位址必須先新增至允許清單，才能啟用允許清單。

1. 按一下&#x200B;**新增IP範圍**，然後指定您要存取Workfront的IP位址或IP位址範圍。
1. （選用）重複先前的步驟，新增其他IP位址或IP位址範圍。

   您最多可以新增45個地址或範圍。

1. 按一下&#x200B;**儲存。**
