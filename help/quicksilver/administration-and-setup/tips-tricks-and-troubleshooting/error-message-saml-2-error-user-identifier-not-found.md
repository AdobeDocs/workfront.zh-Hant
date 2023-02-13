---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '錯誤訊息：SAML 2.0錯誤：找不到用戶標識符'
description: 您無法建立與ADFS的成功連接。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 1%

---

# 錯誤訊息：SAML 2.0錯誤：未找到用戶標識符

## 問題

您無法建立與ADFS的成功連接。

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>如果建立成功的測試連線，但您仍遇到問題，則可能有不正確的屬性對應或同盟ID問題。 如有疑問，請聯絡客戶支援。

## 原因：

ADFS伺服器上的聲明不正確

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

在ADFS伺服器上，請確定有名稱ID的聲明：

1. 在Windows中，按一下 **[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   將顯示「ADFS 2.0管理」對話框。

1. 選擇 **[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信託]** 在左窗格中。

1. 以滑鼠右鍵按一下與Adobe Workfront相關的信賴方信任，然後選取 **[!UICONTROL 編輯聲明規則]**.
1. 驗證聲明是否具有 **[!UICONTROL 傳出聲明類型]** of **[!UICONTROL 名稱ID]**.

![1.png](assets/1-350x287.png)
