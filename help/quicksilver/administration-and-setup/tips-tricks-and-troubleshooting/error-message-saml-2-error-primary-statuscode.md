---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''錯誤訊息：SAML 2.0錯誤：主要狀態代碼'
description: 您無法建立與ADFS的成功連接。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 錯誤訊息：SAML 2.0錯誤：主要狀態代碼

## 問題

您無法建立與ADFS的成功連接。

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

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

## 原因1:安全雜湊演算法設為SHA-256

### 解決方案

1. 在Windows中，按一下 **[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   將顯示「ADFS 2.0管理」對話框。

1. 選擇 **[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信託]** 在左窗格中。

1. 按一下右鍵與 [!DNL Adobe Workfront]，然後選取 **[!UICONTROL 屬性]**.
1. 按一下 **[!UICONTROL 進階]** ，然後選取 **[!UICONTROL SHA-1]** 從 **[!UICONTROL 安全哈希算法]** 下拉式功能表。\
   ![](assets/1-350x287.png)

## 原因2:ADFS簽署憑證即將過期，且已由日期重疊的新憑證取代

### 解決方案

此 [!DNL Workfront] SSO設定頁面會列出憑證的到期日。 如果證書即將過期，您需要從ADFS伺服器手動提取新簽名證書：

1. 在Windows中，按一下 **[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   將顯示「ADFS 2.0管理」對話框。

1. 選擇 **[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信託]** 在左窗格中。

1. 按一下右鍵與 [!DNL Workfront]，然後選取 **[!UICONTROL 屬性]**.
1. 按一下 **[!UICONTROL 簽名]** 標籤。
1. 按一下簽署憑證的名稱，然後按一下 **[!UICONTROL 檢視]**.
1. 按一下「複製到」 **[!UICONTROL 檔案]**...，並選取 **[!UICONTROL 下一個]**.

1. 選擇 **[!UICONTROL Base-64編碼x.509(CER)]**，然後按一下 **[!UICONTROL 下一個]**.

1. 指定檔案名，然後按一下 **[!UICONTROL 下一個]**.
1. 按一下 **[!UICONTROL 完成]**.
1. 在 [!DNL Workfront]，導覽至 **[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 單一登入(SSO)]** 和手動上傳簽署憑證。

## 原因3:證書吊銷檢查失敗

解決方案取決於 [!DNL Microsoft] 您使用的ADFS。 諮詢 [!DNL Microsoft]的檔案，以取得適合您版本的指令。
