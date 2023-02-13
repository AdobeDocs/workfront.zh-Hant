---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 設定您的電子郵件允許清單
description: 如果您的組織使用WorkfrontEnterprise計畫，您可以建立Workfront電子郵件允許清單，控制哪些電子郵件網域可以接受來自Workfront的電子郵件，以及哪些電子郵件網域可以位於使用者在其使用者設定檔中指定的電子郵件地址中。 如果貴組織的安全性原則限制使用者將儲存在Workfront中的資料傳送至外部電子郵件地址，這個功能就會很實用，因為您只能在允許清單中納入內部公司網域，以確保遵循此原則。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 設定您的電子郵件允許清單

如果貴組織使用WorkfrontEnterprise計畫，您可以建立Workfront電子郵件允許清單以控制：

* 哪些電子郵件網域可接受來自Workfront的電子郵件。
* 使用者在其使用者設定檔中指定的電子郵件地址中可以包含哪些電子郵件網域。

如果貴組織的安全性原則限制使用者將儲存在Workfront中的資料傳送至外部電子郵件地址，這個功能就會很實用，因為您只能在允許清單中納入內部公司網域，以確保遵循此原則。

>[!IMPORTANT]
>
>您的IT團隊應確保來自 `notifications@my.workfront.com` 未在貴組織的系統中遭到封鎖。
>
>來自Workfront的所有電子郵件都會從該位址傳送，以增加成功的電子郵件傳送，並消除電子郵件欺騙。 這包括自動警報和使用者對使用者通訊。
>
>例如，您從名為Joan Harris的使用者收到的Workfront電子郵件中的「寄件者」行看起來會像這樣：
>
```
>Joan Harris <notifications@my.workfront.com>
>```

如需將組織的防火牆設定為開啟環境與Adobe Workfront伺服器之間通訊的相關資訊，請參閱 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 其他允許清單

如果貴組織有企業計畫，您可以設定Adobe Workfront IP允許清單，限制您對Workfront的45個IP位址或您指定的IP位址範圍存取。 這為Workfront應用程式提供額外的安全層。 如需詳細資訊，請參閱 [依IP位址限制Adobe Workfront的存取權](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

此外，如果防火牆或郵件伺服器配置為僅允許訪問某些供應商，則必須將某些IP地址添加到允許清單中。 這會開啟您的環境與Adobe Workfront伺服器之間的通訊。 如需相關資訊，請參閱 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 設定您的電子郵件允許清單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **客戶資訊**.

1. 在 **電子郵件允許清單** 部分，選擇 **啟用域允許清單**，然後按一下 **添加域**.
1. 在顯示的方塊中，輸入您要允許的網域，例如 `ourcompany.com`，然後按一下 **添加域**.

1. 重複上一步以新增您要允許的任何其他網域。
1. 完成後，按一下 **儲存**.
