---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 從您的檔案系統新增檔案至Adobe Workfront
description: 您可以在Adobe Workfront中將檔案新增到多個區域中的專案、任務或問題。
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
source-git-commit: 47f029fbbc165db36e750907c9a14bb3c0718d58
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 2%

---

# 從您的檔案系統新增檔案至Adobe Workfront

Workfront目前有兩個版本的檔案區域：舊版檔案區域和新檔案區域。 您的組織所使用的版本取決於您的組織是在舊版Workfront儲存空間還是企業儲存空間。 如需這些儲存體型別的詳細資訊，請參閱[Adobe企業儲存體概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

將檔案新增至Workfront會因貴組織使用的檔案區域版本而異。

* [在舊版檔案區域中，從您的檔案系統新增檔案至](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [在新檔案區域將檔案新增到Workfront](#add-documents-to-workfront-in-the-new-documents-area)



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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
   <p>投稿人或以上</p> 
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>舊版Workfront儲存空間：編輯檔案的存取權</p> 
   <p>企業儲存：檔案的編輯存取權預設為啟用，且無法變更</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在舊版檔案區域中，從您的檔案系統新增檔案

如果您的組織位於舊版Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存體的詳細資訊，請參閱[Adobe企業儲存體與舊版Workfront儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage)。

您可以在Adobe Workfront的下列區域中，將檔案新增至專案、任務或問題：

* 全域檔案區域
* Workfront物件的檔案區域
* Workfront展示板上的已連線卡片

您也可以上傳檔案的新版本，並將連結新增至協力廠商雲端廠商（例如Google Drive、Dropbox和Microsoft OneDrive）的檔案。 如需新增檔案新版本的詳細資訊，請參閱[上傳檔案的新版本](../../documents/managing-documents/upload-new-document-version.md)。 如需新增協力廠商雲端廠商檔案的相關資訊，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

您可以上傳至Workfront的檔案型別和大小沒有限制。 不過，為了成功，上傳必須在5分鐘內完成，而且您必須有足夠的可用儲存空間。

如果您需要有關將檔案新版本上傳到Workfront的資訊，請參閱[上傳檔案新版本](../../documents/managing-documents/upload-new-document-version.md)。


### 在舊版檔案區域中新增檔案至Workfront

您可以從工作站的檔案系統新增檔案至Workfront。 您也可以連結來自協力廠商應用程式（例如Google Drive和SharePoint）的檔案。

>[!IMPORTANT]
>
>* 您一次最多可上傳150份檔案。
>* 檔案大小沒有限制。
>* 檔案下載限製為4GB。

若要新增檔案：

1. 前往您要新增檔案的專案、任務或問題。
1. 按一下&#x200B;**檔案**&#x200B;標籤，然後按一下&#x200B;**新增**&#x200B;下拉式功能表。

   ![新增檔案](assets/add-new-doc.png)

1. 根據您要新增的檔案型別，執行下列任一項作業：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">從您工作站上的檔案系統上傳檔案</td> 
      <td> 
       <ol> 
        <li value="1">從<strong>新增</strong>下拉式功能表中，選取<strong>檔案。</strong></li> 
        <li value="2"> <p>瀏覽並選取您要從工作站上的檔案系統新增的檔案。<br></p> <p>當您選取其他檔案時，可以按住Shift鍵來選取多個檔案。</p> </li> 
        <li value="3">按一下<strong>「開啟」</strong>。</li> 
       </ol> 
       <p><b>注意</b>：您也可以直接從檔案管理員將檔案拖放至檔案清單中。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">從第三方應用程式（例如Google Drive或SharePoint）上傳檔案</td> 
      <td> 
       <ol> 
        <li value="1"> <p>從<strong>新增</strong>下拉式功能表中，選取<strong>從&lt;name_of_third-party_application&gt;</strong>。</p> <p>例如，若要從Google磁碟機上傳檔案，請按一下[從Google磁碟機<strong>] </strong>。</p> </li> 
        <li value="2"> <p>按照提示在第三方應用程式中選取檔案。<br></p> <p>如需連結檔案的詳細資訊，請參閱<a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">從外部應用程式連結檔案</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">向其他Workfront使用者請求檔案</td> 
      <td> 
       <ol> 
        <li value="1">從<strong>新增</strong>下拉式功能表中，選取<strong>要求檔案</strong>。</li> 
        <li value="2">在<strong>您是從</strong>向誰請求檔案中，輸入您向其請求檔案的使用者的名稱。</li> 
        <li value="3">在<strong>告訴他們您要求的內容</strong>方塊中，輸入檔案的名稱。</li> 
        <li value="4"> <p>按一下<strong>傳送要求</strong>。</p> <p>您的請求會顯示在「檔案」標籤上。</p> <p>如需有關請求檔案的詳細資訊，請參閱<a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">請求檔案</a>。</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>


## 在新檔案區域將檔案新增到Workfront

您可以使用企業儲存模式將檔案新增至專案、任務或問題。 如需企業儲存的詳細資訊，請參閱[Adobe企業儲存概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

新檔案區域目前不支援的功能：

* 將檔案上傳到全域檔案區域
* 新增來自第三方雲端廠商（例如Google Drive、Dropbox和Microsoft OneDrive）的檔案的連結。
* 請求檔案
* 複製資料夾的連結
* 出庫檔案
* 從剪貼簿貼上影像
* 新增智慧資料夾


### 在新檔案區域將檔案新增到Workfront

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 如需企業儲存的詳細資訊，請參閱[Adobe企業儲存概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

<!--
>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.
-->

若要新增檔案：

1. 前往您要新增檔案的專案、任務或問題。
1. 按一下左側面板中的&#x200B;**檔案**。
1. 按一下頁面右側的&#x200B;**新增**，或將檔案拖放至顯示的拖放區域中。 您可以一次新增多個檔案。

   ![新增檔案](assets/add-new-doc-new-doc.png)

如果您需要有關將檔案新版本上傳到Workfront的資訊，請參閱[上傳檔案新版本](../../documents/managing-documents/upload-new-document-version.md)。

## 企業儲存的檔案安全性

Workfront可透過檔案以下列方式防止病毒和其他惡意內容進入網站：

**Workfront如何偵測損毀的檔案**

使用企業儲存模型會自動啟用物件的檔案掃描。

500 MB以下的檔案上傳時會進行掃描。 不會掃描超過500 MB的檔案。 如果Workfront偵測到損毀的檔案，則會自動將其移除。

**檔案名稱限制**

由於此整合是使用Adobe企業儲存空間建立的，因此在管理專案和檔案時，應注意一些強制的結構與命名慣例。

* 物件名稱必須是唯一的，而且不能重複
* 對於階層樹狀結構中具有相同父級的對等物件，Adobe企業儲存體必須有唯一的名稱
* 如果檔案屬於相同專案，則不能使用相同名稱
* 檔名稱不能包含下列任何特殊字元： `\ / : * ? " | < >`
* 檔名稱上限為255個字元

考慮到這些限制，Workfront會視需要自動重新命名物件或檔案，以避免衝突。


## 舊版Workfront儲存空間的檔案安全性

Workfront網站可透過檔案以下列方式防止病毒和其他惡意內容進入網站：

**Workfront如何偵測損毀的檔案**

您的組織僅在提出請求時才會啟用檔案掃描。

如果已啟用檔案掃描，則會在上傳檔案時掃描25 MB以下的檔案。 不會掃描超過25 MB的檔案。

如果Workfront偵測到檔案損毀，則會出現一則訊息，指出檔案已損毀。 當Workfront偵測到潛在的惡意內容且檔案已設定為要移除時，您也會收到電子郵件通知。

損毀的檔案會在偵測到24小時內移除，除非您手動移除。 如果您刪除損壞的檔案，Workfront會將此動作作為更新加以追蹤。 如果您允許Workfront將其移除，則不會記錄任何更新。

**檔案名稱限制**

上傳至Workfront的檔案無法在檔案名稱中包含某些字元。 如果檔案在檔案名稱中包含下列任何字元，則檔案上傳時這些字元會從檔案名稱中移除： `! # % * \ | ' " / ? < > { } [ ]`。
