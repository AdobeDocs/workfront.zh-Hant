---
title: 停用檔案整合
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 作為 [!DNL anAdobe] [!DNL Workfront]管理員，您可以停用Workfront與任何協力廠商檔案提供者之間的連線。
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 停用檔案整合

作為[!DNL Adobe] [!DNL Workfront]管理員，您可以停用[!DNL Workfront]與任何協力廠商檔案提供者之間的連線。

當您停用[!DNL Workfront]與檔案提供者之間的連線時，檔案的連結會從[!DNL Workfront]中消失。 使用者無法再看到連結的檔案，也無法透過[!DNL Workfront]連結對檔案進行任何變更，也無法向該提供者新增更多檔案。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

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
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。 如需[!DNL Workfront]管理員的相關資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 停用雲端提供者整合

若要停用[!UICONTROL Workfront DAM]、[!DNL Box]、[!DNL Dropbox]、[!DNL Google Drive]、[!DNL Microsoft OneDrive]、[!DNL WebDAM]的檔案整合：

1. 以[!DNL Workfront]管理員身分登入[!DNL Workfront]。
1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 雲端提供者]**。

1. 取消選取您要從[!DNL Workfront]中斷連線的任何雲端提供者。
1. 按一下「**[!UICONTROL 儲存]**」。

   使用者無法連線到您停用的特定雲端提供者，也無法再將來自該雲端提供者的檔案連結到Workfront。

## 停用[!DNL SharePoint]整合

1. 以[!DNL Workfront]管理員身分登入[!DNL Workfront]。
1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 展開&#x200B;**[!UICONTROL 檔案]**，然後按一下&#x200B;**[!UICONTROL [!DNL SharePoint]整合]**。
1. 選取要停用的[!DNL SharePoint]整合。
1. 按一下&#x200B;**[!UICONTROL 停用]**。\
   使用者無法連線到您停用的[!DNL SharePoint]網站，他們無法再從[!DNL SharePoint]連結檔案到[!DNL Workfront]。

## 停用自訂整合

1. 以系統管理員身分登入[!DNL Workfront]。
1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 自訂整合]**。
1. 選取要停用的自訂整合。
1. 按一下&#x200B;**[!UICONTROL 停用]**。

   使用者無法連線到您停用的協力廠商檔案提供者，也無法再從該雲端提供者將檔案連結到[!DNL Workfront]。
