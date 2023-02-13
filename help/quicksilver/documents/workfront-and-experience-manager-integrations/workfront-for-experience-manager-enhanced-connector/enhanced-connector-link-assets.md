---
title: 使用增強的連接器連結資產和資料夾
description: 您可以將資產或資料夾從Experience Manager Assets連結至支援檔案的任何Workfront物件。
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 使用增強的連接器連結資產和資料夾

您可以將資產或資料夾從Experience Manager Assets連結至支援檔案的任何Workfront物件。 從Experience Manager Assets傳送的資產不會計入Workfront中的整體檔案儲存。 從Workfront上傳並傳送至Experience Manager Assets的檔案確實會計入整體儲存空間。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看文檔上的訪問權限或更高版本</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須

* 安裝Workfront for Experience Manager增強連接器

## 從Experience Manager Assets連結資產

您可以將資產從Experience Manager Assets連結至Workfront。 連結資產後，您就可以

* [校樣連結的Experience Manager Assets資產](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [上傳新版本的檔案](../../../documents/managing-documents/upload-new-document-version.md)

若要將資產連結至Experience Manager Assets:

1. 前往 **檔案** 在Workfront中要添加文檔的區域。
1. 按一下 **新增**，然後選擇管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此不得具體提及Experience Manager Assets。

1. 選取您想要的資產。

   ![](assets/select-an-asset.png)

1. 按一下 **連結**.

## 從Experience Manager Assets連結資料夾

檢視資料夾內個別資產的權限取決於Experience Manager Assets權限。

若要將資料夾連結至Experience Manager Assets:

1. 前往 **檔案** 在Workfront中要添加文檔的區域。
1. 按一下 **新增**，然後選擇管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此不得具體提及Experience Manager Assets。

1. 選取您要的資料夾。

   ![](assets/select-a-folder.png)

1. 按一下 **連結**.

## 從Experience Manager Assets連結新版本

您可以從Experience Manager Assets提取新資產，並將其新增至現有資產，做為Workfront的新版本。 如果檔案已連結，且Experience Manager Assets中已新增新版本，則新版本會自動顯示在Workfront中。

>[!TIP]
>
>如果您前往 **文檔詳細資訊** > **版本**.

若要從Experience Manager Assets連結新版本：

1. 前往 **檔案** 在Workfront中要添加文檔的區域。
1. 選取要以新版本取代的資產。 您無法在連結的資料夾中建立新版本的資產。
1. 按一下 **新增**，然後選擇管理員設定的Experience Manager Assets整合。

   >[!NOTE]
   >
   >您可以為此整合選擇任何名稱，因此不得具體提及Experience Manager Assets。

1. 選取您要的資產。

   ![](assets/select-an-asset.png)

1. 按一下 **連結**.
