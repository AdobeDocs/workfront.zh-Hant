---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 設定您的電子郵件允許清單
description: 如果您的組織使用WorkfrontEnterprise計畫，您可以建立Workfront電子郵件允許清單，以控制允許哪些電子郵件網域接受來自Workfront的電子郵件，以及哪些電子郵件網域可位於使用者在其使用者設定檔中指定的電子郵件地址中。 如果您的組織安全原則限制使用者將Workfront中儲存的資料傳送至外部電子郵件地址，這很有用 — 您可以在允許清單中僅包含內部公司網域，以確保遵循此原則。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 設定您的電子郵件允許清單

如果您的組織使用Workfront企業計畫，您可以建立Workfront電子郵件允許清單來控制：

* 允許哪些電子郵件網域接受來自Workfront的電子郵件。
* 使用者可在使用者設定檔中指定的電子郵件地址中包含哪些電子郵件網域。

如果您的組織安全原則限制使用者將Workfront中儲存的資料傳送至外部電子郵件地址，這很有用 — 您可以在允許清單中僅包含內部公司網域，以確保遵循此原則。

>[!IMPORTANT]
>
>您的IT團隊應確保來自`notifications@my.workfront.com`的傳入電子郵件不會在您的組織系統中遭到封鎖。
>
>所有來自Workfront的電子郵件都會從該地址傳送，以增加成功的電子郵件傳遞，並消除偽造電子郵件的行為。 這包括自動警報和使用者之間的通訊。
>
>例如，您從名為Joan Harris的使用者收到的Workfront電子郵件中的「寄件者」行如下所示：
>`Joan Harris <notifications@my.workfront.com>`

如需有關設定組織防火牆以開啟環境與Adobe Workfront伺服器之間通訊的資訊，請參閱[設定防火牆允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 其他允許清單

如果貴組織擁有企業計畫，您可以設定Adobe Workfront IP允許清單，將對Workfront的存取限製為您指定的45個IP位址或IP位址範圍。 這為Workfront應用程式提供額外的安全層。 如需詳細資訊，請參閱[依IP位址限制存取Adobe Workfront](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md)。

此外，如果您的防火牆或郵件伺服器設定為僅允許存取特定廠商，則必須將特定IP位址新增至其允許清單。 這可在您的環境與Adobe Workfront伺服器之間開啟通訊。 如需相關資訊，請參閱[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 設定您的電子郵件允許清單

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **客戶資訊**。
1. 在&#x200B;**電子郵件允許清單**&#x200B;區段中，選取&#x200B;**啟用網域允許清單**，然後按一下&#x200B;**新增網域**。
1. 在顯示的方塊中，輸入您要允許的網域，例如`ourcompany.com`，然後按一下&#x200B;**新增網域**。
1. 重複上一步驟，新增您要允許的任何其他網域。
1. 完成時，按一下&#x200B;**儲存**。
