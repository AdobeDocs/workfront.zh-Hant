---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「錯誤：自動布建的使用者無法登入」
description: 如果自動布建的使用者首次嘗試登入，並收到系統未指派存取層級的錯誤，這可能是因為您的系統缺少與請求授權關聯的存取層級。 自動布建使用請求授權型別，因此您可以建立與請求授權關聯的存取層級來修正此問題。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# 錯誤：自動布建的使用者無法登入

當自動布建的使用者嘗試第一次登入時，他們會收到以下錯誤：

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## 問題

系統沒有為新使用者指派存取層級。

依預設，自動布建會使用請求授權型別。 當沒有具有「請求」授權的存取層級存在時，系統無法將存取層級指派給使用者。

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
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>.</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

使用請求授權建立基本存取層級：

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 存取層級]**.

1. 按一下 **[!UICONTROL 新增存取層級]**.
1. 輸入 **[!UICONTROL 名稱]**.
1. 在 **[!UICONTROL 授權型別]** 從下拉式功能表中選取「請求」。
1. 按一下「**[!UICONTROL 儲存變更]**」。

使用「要求」授權建立存取層級後，請讓使用者使用其SSO憑證登入。


