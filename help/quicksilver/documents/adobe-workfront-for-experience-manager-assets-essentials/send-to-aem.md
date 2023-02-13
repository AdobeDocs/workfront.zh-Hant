---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 將檔案傳送至Experience Manager Assets或Assets Essentials
description: 您可以將檔案從Workfront傳送至Experience Manager Assets或Assets Essentials。 從Workfront上傳並傳送至Assets Essentials的檔案，仍會計入您整體的檔案儲存空間。 從Assets Essentials連結的資產不會計入整體儲存。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 6bedca2f3394fadc6d6ffbb34654fd1f0194a5d6
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# 將檔案傳送至Experience Manager Assets或Assets Essentials


您可以將檔案從Workfront傳送至Experience Manager Assets或Assets Essentials。 從Workfront上傳並傳送至Assets Essentials的檔案，仍會計入您整體的檔案儲存空間。 從Assets Essentials連結的資產不會計入整體儲存。

從Workfront將資產傳送至Experience Manager Assets或Assets Essentials時，中繼資料欄位會先對應。 也會傳送任何設定為對應上層物件的中繼資料。 如需設定中繼資料對應的詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**範例** 第一次傳送附加至任務的資產時，任務元資料會對應至Experience Manager Assets或Assets Essentials，以及父對象（如專案、產品組合和方案）的任何對應中繼資料。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權概觀</a>*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您必須有Experience Manageras a Cloud Service或Assets Essentials，且您必須以Admin Console使用者身分新增至產品。
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看文檔上的訪問權限或更高版本</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## 從Workfront傳送檔案

當使用者將檔案從Workfront傳送至Experience Manager Assets或Assets Essentials時，對應的中繼資料會隨檔案傳輸。 傳送檔案後，對Workfront中檔案中繼資料所做的變更不會反映在Assets或Assets Essentials中。 如果變更了Workfront中的對應欄位，您必須將包含更新中繼資料的新檔案版本傳送至Assets或Assets Essentials。 若要設定或編輯中繼資料，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

要發送文檔，請執行以下操作：

1. 前往 **檔案** 區域，然後選取要傳送的檔案。
1. 按一下 **傳送至**，然後選擇管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可以選擇此整合的任何名稱，因此不得特別提及Assets或Assets Essentials。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 選取您要資產前往的位置，然後按一下 **選擇資料夾**.
1. 找到所需目的地後，按一下 **儲存**.

## 傳送新版本

您可以將新版本新增至先前已上傳至Workfront的檔案。 如需詳細資訊，請參閱 [上傳新版本的檔案](../../documents/managing-documents/upload-new-document-version.md). 上傳最新版本後，您就可以將其傳送至Assets Essentials。 如果Workfront中的對應欄位已變更，新版本會在傳送時更新Assets Essentials中的中繼資料。

>[!IMPORTANT]
>
>將新版本上傳至Workfront之前，建議您重新命名檔案。 如果您上傳的新版本檔案名稱與舊版完全相同，則只能從Workfront下載最新版本。 無論檔案名稱為何，所有版本都可從Experience Manager Assets或Assets Essentials下載。

若要傳送最新版本：

1. 前往 **檔案** 區域，並找到檔案。
1. 選擇 **傳送至**，然後選擇管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能不會特別提及Assets或Assets Essentials。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 按一下&#x200B;**儲存**。新版本會儲存在與舊版相同的位置。
