---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 從外部應用程式連結檔案
description: 您可以從下列來源將檔案和資料夾連結至Adobe Workfront — 編輯我。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: 5122914acd0ae0fdfb8a5ae7319075ce1072962e
workflow-type: tm+mt
source-wordcount: '2648'
ht-degree: 0%

---

# 從外部應用程式連結檔案

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
     <li>Dropbox企業</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>您可以讓原本在Workfront Proof中建立的校訂可在Workfront中使用。 使用此功能需要Pro Workfront Plan或更高版本。 如需各種可用計畫的詳細資訊，請參閱 <a href="https://www.workfront.com/plans">Workfront計畫</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>您可以從Experience Manager Assets Essentials將檔案連結到Workfront。 如需詳細資訊，請參閱 <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> 適用於Experience Manager Assets Essentials的Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>這需要進行額外購買。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他檔案提供者（透過自訂檔案整合）</td> 
   <td> <p class="workfront_plans">使用此功能需要Pro Workfront Plan或更高版本。 如需各種可用計畫的詳細資訊，請參閱 <a href="https://www.workfront.com/plans">Workfront計畫</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

在連結檔案或資料夾之前，您的Workfront管理員必須為每個檔案提供者或自訂檔案整合啟用此功能，如中所述 [設定檔案整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

您可以透過與直接上傳至Workfront的檔案相同的方法，校訂及核准連結至外部雲端提供者的檔案。

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
   <td> <p>要求或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 檔案儲存

從外部應用程式連結至Workfront的檔案會與外部雲端提供者儲存，而不會儲存在Workfront中。

適用下列例外：

* 若由檔案服務提供，縮圖和預覽影像可能會儲存在Workfront伺服器上。
* 當您在Workfront中使用校訂時，檔案會被複製並新增至校訂伺服器。

## 將檔案從外部應用程式連結至Workfront

您可以將現有檔案與外部雲端提供者連結。 這包括任何共用檔案。

* [必要條件](#prerequisites)
* [將外部檔案連結至Workfront](#link-an-external-document-to-workfront)
* [新增連結檔案的新版本](#add-a-new-version-of-a-linked-document)
* [連結Workfront校訂檔案](#link-workfront-proof-documents)
* [從Workfront中建立Google檔案](#create-a-google-document-from-within-workfront)

### 必要條件 {#prerequisites}

在連結檔案或資料夾之前，您的Workfront管理員必須為每個檔案提供者或自訂檔案整合啟用此功能，如中所述 [設定檔案整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### 將外部檔案連結至Workfront {#link-an-external-document-to-workfront}

您可以從外部應用程式(例如Google和Microsoft OneDrive)將檔案連結至Workfront。

>[!IMPORTANT]
>
>Dropbox會根據檔案路徑來儲存檔案。 因此，如果移動、重新命名或刪除從Dropbox連結的檔案，將無法在Workfront中存取。

1. 前往 **檔案** Workfront中您想要檔案的區域。
1. 按一下 **新增**，然後按一下您要將檔案連結至Workfront的外部檔案提供者。

   例如，若要從Dropbox連結檔案，請按一下 **從Dropbox**.

   您已經授權的外部提供者會出現在清單頂端。

1. （視條件而定）如果系統提示您登入外部服務，請在顯示的方塊中輸入服務的登入認證，然後按一下 **登入**.
1. （視條件而定）如果系統提示您授權外部應用程式，請按一下 **授權** 按鈕。

   您只需執行此動作一次。

1. 在的搜尋方塊中 **連結外部檔案和資料夾** 方塊中，輸入您要搜尋的專案名稱，然後按 **輸入** 以檢視外部應用程式的所有結果，無論結果位於哪個資料夾中。

   或

   瀏覽並選取您要連結的檔案。

   雖然您可以選取多個檔案，但只會連結在目前檢視中選取的檔案。 例如，如果您選取檔案，然後進入資料夾，則您最初選取的檔案不會連結。

1. （視條件而定）如果您是Workfront DAM客戶，請按一下 **縮圖** 圖示以將檔案顯示為縮圖影像。

   >[!NOTE]
   >
   >從Workfront DAM連結檔案時，Workfront DAM客戶可以檢視縮圖。 也會針對Workfront DAM客戶顯示其他服務(例如Dropbox和Box)的縮圖。 不過，不支援在Workfront中檢視Workfront DAM以外服務的縮圖，而且在從SharePoint或Google Drive連結檔案時不會顯示縮圖。

1. 按一下 **連結**.

   在Workfront中，雲端提供者的圖示會出現在檔案旁邊。

   >[!NOTE]
   >
   >對於連結到Box的檔案，在您重新整理頁面之前，不會顯示Box中檔案的連結。

### 新增連結檔案的新版本 {#add-a-new-version-of-a-linked-document}

您可以從外部應用程式新增連結至Workfront的檔案的新版本。

1. 前往 **檔案** 連結檔案的區域，然後選取連結的檔案。

   >[!IMPORTANT]
   >
   >檔案必須位於連結的資料夾之外，才能建立新版本。

1. 按一下 **新增** > **版本**，然後按一下外部檔案提供者。

   例如，若要從Dropbox連結檔案的新版本，請按一下 **從Dropbox**.

   您已經授權的外部提供者會出現在清單頂端。

1. （視條件而定）如果系統提示您登入外部服務，請在顯示的方塊中輸入服務的登入認證，然後按一下 **登入**.
1. （視條件而定）如果系統提示您授權外部應用程式，請按一下 **授權**.

   您只需執行此動作一次。

1. 在的搜尋方塊中 **連結外部檔案和資料夾** 方塊中，輸入您要搜尋的專案名稱，然後按 **輸入** 以檢視外部應用程式的所有結果，無論結果位於哪個資料夾中。

   或

   瀏覽並選取您要連結的檔案。

   您可以選取多個檔案；但是，只會連結在目前檢視中選取的檔案。 例如，如果您選取檔案，然後進入資料夾，則您最初選取的檔案不會連結。

1. （視條件而定）如果您是Workfront DAM客戶，請按一下 **縮圖** 圖示以將檔案顯示為縮圖影像。

   >[!NOTE]
   >
   >從Workfront DAM連結檔案時，Workfront DAM客戶可以檢視縮圖。 也會針對Workfront DAM客戶顯示其他服務(例如Dropbox和Box)的縮圖。 不過，不支援在Workfront中檢視Workfront DAM以外服務的縮圖，而且在從SharePoint或Google Drive連結檔案時不會顯示縮圖。

1. 按一下 **連結**.

   在Workfront中，雲端提供者的圖示會出現在檔案旁邊，表示它們已連結至外部雲端提供者。

   >[!NOTE]
   >
   >對於連結到Box的檔案，在您重新整理頁面之前，不會顯示Box中檔案的連結。

如需有關新增檔案新版本的資訊，請參閱從檔案系統上傳到Workfront的檔案 [從您的檔案系統新增檔案至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#adding-new-versions-of-documents) 在 [從您的檔案系統新增檔案至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### 連結Workfront校訂檔案 {#link-workfront-proof-documents}

您可以將校訂連結至原本存在於Workfront Proof中的Workfront。 當您從Workfront Proof連結校訂時，可在Workfront中使用所有與校訂相關的評論和其他中繼資料。

您只能連結您在Workfront Proof中擁有檢視存取權的校訂。

1. 前往 **檔案** Workfront中您想要檔案的區域。
1. 按一下 **新增**，然後按一下 **來自Workfront Proof**.

   >[!NOTE]
   >
   >此功能表中的選項可能會因環境中設定的協力廠商提供者而異。

1. 在 **連結** 校樣 **從** Workfront校訂方塊中，開始輸入您要在Workfront中提供的校訂名稱。

   當您輸入時，清單會經過篩選。

1. 選取最多10個要連結的校訂。

   任何暗色的校樣名稱都無法連結，因為校樣已與Workfront中的檔案相關聯。

1. 按一下 **連結**.

   最新版本的校訂連結至Workfront。 開啟校訂時，校訂檢視器中會提供所有版本。

### 從Workfront中建立Google檔案 {#create-a-google-document-from-within-workfront}

您可以從Workfront中建立新的Google檔案。 您無法在Workfront中建立其他雲端提供者的新檔案。

1. 前往 **檔案** Workfront中您想要檔案的區域。
1. 按一下 **新增** > **Google檔案**，然後選取您要建立的Google檔案型別。

1. 選取您要建立的Google檔案型別。
1. 如果 **新增Google磁碟機帳戶** 方塊中，按一下 **授權Google Drive**.

   Google檔案已新增至 **檔案** 標籤。

   >[!NOTE]
   >
   > 「我的磁碟機」和「與我共用」會顯示兩個不同的結果。 如果您在[我的磁碟機]中找不到檔案，請存取[與我共用]資料夾。

## 更新檔案並將其從Workfront連結至外部雲端提供者

您可以從Workfront上傳檔案並將其連結至外部雲端提供者。 這會將檔案的儲存空間從Workfront移至外部雲端提供者。 當檔案在外部應用程式中變更時，會自動在Workfront中更新。

沒有Workfront存取許可權的使用者如果擁有應用程式的存取許可權，則可以在外部應用程式中檢視檔案。

1. 選取在Workfront中上傳的檔案。
1. 按一下 **更多** >**傳送至**，然後選取您要儲存連結檔案的雲端提供者。

   您也可以使用「更多」選單 ![](assets/more-icon.png) 檔案詳細資訊頁面執行此操作。

1. 在提供者的應用程式中選取要儲存檔案的資料夾。

   這可以是提供者應用程式中的任何資料夾，包括共用資料夾。

1. 按一下&#x200B;**儲存**。

   外部提供者的標誌會出現在檔名稱旁，表示檔案現在已連結至Workfront並由外部雲端提供者儲存。

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## 連結資料夾

當您在Workfront和外部雲端提供者之間連結資料夾時，該資料夾及其所有內容都會連結。 如果沒有Workfront存取許可權的使用者從外部檔案應用程式新增、移除和修改檔案，其變更會同步至Workfront。 以下各節說明如何連結資料夾和子資料夾：

* [資料夾存取許可權](#folder-access-rights)
* [連結一或多個外部資料夾](#link-one-or-more-external-folders)
* [將子資料夾新增至連結的資料夾](#add-subfolders-to-a-linked-folder)

### 資料夾存取許可權 {#folder-access-rights}

從外部檔案應用程式同步資料夾內容時，Workfront會使用最初連結資料夾之使用者的認證。 這會產生下列使用者體驗：

* 如果使用者無權在外部應用程式中檢視檔案和資料夾，但有權透過Workfront檢視連結的資料夾，則他們只能在Workfront中檢視檔案和資料夾的名稱，不能檢視其內容。
* 當有人存取Workfront中由其他使用者連結至Workfront的連結資料夾（例如連結資料夾中的子資料夾）內的內容時，內容會使用最初連結資料夾的使用者的Workfront登入認證，而不是存取內容的使用者的認證，同步至Workfront。

>[!IMPORTANT]
>
>* 如果從Workfront系統移除原本連結資料夾的使用者，使用者將無法再透過Workfront存取連結資料夾上的內容。 在此情況下，該資料夾必須由在外部應用程式中擁有該資料夾存取權的作用中Workfront使用者重新連結。
>* 如果連結資料夾的使用者無法再存取外部應用程式，Workfront就無法再存取資料夾的內容。 例如，如果最初連結資料夾的使用者離開公司，就可能發生這種情況。 為確保繼續存取，具有資料夾存取許可權的使用者必須重新連結資料夾。

### 連結一或多個外部資料夾 {#link-one-or-more-external-folders}

1. 前往Workfront中您要資料夾的區域，然後按一下  **檔案** ![](assets/document-icon.png) 在左側面板中。

1. 按一下 **新增**，然後按一下您要將資料夾連結至Workfront的外部檔案提供者。
1. （視條件而定）如果您尚未授權外部服務，請指定外部提供者的登入認證，然後按一下 **登入**.

   您已經授權的外部提供者會出現在清單頂端。

1. 在 **連結外部檔案和資料夾** 方塊中，瀏覽並選取您要連結的資料夾。

   或

   輸入您要搜尋的資料夾名稱，然後按鍵 **輸入**.

   您可以選取多個資料夾；不過，只會連結在目前檢視中選取的資料夾。 例如，如果您選取資料夾，然後進入資料夾，則您最初選取的資料夾不會連結。

   >[!NOTE]
   >
   >從Google Drive連結資料夾時，您只能連結位於個人磁碟機（我的磁碟機）和小組磁碟機中的資料夾。 您無法從「與我共用」區域連結資料夾。

1. 按一下 **連結**.

   在Workfront中，雲端提供者的標誌會顯示在資料夾旁，表示已連結至外部雲端提供者。

1. （可選）若要重新命名資料夾，使Workfront中的資料夾名稱與外部檔案應用程式中的資料夾名稱不同，請在 **資料夾** 區段，按一下「更多」功能表 ![](assets/more-icon.png)  檔案夾名稱旁顯示，然後按一下 **重新命名**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

這不會重新命名外部應用程式中的資料夾。

### 將子資料夾新增至連結的資料夾  {#add-subfolders-to-a-linked-folder}

您可以在現有的連結資料夾中建立新資料夾。 您也可以將另一個資料夾拖曳至現有的連結資料夾。

1. 若要在現有連結資料夾中建立新資料夾，請前往現有資料夾，然後建立新資料夾，如所述 [建立檔案資料夾](../../documents/organizing-documents/create-documents-folder.md).

   或

   若要將現有資料夾拖曳至現有連結資料夾，請前往您想要子資料夾的「檔案」區域，然後將其拖曳至連結資料夾。

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >將現有Workfront資料夾拖曳至連結資料夾時，適用下列限制：
   >
   >* 您正在拖曳的資料夾無法連結，也無法包含任何已連結的內容。
   >* 您要拖曳的資料夾（包括其內容）不可超過50 MB。

## 將檔案新增至連結的資料夾

當您透過Workfront將檔案新增至連結的資料夾時，會自動新增為連結的檔案。

1. 選取您想要檔案的連結資料夾，按一下 **新增>檔案**，然後瀏覽至檔案並將其新增至資料夾。



   或

   在 **檔案** 在您想要檔案的區域，將檔案拖曳到連結的資料夾中。

   您檔案的新版本會自動在外部應用程式中建立並連結至Workfront。

>[!NOTE]
>
> * 檔案正在移動時，檔案選項不可用。 檔案移至Experience Manager Assets後，Workfront的檔案清單中將不再顯示。
>
> * 您在檔案移動時對檔案所做的任何動作或編輯都不會顯示在Experience Manager Assets的檔案中，因此將會遺失。


## 刪除連結的檔案或資料夾

當您從外部應用程式中刪除連結的檔案或資料夾時，檔案或資料夾會保留在Workfront系統中，直到您也從Workfront中刪除它為止。

1. 選取連結的檔案或資料夾，然後按一下 **刪除**.
1. 在出現的確認方塊中，按一下 **是的，取消連結**.

   檔案會從Workfront網站取消連結。 它在外部應用程式中不受影響。

## 關於重新命名連結的檔案和資料夾

當您重新命名連結的檔案或資料夾時，變更只會顯示在您建立它的應用程式中。 例如，如果您在Workfront中重新命名連結的檔案，新名稱只會顯示在Workfront中。

如果您希望名稱在Workfront和外部應用程式中相符，則必須在這兩個位置重新命名。

>[!IMPORTANT]
>
>請勿重新命名連結至Dropbox的Workfront檔案；這樣做會使Workfront中的檔案無法存取。 請改為重新命名Dropbox的檔案，然後重新同步檔案，如中所述 [從外部應用程式連結檔案](#synchronizing-changes-made-on-a-linked-document).
