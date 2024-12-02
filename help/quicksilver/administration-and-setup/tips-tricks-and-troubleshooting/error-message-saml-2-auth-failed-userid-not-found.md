---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 錯誤訊息： SAML 2.0驗證失敗：找不到使用者識別碼
description: 使用SAML 2.0時，「找不到SAML 2.0驗證失敗的使用者識別碼」錯誤表示未從ADFS宣告規則傳遞UID或NAME ID。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 錯誤訊息： SAML 2.0驗證失敗：找不到使用者識別碼

## 問題

我在使用SAML 2.0時收到此錯誤：「SAML 2.0驗證失敗：找不到使用者識別碼。」

## 原因

當未從&#x200B;**ADFS宣告規則**&#x200B;傳遞&#x200B;**UID**&#x200B;或&#x200B;**名稱ID**&#x200B;時，就會發生這種情況。

在ADFS中，**信賴方信任**&#x200B;必須有傳遞&#x200B;**UID**&#x200B;或&#x200B;**名稱ID**&#x200B;值的&#x200B;**宣告規則**。 當您執行&#x200B;**[!DNL Workfront]測試連線**&#x200B;時，如果成功，應該會顯示此連線。

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
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解決方案

1. 編輯&#x200B;**[!UICONTROL ADFS資訊]**&#x200B;時，在&#x200B;**[!UICONTROL 信賴方信任]** >選取物件>**[!UICONTROL 編輯宣告規則]**&#x200B;中。

1. **[!UICONTROL LDAP屬性]** （左欄）應該有&#x200B;**[!UICONTROL 電子郵件地址]** （或任何唯一識別碼）。

1. **[!UICONTROL 傳出宣告型別]** （右欄）應為&#x200B;**[!UICONTROL 名稱ID]**。

   >[!NOTE]
   >
   >它不一定要有LDAP屬性電子郵件地址。 可以使用任何可識別使用者的唯一識別碼，但必須將其傳入[!DNL Adobe Workfront]做為&#x200B;**名稱ID**。
