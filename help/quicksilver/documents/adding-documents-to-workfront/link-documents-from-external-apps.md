---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 從外部應用程式連結檔案
description: 您可以從外部來源將檔案和資料夾連結到Adobe Workfront。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '2592'
ht-degree: 1%

---

# 從外部應用程式連結檔案

<!-- Audited: 01/2024 -->

您可以從下列來源將檔案和資料夾連結至Adobe Workfront：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">現有的第三方雲端檔案提供者</td> 
   <td>這些功能包括： 
    <ul> 
     <li>方塊</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
     <li>Quip</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>您可以在Workfront中提供原本在Workfront Proof中建立的校樣。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>您可以從Experience Manager Assets Essentials將檔案連結到Workfront。 如需詳細資訊，請參閱<a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref">適用於Experience Manager Assets Essentials的Adobe Workfront</a>。</td> 
  </tr>

<tr> 
   <td role="rowheader">其他檔案提供者（透過自訂檔案整合）</td> 
   <td> <p class="workfront_plans">這些整合功能可在「設定」區域中設定。</p> </td>
  </tr> 
 </tbody> 
</table>

連結檔案或資料夾之前，您的Workfront管理員必須為每個檔案提供者或自訂檔案整合啟用此功能，如[設定檔案整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md)中所述。

您可以校訂和核准連結至外部雲端提供者的檔案，就像直接上傳至Workfront的檔案一樣。

