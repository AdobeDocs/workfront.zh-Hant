---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '"錯誤：自動布建的用戶無法登錄」'
description: 如果自動布建的使用者嘗試首次登入，並收到系統未指派存取層級的錯誤訊息，可能是因為您的系統缺少與「請求」授權相關聯的存取層級。 自動布建使用「請求」許可證類型，因此，您可以通過建立與「請求」許可證關聯的訪問級別來解決此問題。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# 錯誤：自動布建的用戶無法登錄

當自動布建的使用者嘗試首次登入時，他們會收到下列錯誤：

## 問題

系統沒有為新用戶分配訪問級別。

依預設，自動布建會使用「請求」授權類型。 當沒有具有請求許可證的訪問級別時，系統無法為用戶分配訪問級別。

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

使用請求授權建立基本存取層級：

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 存取層級]**.

1. 按一下 **[!UICONTROL 新訪問級別]**.
1. 輸入 **[!UICONTROL 名稱]**.
1. 在 **[!UICONTROL 許可證類型]** 下拉式功能表中，選取「請求」。
1. 按一下 **[!UICONTROL 儲存變更]**.

使用請求授權建立存取層級後，請讓使用者以其SSO憑證登入。
