---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 移除Adobe Workfront和外部檔案儲存提供者之間的連結
description: 第一次從任何服務上傳檔案時，Adobe Workfront會向使用者要求存取其檔案服務的許可權。 當使用者提供他們的檔案服務憑證以登入時，檔案服務會將其自身連結到Workfront。
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 4%

---

# 移除Adobe Workfront和外部檔案儲存提供者之間的連結

第一次從任何服務上傳檔案時，Adobe Workfront會向使用者要求存取其檔案服務的許可權。 當使用者提供他們的檔案服務憑證以登入時，檔案服務會將其自身連結到Workfront。

如需將外部檔案服務連結至Workfront的相關資訊，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

由於檔案服務是允許連結至Workfront的許可權，Workfront無法移除檔案服務授與的許可權。 您必須從檔案服務應用程式內移除許可權，或者您必須致電我們的支援團隊，以從我們的伺服器移除此連結。

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
   <p>投稿人或以上</p>
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 移除Workfront與Dropbox之間的連結

1. 登入Dropbox。
1. 按一下右上角的個人資料圖片，然後按一下&#x200B;**設定**。
1. 按一下&#x200B;**連線的應用程式**&#x200B;標籤，然後向下捲動至&#x200B;**連結的應用程式**。

1. 按一下Workfront旁的&#x200B;**X**。

## 移除Workfront與Box之間的連結

1. 登入您的Box帳戶。
1. Click your profile picture in the upper right corner.
1. Click **Account Settings**, then the **Security** tab.

1. Find **MyWorkfront** and click the **X** under Forget App.

## Remove the link between Workfront and Google Drive

1. Log in to your Google Drive.
1. Click the gear icon in the upper right corner, then click **Settings**.
1. Click **Manage Apps** on the left side and find **Workfront** in the list.

1. Under the Options drop-down menu, click **Disconnect from Drive**.

## Remove the links between Workfront and Other Document Storage Providers

You must call our Support Team to disconnect Microsoft One Drive or WebDAM from Workfront.

For information about contacting our Support Team, see [Contact Customer Support](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