>[!NOTE]
>
>新檔案區域未提供此功能。<br>
>如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 如需企業儲存的詳細資訊，請參閱[Adobe企業儲存概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td>
   <td> <p>任何</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td>
   <td><p>投稿人或以上</p>
    <p>要求或更高版本</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檔案儲存

從外部應用程式連結至Workfront的檔案會儲存於外部雲端提供者，而非儲存在Workfront中。

The following exceptions apply:

* When provided by the document service, thumbnails and preview images might be stored on Workfront servers.
* When you use proofing in Workfront, the document is copied and added to the proofing servers.

## File size limits

Third-party cloud providers:

* Single file: 5 GB or less
* Multiple file: 1 GB or less (total of all files)

## Link a document from an external application to Workfront

You can link existing documents with an external cloud provider. This includes any shared documents.

### 先決條件 {#prerequisites}

連結檔案或資料夾之前，您的Workfront管理員必須為每個檔案提供者或自訂檔案整合啟用此功能，如[設定檔案整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md)中所述。

### Link an external document to Workfront {#link-an-external-document-to-workfront}

You can link documents to Workfront from an external application such as Google and Microsoft OneDrive.

>[!IMPORTANT]
>
>Dropbox stores documents based on the file path. Because of this, if a file linked from Dropbox is moved, renamed, or deleted, it becomes inaccessible in Workfront.

1. Go to the **Documents** area in Workfront where you want the document.
1. Click **Add New**, then click the external document provider where you want to link documents to Workfront.

   For example, to link documents from Dropbox, click **From Dropbox**.

   External providers that you have already authorized appear at the top of the list.

1. (Conditional) If you are prompted to log into the external service, type your login credentials for the service in the box that appears, then click **Sign in**.
1. (Conditional) If you are prompted to authorize the external application, click the **Authorize** button.

   You need to do this only once.

1. In the search box of the **Link External Files and Folders** box that appears, type the name of the item you want to search for, then press **Enter** to see all results from the external application, regardless of which folder they are storied in.

   或

   Browse to and select the documents you want to link.

   Though you can select multiple documents, only documents that are selected in the current view are linked. 例如，如果您選取檔案，然後進入資料夾，則不會連結您最初選取的檔案。

1. （視條件而定）如果您是Workfront DAM客戶，請按一下&#x200B;**縮圖**&#x200B;圖示，將檔案顯示為縮圖影像。

   >[!NOTE]
   >
   >Workfront DAM客戶在從Workfront DAM連結檔案時，可檢視縮圖。 也會針對Workfront DAM客戶顯示其他服務（例如Dropbox和Box）的縮圖。 但是，不支援在Workfront中檢視Workfront DAM以外服務的縮圖，而且在從SharePoint或Google Drive連結檔案時，不會顯示縮圖。

1. 按一下&#x200B;**連結**。

   在Workfront中，雲端提供者的圖示會出現在檔案旁。

   >[!NOTE]
   >
   >* 如果用來連結檔案的下載URL超過2048個字元，則檔案無法連結。
   >* 對於連結到Box的檔案，在您重新整理頁面之前，不會顯示Box中檔案的連結。

### 新增連結檔案的新版本 {#add-a-new-version-of-a-linked-document}

您可以從外部應用程式新增連結至Workfront的檔案的新版本。

1. 移至連結檔案的&#x200B;**檔案**&#x200B;區域，然後選取連結的檔案。

   >[!IMPORTANT]
   >
   >檔案必須位於連結的資料夾之外，才能建立新版本。

1. 按一下&#x200B;**新增** > **版本**，然後按一下外部檔案提供者。

   例如，若要從Dropbox連結檔案的新版本，請按一下[從Dropbox連結] **&#x200B;**。

   您已經授權的外部提供者會出現在清單頂端。

1. （視條件而定）如果系統提示您登入外部服務，請在顯示的方塊中輸入服務的登入認證，然後按一下&#x200B;**登入**。
1. （視條件而定）如果系統提示您授權外部應用程式，請按一下&#x200B;**授權**。

   您只需執行此操作一次。

1. 在出現的&#x200B;**連結外部檔案和資料夾**&#x200B;方塊的搜尋方塊中，輸入您要搜尋的專案名稱，然後按&#x200B;**Enter**&#x200B;檢視來自外部應用程式的所有結果，無論這些結果儲存在哪個資料夾中。

   或

   瀏覽並選取您要連結的檔案。

   您可以選取多個檔案；不過，只會連結在目前檢視中選取的檔案。 例如，如果您選取檔案，然後進入資料夾，則不會連結您最初選取的檔案。

1. （視條件而定）如果您是Workfront DAM客戶，請按一下&#x200B;**縮圖**&#x200B;圖示，將檔案顯示為縮圖影像。

   >[!NOTE]
   >
   >Workfront DAM客戶在從Workfront DAM連結檔案時，可檢視縮圖。 也會針對Workfront DAM客戶顯示其他服務（例如Dropbox和Box）的縮圖。 但是，不支援在Workfront中檢視Workfront DAM以外服務的縮圖，而且在從SharePoint或Google Drive連結檔案時，不會顯示縮圖。

1. 按一下&#x200B;**連結**。

   在Workfront中，雲端提供者的圖示會出現在檔案旁邊，表示這些檔案已連結至外部雲端提供者。

   >[!NOTE]
   >
   >對於連結到Box的檔案，在您重新整理頁面之前，不會顯示Box中檔案的連結。

如需有關從您的檔案系統新增檔案版本至Workfront的資訊，請參閱[從您的檔案系統新增檔案至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)中的[新增檔案至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront)。

### 連結Workfront Proof檔案 {#link-workfront-proof-documents}

您可以將校訂連結至原本存在於Workfront Proof中的Workfront。 當您從Workfront Proof連結校訂時，所有與校訂相關的評論和其他中繼資料都可在Workfront中使用。

您只能連結在Workfront Proof中您擁有檢視存取權的校訂。

1. 移至Workfront中您想要檔案的&#x200B;**檔案**&#x200B;區域。
1. 按一下[新增] **&#x200B;**，然後按一下&lbrack;來自Workfront Proof的&#x200B;**&#x200B;**。

   >[!NOTE]
   >
   >此功能表中的選項可能會因環境中設定的協力廠商提供者而異。

1. 在出現的&#x200B;**從Workfront Proof連結校樣**&#x200B;方塊中，開始輸入您要在Workfront中提供的校樣名稱。

   當您輸入時，清單會經過篩選。

1. 選取最多10個要連結的校訂。

   任何變暗的校訂名稱都無法連結，因為校訂已與Workfront中的檔案相關聯。

1. 按一下&#x200B;**連結**。

   最新版本的校訂連結至Workfront。 開啟校訂時，校訂檢視器中會提供所有版本。

### 在Workfront中建立Google檔案 {#create-a-google-document-from-within-workfront}

您可以在Workfront中建立新的Google檔案。 您無法在Workfront中為其他雲端服務供應商建立新檔案。

1. 移至Workfront中您想要檔案的&#x200B;**檔案**&#x200B;區域。
1. 按一下&#x200B;**新增** > **Google檔案**，然後選取您要建立的Google檔案型別。
1. 如果出現&#x200B;**新增Google磁碟機帳戶**&#x200B;方塊，請按一下&#x200B;**授權Google磁碟機**。

   Google檔案已新增至&#x200B;**檔案**&#x200B;索引標籤。

   >[!NOTE]
   >
   > 「我的磁碟機」和「與我共用」會顯示兩個不同的結果。 如果您在[我的磁碟機]中找不到檔案，請存取[與我共用]資料夾。

## Upload and link a document from Workfront to an external cloud provider

You can upload and link a document from Workfront to an external cloud provider. This moves storage of the document from Workfront to the external cloud provider. 當檔案在外部應用程式中變更時，會自動在Workfront中更新。

>[!NOTE]
>
>將資產傳送至外部檔案供應者時，會建立資產的新版本。

沒有Workfront存取許可權的使用者如果擁有應用程式的存取許可權，便可以在外部應用程式中檢視檔案。

1. 選取在Workfront中上傳的檔案。
1. 按一下&#x200B;**更多** >**傳送至**，然後選取您要儲存連結檔案的雲端提供者。

   您也可以使用[檔案詳細資訊]頁面上的[更多]功能表![[更多]功能表](assets/more-icon.png)來執行此操作。

1. 在提供者的應用程式中，選取您要儲存檔案的資料夾。

   This can be any folder in the provider&#39;s application, including a shared folder.

1. 按一下「**儲存**」。

   外部提供者的標誌會出現在檔名稱旁，表示檔案現在已連結至Workfront並由外部雲端提供者儲存。

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## 連結資料夾

當您在Workfront和外部雲端提供者之間連結資料夾時，該資料夾及其所有內容都會連結。 If users without Workfront access add, remove, and modify files from the external document application, their changes are synchronized to Workfront.

### 資料夾存取權 {#folder-access-rights}

When synchronizing folder content from an external document application, Workfront uses the credentials of the user who originally linked the folder. 這會產生以下使用者體驗：

* If users do not have access to view files and folders in the external application, but do have access to view the linked folder via Workfront, they can view only the names of the files and folders in Workfront, not their contents.
* 當有人存取Workfront中由其他使用者連結至Workfront的連結資料夾（例如連結資料夾中的子資料夾）內的內容時，內容會使用原本連結資料夾的使用者Workfront登入認證（而非存取內容的使用者認證）同步至Workfront。

>[!IMPORTANT]
>
>* If the user who originally linked the folder is removed from the Workfront system, users are no longer able to access content on the linked folder via Workfront. In this case, the folder must be relinked by an active Workfront user who has rights to the folder in the external application.
>* If the user who linked a folder no longer has access to the external application, Workfront can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.

### Link one or more external folders {#link-one-or-more-external-folders}

1. Go to the area in Workfront where you want the folder, then click  **Documents** ![Documents icon](assets/document-icon.png) in the left panel .

1. Click **Add New**, then click the external document provider from which you want to link a folder to Workfront.
1. (Conditional) If you have not yet authorized the external service, specify your login credentials for the external provider, then click **Sign in**.

   您已經授權的外部提供者會出現在清單頂端。

1. In the **Link External Files and Folders** box that appears, browse to and select the folders you want to link.

   或

   Type the name of the folder you want to search for, then press **Enter**.

   You can select multiple folders; however, only folders that are selected in the current view are linked. For example, if you select a folder, then go into a folder, the folder you originally selected is not linked.

   >[!NOTE]
   >
   >When linking folders from Google Drive, you can only link folders that are within your personal drive (My Drive) and Team Drive. You cannot link folders from the Shared with Me area.

1. 按一下&#x200B;**連結**。

   In Workfront, the cloud provider&#39;s logo displays next to the folder, indicating that it is linked to the external cloud provider.

1. (Optional) To rename the folder so that the folder name in Workfront is different from the folder name in the external document application, select the folder in the **Folders** section, click the  More menu ![More menu](assets/more-icon.png)  that displays next to the folder name, then click **Rename**.

   ![Rename folder](assets/documents-folderlink-rename-nwe-350x154.png)

This does not rename the folder in the external application.

### Add subfolders to a linked folder  {#add-subfolders-to-a-linked-folder}

You can create a new folder inside an existing linked folder. You can also drag another folder into an existing linked folder.

1. To create a new folder within an existing linked folder, go to the existing folder, then create the new folder as described in [Create document folders](../../documents/organizing-documents/create-documents-folder.md).

   或

   若要將現有資料夾拖曳至現有的連結資料夾，請移至您想要子資料夾的「檔案」區域，然後將其拖曳至連結資料夾。

   ![拖曳至連結的資料夾](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >將現有Workfront資料夾拖曳至連結資料夾時，適用下列限制：
   >
   >* 您正在拖曳的資料夾無法連結，也無法包含任何已連結的內容。
   >* 您要拖曳的資料夾（包括其內容）不可超過50 MB。

## 將檔案新增至連結的資料夾

當您透過Workfront將檔案新增至連結資料夾時，會自動新增為連結檔案。

1. 選取您想要檔案的連結資料夾，按一下&#x200B;**新增>檔案**，然後瀏覽至檔案並將其新增至資料夾。

   或

   在您想要檔案的&#x200B;**檔案**&#x200B;區域中，將檔案拖曳至連結的資料夾。

   您檔案的新版本會自動在外部應用程式中建立，並連結至Workfront。

>[!NOTE]
>
> * 檔案正在移動時，檔案選項不可用。
>
> * 檔案移至Experience Manager Assets後，Workfront的檔案清單中將不再顯示。
>
> * 您在檔案移動時對它所做的任何動作或編輯都不會顯示在Experience Manager Assets的檔案中，因此將會遺失。

## 刪除連結的檔案或資料夾

當您從外部應用程式中刪除連結的檔案或資料夾時，該檔案或資料夾會保留在Workfront系統中，直到您也從Workfront中刪除它為止。

1. 選取連結的檔案或資料夾，然後按一下&#x200B;**刪除**。
1. 在出現的確認方塊中，按一下&#x200B;**是，取消連結**。

   檔案會從Workfront網站取消連結。 在外部應用程式中不受影響。

## 關於重新命名連結的檔案和資料夾

當您重新命名連結的檔案或資料夾時，變更只會顯示在您執行變更的應用程式中。 例如，如果您在Workfront中重新命名連結的檔案，新名稱僅會顯示在Workfront中。

如果您希望名稱在Workfront和外部應用程式中保持一致，則必須在兩個位置將其重新命名。

>[!IMPORTANT]
>
>請勿重新命名連結至Dropbox的Workfront檔案，否則會導致Workfront中的檔案無法存取。 請改為在Dropbox中重新命名檔案，然後重新同步檔案。
