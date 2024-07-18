---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從Experience Manager Assets或Assets Essentials連結資產和資料夾
description: 您可以從Experience Manager Assets或Assets Essentials將資產或資料夾連結至支援檔案的任何Adobe Workfront物件。 從Assets Essentials傳送的Assets不會計入Workfront的整體檔案儲存中。 從Workfront上傳並傳送至Assets Essentials的檔案確實會計入整體儲存空間。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# 從Experience Manager Assets或Assets Essentials連結資產和資料夾

您可以從Experience Manager Assets或Assets Essentials將資產或資料夾連結至支援檔案的任何Adobe Workfront物件。 從Assets Essentials傳送的Assets不會計入Workfront的整體檔案儲存中。 從Workfront上傳並傳送至Assets Essentials的檔案確實會計入整體儲存空間。

從Workfront傳送資產至Experience Manager Assets或Assets Essentials時，會先對應中繼資料欄位。 如果您的Workfront管理員已啟用物件中繼資料同步，則欄位在任一應用程式中變更後仍會保持最新狀態。

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
   <td>您必須擁有Experience Manageras a Cloud Service或Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager許可權</td> 
    <td>您必須擁有資料夾的寫入許可權。</td> 
   </tr>
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視存取許可權或更高</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

開始之前，

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱[設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

## 從Experience Manager Assets或Assets Essentials連結資產

您可以將資產從Experience Manager Assets或Assets Essentials連結至Workfront。 資產連結後，您可以

* [校訂Experience Manager Assets或Assets Essentials的連結資產](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [上傳檔案的新版本](../../documents/managing-documents/upload-new-document-version.md)

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 選取「**新增**」，然後選取系統管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能不會特別提及Assets或Assets Essentials。

1. 選取您想要的資產。

   ![](assets/select-an-asset.png)

1. 按一下&#x200B;**選取**。

## 從Experience Manager Assets或Assets Essentials連結資料夾

檢視檔案夾內個別資產的許可權取決於Experience Manager Assets或Assets Essentials許可權。

1. 移至Workfront中您想要資料夾的&#x200B;**檔案**&#x200B;區域。
1. 選取「**新增**」，然後選取系統管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能沒有特別提及Assets或Assets Essentials。

1. 選取您想要的資料夾。

   ![](assets/select-a-folder.png)

1. 按一下&#x200B;**選取**。

## 從Experience Manager Assets或Assets Essentials連結新版本

您可以從Assets Essentials提取新資產，並將其作為新版本新增到現有資產。 如果檔案已連結，且Assets Essentials中已新增新版本，則新版本會自動顯示在Workfront中。

若要從Assets Essentials連結新版本：

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 選取您要取代為新版本的資產。 您無法在連結的資料夾中建立新版本的資產。
1. 選取「**新增** > **版本**」，然後選取系統管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能沒有特別提及Assets或Assets Essentials。

1. 選取您想要的資產。

   ![](assets/select-an-asset.png)

1. 按一下&#x200B;**選取**。

>[!TIP]
>
>如果您前往&#x200B;**檔案詳細資料** > **版本**，即可檢視資產的所有版本。
