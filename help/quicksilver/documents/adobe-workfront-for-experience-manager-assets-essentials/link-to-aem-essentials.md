---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從Experience Manager Assets Essentials連結資產和資料夾
description: You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents. Assets sent from Assets Essentials don't count towards your overall document storage in Workfront. Documents uploaded and sent from Workfront to Assets Essentials do count towards overall storage.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 0b93f6f6-cf4b-4077-a464-be7f19f7cd25
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 4%

---

# 從Experience Manager Assets Essentials連結資產和資料夾

You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents.

To link assets and folders from Experience Manager Assets using Content Advisor, see [Link assets and folders with Content Advisor powered by Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

If you are on enterprise storage, see [Use the Adobe Experience Manager with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 授權</td> 
   <td> 
   <p>投稿人或以上</p> 
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他產品</td> 
   <td>您必須擁有Experience Manager as a Cloud Service或Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager許可權</td> 
    <td>您必須擁有資料夾的寫入許可權。</td> 
   </tr>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視存取許可權或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前：

* 您的Workfront管理員必須設定Experience Manager整合。 For more information, see [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Link an asset from Experience Manager Assets Essentials

1. Go to the **Documents** area in Workfront where you want to add the document.
1. Select **Add New**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >Workfront管理員可以選擇此整合的任何名稱，因此可能不會特別提及Experience Manager Assets Essentials。

1. 選取您想要的資產。

   ![選取資產](assets/select-an-asset.png)

1. 按一下「**選取**」。

## 從Experience Manager Assets Essentials連結新版本

您可以從Experience Manager Assets Essentials提取新資產，並將其作為新版本新增到現有資產。 如果檔案已連結並在Experience Manager Assets Essentials中新增了新版本，新版本會自動出現在Workfront中。

若要連結新版本：

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 選取您要取代為新版本的資產。 您無法在連結的資料夾中建立新版本的資產。
1. 選取「**新增** > **版本**」，然後選取系統管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可以選擇此整合的任何名稱，因此可能沒有特別提及Experience Manager Assets Essentials。

1. 選取您要連結的資產。

1. 按一下「**選取**」。

## 從Experience Manager Assets Essentials連結資料夾

檢視檔案夾內個別資產的許可權取決於Experience Manager Assets Essentials許可權。

1. 移至Workfront中您想要資料夾的&#x200B;**檔案**&#x200B;區域。
1. 選取「**新增**」，然後選取管理員設定的Experience Manager整合。

   >[!NOTE]
   >
   >Workfront管理員可以選擇此整合的任何名稱，因此可能沒有特別提及Experience Manager Assets Essentials。

1. 選取您想要的資料夾。

   ![選取資料夾](assets/select-a-folder.png)

1. 按一下「**選取**」。

## 考量事項

* 內容警告器功能不適用於Assets Essentials。 若要使用「內容警告器」連結資產和資料夾，請參閱[使用Experience Manager Assets支援的「內容警告器」連結資產和資料夾](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md)。

* 從Assets Essentials傳送的Assets不會計入Workfront的整體檔案儲存中。 從Workfront上傳並傳送至Assets Essentials的檔案確實會計入整體儲存空間。

* 從Workfront傳送資產至Experience Manager Assets Essentials時，會先對應中繼資料欄位。 如果您的Workfront管理員已啟用物件中繼資料同步，則欄位在任一應用程式中變更後仍會保持最新狀態。
