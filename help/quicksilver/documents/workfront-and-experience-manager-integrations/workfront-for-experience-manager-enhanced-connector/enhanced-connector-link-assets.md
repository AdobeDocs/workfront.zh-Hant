---
title: 使用增強型聯結器連結資產和資料夾
description: 您可以從Experience Manager Assets將資產或資料夾連結至支援檔案的任何Workfront物件。
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---


# 使用增強型聯結器連結資產和資料夾

您可以從Experience Manager Assets將資產或資料夾連結至支援檔案的任何Workfront物件。 從Experience Manager Assets傳送的Assets不會計入Workfront的整體檔案儲存中。 從Workfront上傳並傳送至Experience Manager Assets的檔案確實會計入整體儲存空間。


>[!NOTE]
>
>在Workfront中無法預覽透過增強型聯結器連結的Excel檔案。 您必須下載檔案才能存取。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或以上</p>
   <p>要求或更高版本</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他產品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>在檔案上檢視存取許可權或更高的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>


如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須

* 安裝適用於Experience Manager增強型聯結器的Workfront

## 從Experience Manager Assets連結資產

您可以將資產從Experience Manager Assets連結至Workfront。 資產連結後，您可以

* [校訂Experience Manager Assets的連結資產](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [上傳檔案的新版本](../../../documents/managing-documents/upload-new-document-version.md)

若要將資產連結至Experience Manager Assets：

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 按一下&#x200B;**新增**，然後選擇您的管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此可能沒有特別提及Experience Manager Assets。

1. 選取您想要的資產。

   ![選取資產](assets/select-an-asset.png)

1. 按一下&#x200B;**連結**。

## 從Experience Manager Assets連結資料夾

檢視檔案夾內個別資產的許可權取決於Experience Manager Assets許可權。

若要將資料夾連結至Experience Manager Assets：

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 按一下&#x200B;**新增**，然後選擇您的管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此可能沒有特別提及Experience Manager Assets。

1. 選取您想要的資料夾。

   ![選取資料夾](assets/select-a-folder.png)

1. 按一下&#x200B;**連結**。

## 從Experience Manager Assets連結新版本

您可以從Experience Manager Assets提取新資產，並將其新增到Workfront中的現有資產，作為新版本。 如果檔案已連結，並在Experience Manager Assets中新增了新版本，新版本會自動顯示在Workfront中。

>[!TIP]
>
>如果您前往&#x200B;**檔案詳細資料** > **版本**，即可檢視資產的所有版本。

若要從Experience Manager Assets連結新版本：

1. 移至Workfront中要新增檔案的&#x200B;**檔案**&#x200B;區域。
1. 選取您要取代為新版本的資產。 您無法在連結的資料夾中建立新版本的資產。
1. 按一下&#x200B;**新增**，然後選擇您的管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此可能沒有特別提及Experience Manager Assets。

1. 選取您想要的資產。

   ![選取資產](assets/select-an-asset.png)

1. 按一下&#x200B;**連結**。
