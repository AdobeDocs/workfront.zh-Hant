---
title: 停用檔案整合
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 作為 [!DNL anAdobe] [!DNL Workfront]管理員，您可以停用Workfront與任何協力廠商檔案提供者之間的連線。
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 2%

---

# 停用檔案整合

作為[!DNL Adobe] [!DNL Workfront]管理員，您可以停用[!DNL Workfront]與任何協力廠商檔案提供者之間的連線。

當您停用[!DNL Workfront]與檔案提供者之間的連線時，檔案的連結會從[!DNL Workfront]中消失。 使用者無法再看到連結的檔案，也無法透過[!DNL Workfront]連結對檔案進行任何變更，也無法向該提供者新增更多檔案。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table>
  <tr>
   <td>Adobe Workfront套件
   </td>
   <td> <p>Prime或Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront授權
   </td>
   <td><p>標準</p>
   <p>規劃</p>
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 停用雲端提供者整合

若要停用[!UICONTROL Workfront DAM]、[!DNL Box]、[!DNL Dropbox]、[!DNL Google Drive]、[!DNL Microsoft OneDrive]、[!DNL WebDAM]的檔案整合：

1. 以[!DNL Workfront]管理員身分登入[!DNL Workfront]。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 雲端提供者]**。

1. 取消選取您要從[!DNL Workfront]中斷連線的任何雲端提供者。
1. 按一下「**[!UICONTROL 儲存]**」。

   使用者無法連線到您停用的特定雲端提供者，也無法再將來自該雲端提供者的檔案連結到Workfront。

## 停用[!DNL SharePoint]整合

1. 以[!DNL Workfront]管理員身分登入[!DNL Workfront]。

{{step-1-to-setup}}

1. 展開&#x200B;**[!UICONTROL 檔案]**，然後按一下&#x200B;**[!UICONTROL [!DNL SharePoint]整合]**。
1. 選取要停用的[!DNL SharePoint]整合。
1. 按一下&#x200B;**[!UICONTROL 停用]**。\
   使用者無法連線到您停用的[!DNL SharePoint]網站，他們無法再從[!DNL SharePoint]連結檔案到[!DNL Workfront]。

## 停用自訂整合

1. 以系統管理員身分登入[!DNL Workfront]。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 自訂整合]**。
1. 選取要停用的自訂整合。
1. 按一下&#x200B;**[!UICONTROL 停用]**。

   使用者無法連線到您停用的協力廠商檔案提供者，也無法再從該雲端提供者將檔案連結到[!DNL Workfront]。
