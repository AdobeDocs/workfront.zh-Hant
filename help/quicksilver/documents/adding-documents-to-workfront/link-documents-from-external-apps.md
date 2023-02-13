---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 從外部應用程式連結文檔
description: 您可以從以下源將文檔和資料夾連結到Adobe Workfront - EDIT ME。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: 0ecee45183f5bc77a1c4a489013e486d8c26094c
workflow-type: tm+mt
source-wordcount: '2586'
ht-degree: 0%

---

# 從外部應用程式連結文檔

您可以透過下列來源將檔案和資料夾連結至Adobe Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">現有第三方雲文檔提供程式</td> 
   <td>其中包括： 
    <ul> 
     <li>方塊</li> 
     <li>Dropbox</li> 
     <li>Dropbox業務</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>MicrosoftSharePoint</li> 
     <li>Google Drive</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>您可以讓原本於Workfront Proof中建立的校樣，在Workfront中可用。 使用此功能需要Pro Workfront計畫或更高版本。 如需各種可用計畫的詳細資訊，請參閱 <a href="https://www.workfront.com/plans">Workfront計畫</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>您可以從Experience Manager Assets Essentials將檔案連結至Workfront。 如需詳細資訊，請參閱 <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront for Experience Manager Assets Essentials</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>這需要額外購買。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他檔案提供者（透過自訂檔案整合）</td> 
   <td> <p class="workfront_plans">使用此功能需要Pro Workfront計畫或更高版本。 如需各種可用計畫的詳細資訊，請參閱 <a href="https://www.workfront.com/plans">Workfront計畫</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

