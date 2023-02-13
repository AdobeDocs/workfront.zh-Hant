---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '"錯誤消息：無法驗證XML數字簽名」'
description: 您無法建立與ADFS的成功連接。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 錯誤訊息：無法驗證XML數字簽名

## 問題

您無法建立與ADFS的成功連接。

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>如果建立成功的測試連線，但您仍遇到問題，則可能有不正確的屬性對應或同盟ID問題。 如有疑問，請聯絡客戶支援。

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

## 原因1:證書不正確

### 解決方案

從ADFS伺服器手動擷取簽署憑證：

1. 在 [!DNL Windows]，按一下 **[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   將顯示「ADFS 2.0管理」對話框。

1. 選擇 **[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信託]** 在左窗格中。

1. 按一下右鍵 **[!UICONTROL 信賴方信任]**，然後選取 **[!UICONTROL 屬性]**.

1. 按一下 **[!UICONTROL 簽名]** 標籤。
1. 按一下簽署憑證的名稱，然後按一下 **[!UICONTROL 檢視]**.
1. 按一下「複製到」 **[!UICONTROL 檔案]**...，並選取 **[!UICONTROL 下一個]**.

1. 選擇 **[!UICONTROL Base-64編碼x.509(CER)]**，然後按一下 **[!UICONTROL 下一個]**.

1. 指定檔案名，然後按一下 **[!UICONTROL 下一個]**.
1. 按一下 **[!UICONTROL 完成]**.
1. 在 [!DNL Adobe Workfront]，導覽至 **[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 單一登入(SSO)]** 和手動上傳簽署憑證。

## 原因2:當 [!DNL Workfront] 需要RSA簽名

### 解決方案

重新建立憑證，並使用RSA簽章，而非DSA。

## 原因3:XML資料不正確

### 解決方案

從ADFS管理系統重新導出和重新導入XML元資料。

## 原因4:由於SAML端發生錯誤，無法執行要求

### 解決方案

請連絡您的SAML提供者。
