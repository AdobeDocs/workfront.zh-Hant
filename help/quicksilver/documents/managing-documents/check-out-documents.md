---
product-area: documents
navigation-topic: manage-documents
title: 簽出文檔
description: 您可以簽出文檔，以防止其他用戶刪除文檔或上傳新版本。 一次只能有一個用戶可以簽出文檔。 您可以勾選上傳至Adobe Workfront的任何檔案，以及連結至協力廠商檔案提供者(方塊、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自訂提供者)的檔案。
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 簽出文檔

您可以簽出文檔，以防止其他用戶刪除文檔或上傳新版本。 一次只能有一個用戶可以簽出文檔。 您可以勾選上傳至Adobe Workfront的任何檔案，以及連結至協力廠商檔案提供者(方塊、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自訂提供者)的檔案。 

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
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 對已簽出文檔允許的操作

對文檔具有管理訪問權限的用戶可以執行以下操作：

* 編輯文檔（文檔名稱、說明、自定義資料）
* 移動文檔
* 共用檔案
* 預覽文檔
* 下載檔案

   >[!TIP]
   >
   > 雖然用戶可以在另一個用戶簽出文檔時下載該文檔，但我們建議用戶等待文檔重新簽入後再下載。 簽出文檔時，通常表示文檔上仍在執行工作。 等到檔案簽回後再下載，即可確保使用者擁有最新版本。

* 批准文檔或將批准應用於文檔。
* 在校對查看器中查看文檔

   有關校對的詳細資訊，請參見 [校對](../../review-and-approve-work/proofing/proofing.md)

## 簽出文檔

如果您對文檔具有管理權限，則可將其簽出以禁止對文檔執行某些操作。 

1. 轉到儲存文檔的區域，然後選擇文檔。 

   有關添加文檔的資訊，請參閱 [從您的檔案系統將檔案新增至Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. 按一下 **結帳** 圖示 ![](assets/check-out-25x23.png).

1. 鎖表徵圖 ![](assets/lock-icon-locked-qs.png) 顯示在文檔名稱的右側。 登出Workfront後，檔案會保持簽出狀態。
1. 只有簽出文檔的用戶或Workfront管理員才能簽入文檔。

## 管理已簽出文檔

請考慮以下有關已簽出文檔的資訊：

* 在可以刪除儲存已簽出文檔的對象之前，必須先將文檔簽回。 
* 如果Workfront管理員刪除了簽出他們不擁有的文檔的用戶，則Workfront會自動簽入該文檔。
* 如果Workfront管理員刪除了簽出其擁有的文檔的用戶，並且該文檔上載到對象上，則文檔將保持簽出狀態。 只有Workfront管理員可以重新登入。
* 如果Workfront管理員刪除了簽出其擁有的文檔的用戶，並且該文檔僅在「文檔」區域（而不是對象上）中上載，則該文檔將與用戶一起刪除。

   如需刪除使用者的相關資訊，請參閱 [刪除使用者](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* 如果Workfront管理員停用了使用者，則他們已簽出的任何檔案都會保持簽出狀態。 只有Workfront管理員可以重新登入。 

## 簽入文檔

您必須先簽回檔案，才能上傳新版本或將其刪除。 

要簽入文檔，請執行以下操作：

1. 轉到儲存文檔的區域，然後選擇文檔。 

   鎖表徵圖 ![](assets/lock-icon-locked-qs.png) 顯示在文檔名稱的右側。

1. 按一下 **簽入** 圖示 ![](assets/check-in-25x22.png).
