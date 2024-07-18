---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 移除Adobe Workfront和外部檔案儲存提供者之間的連結
description: 第一次從任何服務上傳檔案時，Adobe Workfront會向使用者要求存取其檔案服務的許可權。 當使用者提供他們的檔案服務憑證以登入時，檔案服務會將其自身連結到Workfront。
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 移除Adobe Workfront和外部檔案儲存提供者之間的連結

第一次從任何服務上傳檔案時，Adobe Workfront會向使用者要求存取其檔案服務的許可權。 當使用者提供他們的檔案服務憑證以登入時，檔案服務會將其自身連結到Workfront。

如需將外部檔案服務連結至Workfront的相關資訊，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

由於檔案服務是允許連結至Workfront的許可權，Workfront無法移除檔案服務授與的許可權。 您必須從檔案服務應用程式內移除許可權，或者您必須致電我們的支援團隊，以從我們的伺服器移除此連結。

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 移除Workfront與Dropbox之間的連結

1. 登入Dropbox。
1. 按一下右上角的個人資料圖片，然後按一下&#x200B;**設定**。
1. 按一下&#x200B;**連線的應用程式**&#x200B;標籤，然後向下捲動至&#x200B;**連結的應用程式**。

1. 按一下Workfront旁的&#x200B;**X**。

## 移除Workfront與Box之間的連結

1. 登入您的Box帳戶。
1. 按一下右上角的設定檔圖片。
1. 按一下「**帳戶設定**」，然後按一下「**安全性**」標籤。

1. 尋找&#x200B;**MyWorkfront**&#x200B;並按一下「忘記應用程式」底下的&#x200B;**X**。

## 移除Workfront與Google Drive之間的連結

1. 登入您的Google Drive。
1. 按一下右上角的齒輪圖示，然後按一下&#x200B;**設定**。
1. 按一下左側的&#x200B;**管理應用程式**，然後在清單中尋找&#x200B;**Workfront**。

1. 在[選項]下拉式功能表下，按一下[中斷與磁碟機的連線]。****

## 移除Workfront與其他檔案儲存提供者之間的連結

您必須致電我們的支援團隊，中斷與Workfront的Microsoft One Drive或WebDAM連線。

如需連絡支援團隊的詳細資訊，請參閱[連絡客戶支援](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。
