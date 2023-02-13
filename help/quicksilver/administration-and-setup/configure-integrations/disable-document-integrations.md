---
title: 停用檔案整合
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: As [!DNL anAdobe] [!DNL Workfront] 管理員，您可以停用Workfront與任何協力廠商檔案提供者之間的連線。
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---

# 停用檔案整合

作為 [!DNL Adobe] [!DNL Workfront] 管理員，您可以停用 [!DNL Workfront] 和第三方檔案提供商。

當您停用 [!DNL Workfront] 和檔案提供者，檔案的連結會從 [!DNL Workfront]. 使用者無法再看見連結的檔案，無法透過 [!DNL Workfront] 連結，且無法將更多檔案新增至該提供者。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 停用雲端提供者整合

若要停用的檔案整合 [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. 登入 [!DNL Workfront] as a [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 雲端提供者]**.

1. 取消選擇您要斷開與 [!DNL Workfront].
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   使用者無法連線至您停用的特定雲端提供者，且無法再將該雲端提供者的檔案連結至Workfront。

## 停用 [!DNL SharePoint] 整合

1. 登入 [!DNL Workfront] as a [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 展開 **[!UICONTROL 檔案]**，然後按一下 **[!UICONTROL [!DNL SharePoint]整合]**.
1. 選取 [!DNL SharePoint] 您要停用的整合。
1. 按一下 **[!UICONTROL 停用]**.\
   使用者無法連線至 [!DNL SharePoint] 網站，而且他們無法再連結 [!DNL SharePoint] to [!DNL Workfront].

## 停用自訂整合

1. 登入 [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 自訂整合]**.
1. 選取您要停用的自訂整合。
1. 按一下 **[!UICONTROL 停用]**.

   用戶無法連接到您禁用的第三方文檔提供程式，並且他們無法再將文檔從雲提供程式連結到 [!DNL Workfront].
