---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 啟用Outlook以與Workfront和SAML 2.0搭配使用
description: 如果您啟用SAML 2.0驗證，並且希望您的使用者能夠使用其SAML 2.0憑證，從Microsoft Outlook登入Workfront，則必須啟用SAML 2.0，才能在Office增益集中進行驗證。
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# 啟用Outlook以與Workfront和SAML 2.0搭配使用

如果您啟用SAML 2.0驗證，並且希望您的使用者能夠使用其SAML 2.0憑證，從Microsoft Outlook登入Workfront，則必須啟用SAML 2.0，才能在Office增益集中進行驗證。

>[!NOTE]
>
>如果貴組織的Workfront執行個體使用自訂SSO入口網站，則無法使用此功能。>
><!--
>or is enabled with Adobe IMS>
>-->
>如需詳細資訊，請洽詢您的網路或IT管理員。

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

## 啟用Outlook以與Workfront和SAML 2.0搭配使用

1. 按一下 **設定** 在全域導覽列上Adobe Workfront的右上角附近。
1. 按一下 **系統** > **偏好設定**.

1. 在 **安全性** 區段，請確定 **在Office 365增益集中允許SAML 2.0驗證**&#x200B;啟用。

   此選項僅針對Office 365增益集，啟用將Workfront嵌入Iframe。 這不會開啟點擊頂升違規，因為不涉及可點按的內容。

   預設會啟用此選項。

   >[!NOTE]
   >
   >如果您啟用選項 **允許在iframe中內嵌Workfront**，選項 **在Office 365增益集中允許SAML 2.0驗證** 為灰色且啟用。
   >
   >![](assets/if-you-enable.png)

1. 按一下&#x200B;**儲存**。

   您在此儲存的變更會影響Workfront中所有使用者的體驗。
