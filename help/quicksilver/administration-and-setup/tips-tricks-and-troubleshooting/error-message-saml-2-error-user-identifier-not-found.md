---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「錯誤訊息： SAML 2.0錯誤：找不到使用者識別碼」
description: 您無法成功建立與ADFS的連線。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '215'
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

ADFS伺服器上的宣告不正確。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

+++ 展開以檢視本文中功能的存取需求。

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
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是[!DNL Workfront]管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解決方案

在ADFS伺服器上，確定有名稱ID的宣告：

1. 在Windows中，按一下&#x200B;**[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**。\
   隨即顯示「ADFS 2.0管理」對話方塊。

1. 在左窗格中選取&#x200B;**[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信任]**。

1. 以滑鼠右鍵按一下與Adobe Workfront相關的信賴方信任，然後選取&#x200B;**[!UICONTROL 編輯宣告規則]**。
1. 確認宣告有&#x200B;**[!UICONTROL 名稱ID]**&#x200B;的&#x200B;**[!UICONTROL 傳出宣告型別]**。

![1.png](assets/1-350x287.png)
