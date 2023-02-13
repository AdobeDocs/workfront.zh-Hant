---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從Experience Manager Assets或Assets Essentials連結資產和資料夾
description: 您可以將資產或資料夾從Experience Manager Assets或Assets Essentials連結至支援檔案的任何Adobe Workfront物件。 從Assets Essentials傳送的資產不會計入Workfront中的整體檔案儲存。 從Workfront上傳並傳送至Assets Essentials的檔案確實會計入整體儲存空間。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# 從Experience Manager Assets或Assets Essentials連結資產和資料夾

您可以將資產或資料夾從Experience Manager Assets或Assets Essentials連結至支援檔案的任何Adobe Workfront物件。 從Assets Essentials傳送的資產不會計入Workfront中的整體檔案儲存。 從Workfront上傳並傳送至Assets Essentials的檔案確實會計入整體儲存空間。

從Workfront將資產傳送至Experience Manager Assets或Assets Essentials時，中繼資料欄位會先對應。 如果您的Workfront管理員已啟用物件中繼資料同步，如果欄位在任一應用程式中變更，則欄位會保持最新。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您必須有Experience Manageras a Cloud Service或Assets Essentials，且您必須以Admin Console使用者身分新增至產品。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager權限</td> 
    <td>您必須具有資料夾的寫入權限。</td> 
   </tr>
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看訪問權限或更高版本</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 從Experience Manager Assets或Assets Essentials連結資產

您可以將資產從Experience Manager Assets或Assets Essentials連結至Workfront。 連結資產後，您就可以

* [校樣Experience Manager Assets或Assets Essentials的連結資產](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [上傳新版本的檔案](../../documents/managing-documents/upload-new-document-version.md)

1. 前往 **檔案** 在Workfront中要添加文檔的區域。
1. 選擇 **新增**，然後選取管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可以選擇此整合的任何名稱，因此不得特別提及Assets或Assets Essentials。

1. 選取您想要的資產。

   ![](assets/select-an-asset.png)

1. 按一下 **選擇**.

## 從Experience Manager Assets或Assets Essentials連結資料夾

檢視資料夾內個別資產的權限取決於Experience Manager Assets或Assets Essentials權限。

1. 前往 **檔案** 區域(在Workfront中您要資料夾的位置)。
1. 選擇 **新增**，然後選取管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能不會特別提及Assets或Assets Essentials。

1. 選取您要的資料夾。

   ![](assets/select-a-folder.png)

1. 按一下 **選擇**.

## 從Experience Manager Assets或Assets Essentials連結新版本

您可以從Assets Essentials提取新資產，並將其新增至現有資產，做為新版本。 如果檔案已連結，且Assets Essentials中已新增新版本，則新版本會自動顯示在Workfront中。

若要從Assets Essentials連結新版本：

1. 前往 **檔案** 在Workfront中要添加文檔的區域。
1. 選取要以新版本取代的資產。 您無法在連結的資料夾中建立新版本的資產。
1. 選擇 **新增** > **版本**，然後選取管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能不會特別提及Assets或Assets Essentials。

1. 選取您要的資產。

   ![](assets/select-an-asset.png)

1. 按一下 **選擇**.

>[!TIP]
>
>如果您前往 **文檔詳細資訊** > **版本**.
