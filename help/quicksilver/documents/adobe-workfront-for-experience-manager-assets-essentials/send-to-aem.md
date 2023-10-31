---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 傳送檔案至Experience Manager Assets或Assets Essentials
description: 您可以從Workfront傳送檔案至Experience Manager Assets或Assets Essentials。 從Workfront上傳並傳送至Assets Essentials的檔案仍會計入您的整體檔案儲存。 從Assets Essentials連結的資產不會計入整體儲存空間。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 24ffde1850a005428a3f619fc00842a8779bbc6d
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# 傳送檔案至Experience Manager Assets或Assets Essentials

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽Sandbox環境中可用。</span>

您可以從Workfront傳送檔案至Experience Manager Assets或Assets Essentials。 從Workfront上傳並傳送至Assets Essentials的檔案仍會計入您的整體檔案儲存。 從Assets Essentials連結的資產不會計入整體儲存空間。

從Workfront傳送資產至Experience Manager Assets或Assets Essentials時，會先對應中繼資料欄位。 設定為對應父物件的任何中繼資料也會一併傳送。 如需設定中繼資料對應的詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**範例** 第一次傳送附加到任務的資產時，任務中繼資料會對應至Experience Manager Assets或Assets Essentials，以及父物件（例如專案、專案組合和方案）的任何對應中繼資料。

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
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">舊版授權概觀</a>*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您必須擁有Experience Manageras a Cloud Service或Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視檔案的存取許可權或以上許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## 從Workfront傳送檔案

當使用者將檔案從Workfront傳送到Experience Manager Assets或Assets Essentials時，對應的中繼資料會沿著檔案傳輸。 傳送檔案後，在Workfront中對檔案中繼資料所做的變更不會反映在資產或Assets Essentials中。 如果Workfront中的對應欄位已變更，您必須將包含更新後中繼資料的新版檔案傳送至「資產」或「Assets Essentials」。 若要設定或編輯中繼資料，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

若要傳送檔案：

1. 前往 **檔案** Workfront區域，並選取您要傳送的檔案。
1. 按一下 **傳送至**，然後選擇您的管理員所設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能不會特別提及資產或Assets Essentials。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 選擇要將資產移至何處，然後按一下 **選取資料夾**.
1. 當您找到想要的目的地，請按一下 **儲存**.

## 傳送新版本

您可以將新版本新增至先前已上傳至Workfront的檔案。 如需詳細資訊，請參閱 [上傳檔案的新版本](../../documents/managing-documents/upload-new-document-version.md). 上傳最新版本後，即可傳送給Assets Essentials。 如果Workfront中的對應欄位已變更，新版本會在傳送時更新Assets Essentials中的中繼資料。

>[!IMPORTANT]
>
>上傳新版本至Workfront之前，建議您重新命名檔案。 如果您上傳的檔案名稱與舊版完全相同的新版本，則只能從Workfront下載最新版本。 所有版本均可從Experience Manager Assets或Assets Essentials下載，無論檔案名稱為何。

若要傳送最新版本：

1. 前往 **檔案** Workfront區域，然後找到檔案。
1. 選取 **傳送至**，然後選擇您的管理員所設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可為這項整合選擇任何名稱，因此可能沒有特別提及資產或Assets Essentials。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 按一下&#x200B;**儲存**。新版本會儲存在與舊版本相同的位置。

## 在Experience Manager Assets中將檔案移至連結的資料夾

>[!NOTE]
>
>此功能僅適用於Experience Manager Assetsas a Cloud Service。 它不適用於Experience Manager Assets Essentials。

如果檔案和連結資料夾都在相同的檔案清單中（例如專案的檔案區域），您可以將檔案移動到Experience Manager Assets中的連結資料夾。

1. 找到您要移動的檔案。
1. 將檔案拖放至您要移動它的連結Experience Manager Assets資料夾。

<div class="preview">檔案正在移動時，檔案選項不可用。 檔案移至Experience Manager Assets後，Workfront的檔案清單中將不再顯示。

>[!NOTE]
>
> 您在檔案移動時對它所做的任何動作或編輯都不會顯示在Experience Manager Assets的檔案中，因此將會遺失。
</div>
