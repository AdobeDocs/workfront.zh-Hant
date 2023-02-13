---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '錯誤訊息：SAML 2.0驗證失敗：找不到用戶標識符'
description: 當您使用SAML 2.0時，「SAML 2.0 Authentication Failed-User Identifier Not Found」錯誤表示不會從ADFS聲明規則傳遞UID或NAME ID。 在ADFS中，信賴方信任需要具有傳遞UID或NAME ID值的聲明規則。 當您執行 [!DNL Workfront] 測試連線，如果成功，應會顯示此訊息。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---

# 錯誤訊息：SAML 2.0驗證失敗：未找到用戶標識符

## 問題

使用SAML 2.0時，我會收到此錯誤：&quot;SAML 2.0驗證失敗：未找到用戶標識符。」

## 原因

當 **UID** 或 **名稱ID** 不會從 **ADFS索賠規則**.

在ADFS中， **信賴方信任** 需要 **索賠規則** 會傳遞a **UID** 或 **名稱ID** 值。 當您執行 **[!DNL Workfront]測試連線**，如果成功，應會顯示此訊息。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

1. 編輯 **[!UICONTROL ADFS資訊]**，在 **[!UICONTROL 信賴方信託]** >選擇對象>**[!UICONTROL 編輯聲明規則]**.

1. 此 **[!UICONTROL LDAP屬性]** （左欄）應具有 **[!UICONTROL 電子郵件地址]** （或任何唯一識別碼）。

1. 此 **[!UICONTROL 傳出聲明類型]** （右欄）應為 **[!UICONTROL 名稱ID]**.

   >[!NOTE]
   >
   >它不必具有LDAP屬性電子郵件地址。 可使用任何可識別使用者的唯一識別碼，但必須將其傳入 [!DNL Adobe Workfront] 作為 **名稱ID**.
