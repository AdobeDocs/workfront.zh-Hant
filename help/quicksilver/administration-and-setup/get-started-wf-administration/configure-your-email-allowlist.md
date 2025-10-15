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
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '399'
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
>&#x200B;>`Joan Harris <notifications@my.workfront.com>`

如需有關設定組織防火牆以開啟環境與Adobe Workfront伺服器之間通訊的資訊，請參閱[設定防火牆允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p> <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是Workfront管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 其他允許清單

如果您的防火牆或郵件伺服器設定為僅允許特定廠商存取，則必須將特定IP位址新增至其允許清單。 這可在您的環境與Adobe Workfront伺服器之間開啟通訊。 如需相關資訊，請參閱[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 設定您的電子郵件允許清單

{{step-1-to-setup}}

1. 按一下&#x200B;**系統** > **客戶資訊**。
1. 在&#x200B;**電子郵件允許清單**&#x200B;區段中，選取&#x200B;**啟用網域允許清單**，然後按一下&#x200B;**新增網域**。
1. 在顯示的方塊中，輸入您要允許的網域，例如`ourcompany.com`，然後按一下&#x200B;**新增網域**。
1. 重複上一步驟，新增您要允許的任何其他網域。
1. 完成時，按一下&#x200B;**儲存**。
