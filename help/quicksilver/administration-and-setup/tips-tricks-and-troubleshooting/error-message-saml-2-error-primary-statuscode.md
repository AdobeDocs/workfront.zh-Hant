---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 錯誤訊息： SAML 2.0錯誤：主要狀態碼
description: 您無法成功建立與ADFS的連線。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

# 錯誤訊息： SAML 2.0錯誤：主要狀態碼

## 問題

您無法成功建立與ADFS的連線。

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>如果您建立了成功的測試連線，但仍遇到問題，則屬性對應可能不正確，或是同盟ID有問題。 如有疑問，請聯絡客戶支援。

## 存取需求

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

## 原因1：安全雜湊演演算法設為SHA-256

### 解決方案

1. 在Windows中，按一下&#x200B;**[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**。\
   隨即顯示「ADFS 2.0管理」對話方塊。

1. 在左窗格中選取&#x200B;**[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信任]**。

1. 以滑鼠右鍵按一下與[!DNL Adobe Workfront]相關的信賴方信任，然後選取&#x200B;**[!UICONTROL 內容]**。
1. 按一下&#x200B;**[!UICONTROL 進階]**&#x200B;標籤，然後從&#x200B;**[!UICONTROL 安全雜湊演演算法]**&#x200B;下拉式功能表中選取&#x200B;**[!UICONTROL SHA-1]**。\
   ![](assets/1-350x287.png)

## 原因2： ADFS簽署憑證即將到期，並已由日期重疊的新憑證取代

### 解決方案

[!DNL Workfront] SSO設定頁面列出憑證到期日。 如果憑證即將到期，您必須手動從ADFS伺服器提取新簽署憑證：

1. 在Windows中，按一下&#x200B;**[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**。\
   隨即顯示「ADFS 2.0管理」對話方塊。

1. 在左窗格中選取&#x200B;**[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信任]**。

1. 以滑鼠右鍵按一下與[!DNL Workfront]相關的信賴方信任，然後選取&#x200B;**[!UICONTROL 內容]**。
1. 按一下&#x200B;**[!UICONTROL 簽章]**&#x200B;標籤。
1. 按一下簽署憑證的名稱，然後按一下[檢視]。****
1. 按一下[複製到&#x200B;**[!UICONTROL 檔案]**...]，然後選取&#x200B;**[!UICONTROL 下一步]**。

1. 選取&#x200B;**[!UICONTROL Base-64編碼的x.509 (CER)]**，然後按一下&#x200B;**[!UICONTROL 下一步]**。

1. 指定檔案名稱，然後按一下&#x200B;**[!UICONTROL 下一步]**。
1. 按一下「**[!UICONTROL 完成]**」。
1. 在[!DNL Workfront]中，瀏覽至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 系統]** > **[!UICONTROL 單一登入(SSO)]**，並手動上傳簽署憑證。

## 原因3：憑證撤銷檢查失敗

此問題的解決方案取決於您所使用的[!DNL Microsoft] ADFS版本。 請參閱[!DNL Microsoft]的檔案以取得您版本的適當命令。
