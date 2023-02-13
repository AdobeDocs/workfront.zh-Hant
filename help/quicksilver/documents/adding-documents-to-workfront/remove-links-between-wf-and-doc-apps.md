---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 移除Adobe Workfront和外部檔案儲存提供者之間的連結
description: 首次從任何服務上傳檔案時，Adobe Workfront會向使用者要求存取其檔案服務的權限。 當使用者提供其檔案服務憑證以登入時，檔案服務會連結至Workfront。
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 移除Adobe Workfront和外部檔案儲存提供者之間的連結

首次從任何服務上傳檔案時，Adobe Workfront會向使用者要求存取其檔案服務的權限。 當使用者提供其檔案服務憑證以登入時，檔案服務會連結至Workfront。

如需將外部檔案服務連結至Workfront的詳細資訊，請參閱 [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

由於檔案服務是允許連結至Workfront的服務，因此Workfront無法移除檔案服務所授予的權限。 您必須從文檔服務應用程式中刪除該權限，或者必須致電我們的支援團隊從我們的伺服器中刪除此連結。

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

## 移除Workfront與Dropbox之間的連結

1. 登入Dropbox。
1. 按一下右上角的個人資料圖片，然後按一下 **設定**.
1. 按一下 **連接的應用** 標籤，然後向下捲動至 **連結的應用程式**.

1. 按一下 **X** 在Workfront旁邊。

## 移除Workfront與Box之間的連結

1. 登入您的Box帳戶。
1. 按一下右上角的個人資料圖片。
1. 按一下 **帳戶設定**，則 **安全性** 標籤。

1. 查找 **MyWorkfront** 並按一下 **X** 在「忘記應用程式」下。

## 移除Workfront和Google驅動器之間的連結

1. 登入Google Drive。
1. 按一下右上角的齒輪圖示，然後按一下 **設定**.
1. 按一下 **管理應用程式** 在左側，找到 **Workfront** 在清單中。

1. 在「選項」下拉式功能表下，按一下 **從驅動器斷開連接**.

## 移除Workfront和其他檔案儲存提供者之間的連結

您必須致電支援團隊，將Microsoft One Drive或WebDAM與Workfront斷開連接。

如需聯絡支援團隊的相關資訊，請參閱 [聯絡客戶支援](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
