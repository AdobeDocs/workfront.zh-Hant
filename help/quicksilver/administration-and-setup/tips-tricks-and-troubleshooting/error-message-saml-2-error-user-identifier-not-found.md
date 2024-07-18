---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「錯誤訊息： SAML 2.0錯誤：找不到使用者識別碼」
description: 您無法成功建立與ADFS的連線。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# 錯誤訊息： SAML 2.0錯誤：找不到使用者識別碼

## 問題

您無法成功建立與ADFS的連線。

![識別碼_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>如果您建立了成功的測試連線，但仍遇到問題，則屬性對應可能不正確，或是同盟ID有問題。 如有疑問，請聯絡客戶支援。

## 原因：

ADFS伺服器上的宣告不正確

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。 如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> <p><b>注意</b>：如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

在ADFS伺服器上，確定有名稱ID的宣告：

1. 在Windows中，按一下&#x200B;**[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**。\
   隨即顯示「ADFS 2.0管理」對話方塊。

1. 在左窗格中選取&#x200B;**[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信任]**。

1. 以滑鼠右鍵按一下與Adobe Workfront相關的信賴方信任，然後選取&#x200B;**[!UICONTROL 編輯宣告規則]**。
1. 確認宣告有&#x200B;**[!UICONTROL 名稱ID]**&#x200B;的&#x200B;**[!UICONTROL 傳出宣告型別]**。

![1.png](assets/1-350x287.png)
