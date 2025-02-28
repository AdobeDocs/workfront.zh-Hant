---
product-area: documents
navigation-topic: manage-documents
title: 簽出檔案
description: 您可以出庫檔案，以防止其他使用者刪除檔案或上傳檔案的新版本。 一次只能有一個使用者出庫檔案。 您可以簽出已上傳至Adobe Workfront的任何檔案，以及連結至協力廠商檔案提供者(Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自訂提供者)的檔案。
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---

# 簽出檔案

您可以出庫檔案，以防止其他使用者刪除檔案或上傳檔案的新版本。 一次只能有一個使用者出庫檔案。 您可以簽出已上傳至Adobe Workfront的任何檔案，以及連結至協力廠商檔案提供者(Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自訂提供者)的檔案。 

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理對檔案的存取</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 已取出檔案允許的動作

具有檔案管理存取許可權的使用者可以執行以下操作：

* 編輯檔案（檔名稱、說明、自訂資料）
* 移動檔案
* 共用檔案
* 預覽檔案
* 下載檔案

  >[!TIP]
  >
  > 雖然使用者可以在檔案由其他使用者出庫時下載檔案，但我們建議使用者等到檔案已入庫後再下載。 當檔案出庫時，它通常表示檔案上的工作仍在進行中。 等到檔案簽入後再下載，可確保使用者擁有最新版本。

* 核准檔案或套用核准至檔案。
* 在校訂檢視器中檢閱檔案

  如需校訂的詳細資訊，請參閱[校訂](../../review-and-approve-work/proofing/proofing.md)

## 將檔案出庫

如果您擁有檔案的管理許可權，則可以將其出庫以禁止對檔案執行某些動作。 

1. 移至儲存檔案的區域，然後選取檔案。 

   如需新增檔案的詳細資訊，請參閱[從您的檔案系統新增檔案至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)。

1. 按一下&#x200B;**簽出**&#x200B;圖示![簽出圖示](assets/check-out-25x23.png)。

1. 鎖定圖示![鎖定圖示](assets/lock-icon-locked-qs.png)會顯示在檔名稱的右側。 在您登出Workfront後，檔案會保持出庫狀態。
1. 只有出庫檔案的使用者或Workfront管理員才能將檔案入庫。

## 管理已取出檔案

關於出庫的檔案，請考慮下列事項：

* 您必須先將檔案入庫，才能刪除儲存出庫檔案的物件。 
* 如果Workfront管理員刪除已簽出非其擁有之檔案的使用者，Workfront會自動簽入該檔案。
* 如果Workfront管理員刪除出庫其所擁有檔案的使用者，且檔案已上傳至物件上，則檔案仍會保持出庫狀態。 只有Workfront管理員可以將其重新簽入。
* 如果Workfront管理員刪除出庫其擁有檔案的使用者，且檔案僅在「檔案」區域（而非物件）上傳，則會刪除該使用者的檔案。

  如需有關刪除使用者的資訊，請參閱[刪除使用者](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)。

* 如果Workfront管理員停用使用者，則他們已出庫的任何檔案都會保持出庫狀態。 只有Workfront管理員可以重新簽入。 

## 將檔案簽入

您必須先將檔案簽回，然後才能上傳新版本或刪除它。 

若要入庫檔案，請執行下列動作：

1. 移至儲存檔案的區域，然後選取檔案。 

   鎖定圖示![鎖定圖示](assets/lock-icon-locked-qs.png)會顯示在檔名稱的右側。

1. 按一下&#x200B;**簽入**&#x200B;圖示![簽入圖示](assets/check-in-25x22.png)。
