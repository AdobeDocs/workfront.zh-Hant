---
product-area: documents
navigation-topic: organize-documents
title: 建立檔案資料夾
description: 檔案可整理到資料夾中。 您可以在個人的「檔案」區域中建立個人資料夾。
author: Courtney
feature: Digital Content and Documents
exl-id: 41974d6b-fb00-49b7-9db2-36519994e0fd
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 2%

---

# 建立檔案資料夾

檔案可整理到資料夾中。 Workfront目前有兩個版本的檔案區域：舊版檔案區域和新檔案區域。 您的組織所使用的版本取決於您的組織是在舊版Workfront儲存空間還是企業儲存空間。 如需這些儲存體型別的詳細資訊，請參閱[Adobe企業儲存體概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存來管理檔案的任何Workfront套件</p>
<p>使用Adobe企業儲存體管理檔案的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或以上</p>
   <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在舊版檔案區域中建立檔案資料夾

如果您的組織位於舊版Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需有關舊版Workfront儲存體的詳細資訊，請參閱[Adobe企業儲存體與舊版Workfront儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage)。

>[!NOTE]
>
>組織檔案只會建立檔案與關聯它們的物件之間的連結。 它不會在系統中重新定位它們。

### 顯示資料夾

您可以在縮圖、標準或清單檢視中顯示資料夾。 若要變更檢視，請使用右上角的檢視選項。

{{step1-to-documents}}

或

開啟Workfront物件後，按一下左側面板中的&#x200B;**檔案**。

1. Click the view options above the right panel to change how the documents are displayed.

   ![Document view options](assets/screenshot-2016-07-07-12.46.54.png)

### Create folders and subfolders

Create folders to better organize your documents. You can create up to 2,000 folders on an object and up to 50 subfolders within each folder. Subfolders count towards the 2,000 folder maximum.

{{step1-to-documents}}

或

開啟Workfront物件後，按一下左側面板中的&#x200B;**檔案**。

1. To create a top-level folder, ensure that nothing is selected, then click **Add New** > **Folder**.

   或

   To create a sub-folder, select the folder where you want to create the sub-folder, then click **Add New** > **Folder**.

### Sharing folders

For information about sharing folders, see [Share a document folder](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Create document folders in the new documents area

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 如需企業儲存的詳細資訊，請參閱[Adobe企業儲存概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

### System-generated folders

When you upload a document to a task or issue, Workfront automatically creates a system-generated folder named after the task or issue. This folder is linked to the task or issue and inherits its permissions. System-generated folders are visible in the project-level documents area.

For more information about folder permissions, see [How document permissions work](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

### Create subfolders

You can create subfolders within a system-generated folder to organize documents further. All subfolders inherit permissions from the parent folder.

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.
1. Click into the folder you want to create a subfolder in, then click the **Add folder** ![add folder icon](assets/add-folder-icon.png) icon.
   ![add subfolder](assets/add-subfolder.png)
1. 輸入子資料夾的名稱，然後按一下[建立]。**&#x200B;**

### 重新命名資料夾

系統產生的資料夾會自動繼承任務或問題的名稱。 按一下資料夾名稱並加以編輯即可重新命名。

若要重新命名資料夾：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。
1. 找到您要重新命名的資料夾，然後按一下&#x200B;**更多** ![更多](assets/more-icon.png)圖示。
1. 按一下&#x200B;**重新命名**，然後輸入資料夾的新名稱。

   ![重新命名資料夾](assets/rename-folder.png)

1. 按一下&#x200B;**重新命名**。

### 行動資料夾

系統產生的資料夾可以移動到另一個專案、任務或問題。 如果系統產生的資料夾移至其他位置，其連結物件會更新為新物件，許可權會繼承自新的父物件。 您也可以將子資料夾移至另一個專案、任務或問題。

>[!NOTE]
>
>移動對話方塊中只能使用相同儲存型別的專案、任務和問題。 例如，如果您是在企業儲存體專案中行動資料夾，則只有使用企業儲存體的專案、任務和問題才能移動到。


若要行動資料夾：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。
1. 找到您要移動的資料夾，然後按一下&#x200B;**更多** ![更多](assets/more-icon.png)圖示。
1. 按一下&#x200B;**移動**，然後選取您要行動資料夾的專案、任務或問題。


   ![行動資料夾](assets/rename-folder.png)

<!-- STEPS PLACEHOLDER: Add steps for moving a folder in the new documents area -->

### 刪除資料夾

若要刪除資料夾：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。
1. 找到您要刪除的資料夾，然後按一下&#x200B;**更多** ![更多](assets/more-icon.png)圖示。
1. 按一下&#x200B;**刪除**。

   ![delete folder](assets/rename-folder.png)