在連結文檔或資料夾之前，您的Workfront管理員必須為每個文檔提供程式或自定義文檔整合啟用此功能，如 [配置文檔整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

您可以透過直接上傳至Workfront的檔案，以與上傳至外部雲端提供者相同的方式，來校樣及核准連結至的檔案。 

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 檔案儲存

從外部應用程式連結至Workfront的檔案會與外部雲端提供者一起儲存，而非在Workfront內。

例外如下：

* 檔案服務提供時，縮圖和預覽影像可能會儲存在Workfront伺服器上。
* 當您在Workfront中使用校對時，檔案會複製並新增至校對伺服器。 

## 將檔案從外部應用程式連結至Workfront

您可以將現有檔案與外部雲端提供者連結。 這包括任何共用文檔。

* [必要條件](#prerequisites)
* [將外部檔案連結至Workfront](#link-an-external-document-to-workfront)
* [添加新版本的連結文檔](#add-a-new-version-of-a-linked-document)
* [連結Workfront校樣檔案](#link-workfront-proof-documents)
* [從Workfront中建立Google檔案](#create-a-google-document-from-within-workfront)

### 必要條件 {#prerequisites}

在連結文檔或資料夾之前，您的Workfront管理員必須為每個文檔提供程式或自定義文檔整合啟用此功能，如 [配置文檔整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### 將外部檔案連結至Workfront {#link-an-external-document-to-workfront}

您可以將檔案從外部應用程式(例如Google和Microsoft OneDrive)連結至Workfront。

>[!IMPORTANT]
>
>Dropbox根據檔案路徑儲存檔案。 因此，如果移動、重新命名或刪除從Dropbox連結的檔案，在Workfront中將無法存取。

1. 前往 **檔案** 在Workfront中您想要文檔的區域。
1. 按一下 **新增**，然後按一下要將文檔連結到Workfront的外部文檔提供程式。

   例如，要從Dropbox連結文檔，請按一下 **從Dropbox**.

   您已授權的外部提供者會顯示在清單頂端。

1. （條件性）如果系統提示您登入外部服務，請在顯示的方塊中輸入服務的登入認證，然後按一下 **登入**.
1. （條件性）如果系統提示您授權外部應用程式，請按一下 **授權** 按鈕。

   你只需要做一次。

1. 在 **連結外部檔案和資料夾** 框中，鍵入要搜索的項的名稱，然後按鍵 **輸入** 查看外部應用程式的所有結果，而無論其儲存在哪個資料夾中。

   或

   瀏覽並選擇要連結的文檔。

   雖然可以選擇多個文檔，但僅連結當前視圖中選擇的文檔。 例如，如果選擇文檔，然後進入資料夾，則最初選擇的文檔不會連結。

1. （視條件而定）如果您是Workfront DAM客戶，請按一下 **縮圖** 表徵圖將檔案顯示為縮圖影像。

   >[!NOTE]
   Workfront DAM客戶從Workfront DAM連結檔案時可以檢視縮圖。 Workfront DAM客戶可能也會針對其他服務(例如Dropbox和方塊)顯示縮圖。 不過，在Workfront中檢視Workfront DAM以外服務的縮圖並不受支援，而且從SharePoint或Google驅動器連結檔案時，不會顯示縮圖。

1. 按一下 **連結**.

   在Workfront中，雲端提供者的圖示會出現在檔案旁。

   >[!NOTE]
   對於連結到Box的文檔，在刷新頁面之前，不會顯示連結到Box中的文檔。

### 添加新版本的連結文檔 {#add-a-new-version-of-a-linked-document}

您可以從外部應用程式新增連結至Workfront的檔案新版本。

1. 前往 **檔案** 連結文檔的區域，然後選擇連結的文檔。

   >[!IMPORTANT]
   文檔必須位於連結資料夾之外才能建立新版本。

1. 按一下 **新增** > **版本**，然後按一下外部文檔提供程式。

   例如，要從Dropbox連結新版本的文檔，請按一下 **從Dropbox**.

   您已授權的外部提供者會顯示在清單頂端。

1. （條件性）如果系統提示您登入外部服務，請在顯示的方塊中輸入服務的登入認證，然後按一下 **登入**.
1. （條件性）如果系統提示您授權外部應用程式，請按一下 **授權**.

   你只需要做一次。

1. 在 **連結外部檔案和資料夾** 框中，鍵入要搜索的項的名稱，然後按鍵 **輸入** 查看外部應用程式的所有結果，而無論其儲存在哪個資料夾中。

   或

   瀏覽並選擇要連結的文檔。

   可以選擇多個文檔；但是，僅連結當前視圖中選擇的文檔。 例如，如果選擇文檔，然後進入資料夾，則最初選擇的文檔不會連結。

1. （視條件而定）如果您是Workfront DAM客戶，請按一下 **縮圖** 表徵圖將檔案顯示為縮圖影像。

   >[!NOTE]
   Workfront DAM客戶從Workfront DAM連結檔案時可以檢視縮圖。 Workfront DAM客戶可能也會針對其他服務(例如Dropbox和方塊)顯示縮圖。 不過，在Workfront中檢視Workfront DAM以外服務的縮圖並不受支援，而且從SharePoint或Google驅動器連結檔案時，不會顯示縮圖。

1. 按一下 **連結**.

   在Workfront中，雲端提供者的圖示會出現在檔案旁，指出它們已連結至外部雲端提供者。

   >[!NOTE]
   對於連結到Box的文檔，在刷新頁面之前，不會顯示連結到Box中的文檔。

有關添加已從檔案系統上載到Workfront的新版本的文檔的資訊，請參見 [從您的檔案系統將檔案新增至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#adding-new-versions-of-documents) in [從您的檔案系統將檔案新增至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### 連結Workfront校樣檔案 {#link-workfront-proof-documents}

您可以將校樣連結至原本存在於Workfront Proof的Workfront。 當您從Workfront Proof連結校樣時，Workfront中會提供與校樣相關聯的所有註解和其他中繼資料。 

您只能連結在Workfront校樣中具有「檢視」存取權的校樣。

1. 前往 **檔案** 在Workfront中您想要文檔的區域。
1. 按一下 **新增**，然後按一下 **從Workfront校樣**.

   >[!NOTE]
   此功能表中的選項可能會因環境中設定的第三方提供者而異。

1. 在 **連結** 校樣 **從** Workfront校樣方塊隨即出現，開始輸入您要在Workfront中使用的校樣名稱。

   清單會隨您輸入而篩選。

1. 選取最多10個要連結的校樣。

   任何灰色的校樣名稱無法連結，因為校樣已與Workfront中的檔案相關聯。

1. 按一下 **連結**.

   校樣的最新版本已連結至Workfront。 當您開啟校樣時，校樣檢視器中會提供所有版本。

### 從Workfront中建立Google檔案 {#create-a-google-document-from-within-workfront}

您可以從Workfront中建立新的Google檔案。 您無法從Workfront內為其他雲端提供者建立新檔案。

1. 前往 **檔案** 在Workfront中您想要文檔的區域。
1. 按一下 **新增** > **Google檔案**，然後選取您要建立的Google檔案類型。

1. 選擇要建立的Google文檔類型。
1. 若 **添加Google驅動器帳戶** 框中，按一下 **授權Googe Drive**.

   Google檔案會新增至 **檔案** 標籤。

   >[!NOTE]
    「My Drive（我的驅動器）」和「Shared with Me（與我共用）」顯示兩個不同的結果。 如果在「My Drive（我的驅動器）」中找不到檔案，請檢查「Shared with Me（與我共用）」資料夾。

## 將檔案從Workfront更新並連結至外部雲端提供者

您可以上傳檔案，並將其從Workfront連結至外部雲端提供者。 這會將檔案的儲存空間從Workfront移至外部雲端提供者。 當檔案在外部應用程式中變更時，會在Workfront中自動更新。

沒有Workfront存取權的使用者若有應用程式的存取權，可以在外部應用程式中查看檔案。

1. 選取在Workfront中上傳的檔案。
1. 按一下 **更多** >**傳送至**，然後選擇要儲存連結文檔的雲提供程式。

   您也可以使用「更多」功能表 ![](assets/more-icon.png) 在「文檔詳細資訊」頁上執行此操作。

1. 在提供程式的應用程式中選擇要儲存文檔的資料夾。

   這可以是提供程式應用程式中的任何資料夾，包括共用資料夾。

1. 按一下&#x200B;**儲存**。

   外部提供者的標誌會出現在檔案名稱旁，以指出檔案現在已連結至Workfront，並由外部雲端提供者儲存。

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## 連結資料夾

在Workfront和外部雲端提供者之間連結資料夾時，會連結該資料夾及其所有內容。 如果沒有Workfront存取權的使用者從外部檔案應用程式新增、移除和修改檔案，則其變更會同步至Workfront。 以下幾節將說明如何連結資料夾和子資料夾：

* [資料夾存取權限](#folder-access-rights)
* [連結一或多個外部資料夾](#link-one-or-more-external-folders)
* [將子資料夾添加到連結的資料夾](#add-subfolders-to-a-linked-folder)

### 資料夾存取權限 {#folder-access-rights}

從外部檔案應用程式同步資料夾內容時，Workfront會使用最初連結資料夾之使用者的認證。 這會產生下列使用者體驗：

* 如果使用者沒有在外部應用程式中檢視檔案和資料夾的存取權，但有透過Workfront檢視連結資料夾的存取權，則只能檢視Workfront中檔案和資料夾的名稱，不能檢視其內容。
* 當某人存取其他使用者連結至Workfront的連結資料夾內的內容（例如連結資料夾中的子資料夾）時，內容會使用最初連結資料夾的使用者的Workfront登入憑證（而非存取內容之使用者的憑證）同步至Workfront。

>[!IMPORTANT]
* 如果原本連結資料夾的使用者從Workfront系統中移除，使用者將無法再透過Workfront存取連結資料夾的內容。 在此情況下，資料夾必須由具有外部應用程式中資料夾權限的作用中Workfront使用者重新連結。
* 如果連結資料夾的使用者無法再存取外部應用程式，Workfront將無法再存取資料夾的內容。 例如，如果原本連結資料夾的使用者離開公司，就可能會發生此情況。 若要確保持續存取，具有資料夾存取權的使用者必須重新連結資料夾。


### 連結一或多個外部資料夾 {#link-one-or-more-external-folders}

1. 前往Workfront中您要資料夾的區域，然後按一下  **檔案** ![](assets/document-icon.png) 中。

1. 按一下 **新增**，然後按一下要將資料夾連結到Workfront的外部文檔提供程式。
1. （條件性）如果您尚未授權外部服務，請指定外部提供者的登入憑證，然後按一下 **登入**.

   您已授權的外部提供者會顯示在清單頂端。

1. 在 **連結外部檔案和資料夾** 框中，瀏覽並選擇要連結的資料夾。

   或

   輸入要搜索的資料夾名稱，然後按 **輸入**.

   您可以選取多個資料夾；但是，僅連結當前視圖中選定的資料夾。 例如，如果您選取資料夾，然後進入資料夾，則最初選取的資料夾不會連結。

   >[!NOTE]
   從Google驅動器連結資料夾時，您只能連結個人驅動器（我的驅動器）和團隊驅動器中的資料夾。 無法從「與我共用」區域連結資料夾。

1. 按一下 **連結**.

   在Workfront中，雲端提供者的標誌會顯示在資料夾旁，指出其已連結至外部雲端提供者。

1. （可選）要更名資料夾，使Workfront中的資料夾名稱與外部文檔應用程式中的資料夾名稱不同，請在 **資料夾** ，按一下「更多」菜單 ![](assets/more-icon.png)  顯示在資料夾名稱旁，然後按一下 **重新命名**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

這不會重新命名外部應用程式中的資料夾。

### 將子資料夾添加到連結的資料夾  {#add-subfolders-to-a-linked-folder}

您可以在現有連結資料夾內建立新資料夾。 您也可以將另一個資料夾拖曳至現有的連結資料夾。

1. 若要在現有連結資料夾內建立新資料夾，請移至現有資料夾，然後建立新資料夾，如 [建立文檔資料夾](../../documents/organizing-documents/create-documents-folder.md).

   或

   要將現有資料夾拖動到現有連結資料夾中，請轉至要將子資料夾拖動到的「文檔」區域，然後將其拖動到連結資料夾中。

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   將現有的Workfront資料夾拖曳至連結的資料夾時，會套用下列限制：
   * 您拖動的資料夾不能已連結，也不能包含任何已連結的內容。
   * 您拖曳的資料夾（包括其內容）不得超過50 MB。


## 將文檔添加到連結的資料夾

透過Workfront將檔案新增至連結的資料夾時，系統會自動將其新增為連結的檔案。

1. 在 **檔案** 將文檔拖動到連結資料夾的區域。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode"> <img src="assets/documents-linked-document-move-nwe-350x126.png" style="width: 350;height: 126;">Selection box is wonky on the left<br></p>
   -->

   或

   選擇要獲取文檔的連結資料夾，按一下 **添加新文檔>文檔**，然後瀏覽到文檔並將其添加到資料夾。

   系統會自動在外部應用程式中建立新版本的檔案，並連結至Workfront。

## 刪除連結的文檔或資料夾

從外部應用程式刪除連結的文檔或資料夾時，該文檔或資料夾將保留在Workfront系統中，直到從Workfront中刪除它為止。

1. 選擇連結的文檔或資料夾，然後按一下 **刪除**.
1. 在顯示的確認方塊中，按一下 **是，取消連結**.

   檔案會從Workfront網站取消連結。 它不會在外部應用程式中受到影響。

## 關於更名連結的文檔和資料夾

更名連結的文檔或資料夾時，更改只在您進行更改的應用程式中可見。 例如，如果在Workfront中重新命名連結的檔案，則新名稱只會顯示在Workfront中。

如果您想要在Workfront和外部應用程式中比對名稱，必須同時在兩處重新命名名稱。

>[!IMPORTANT]
請勿更名Workfront中連結至Dropbox的檔案；如此會導致無法存取Workfront中的檔案。 請改為以Dropbox重新命名檔案，然後重新同步檔案，如 [從外部應用程式連結文檔](#synchronizing-changes-made-on-a-linked-document).
