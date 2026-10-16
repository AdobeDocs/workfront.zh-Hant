---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 將網頁連結新增為檔案
description: 您可以將網站新增至Adobe Workfront做為網頁連結，並申請核准。
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 85f0798c7956369e7b3c92a6c777414fa81511b6
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 4%
---
# 將網頁連結新增為檔案

您可以從新的檔案區域將網站新增至Adobe Workfront，作為網頁連結。 新增後，您可以透過請求核准上傳檔案的方式，在即時網頁上請求核准。

如果您的組織使用Adobe雲端儲存空間，當您存取Workfront中的檔案時，將會看到新的檔案區域。 如需Adobe雲端儲存空間的詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存來管理檔案的任何Workfront套件</p>
<p>使用Adobe雲端儲存空間管理檔案的任何Workflow套件</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 授權</td> 
   <td> 
   <p>投稿人或以上</p> 
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>舊版Workfront儲存空間：編輯檔案的存取權</p> 
   <p>Adobe雲端儲存空間：檔案的編輯存取權預設為啟用，無法變更</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將網頁連結新增為檔案

您可以將HTML網頁以網頁連結的形式上傳至Workfront。 新增後，您可以透過請求核准上傳檔案的方式，在即時網頁上請求核准。 如需Frame.io如何處理網頁連結的詳細資訊，請參閱[HTML的Frame.io檢閱](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links)。


>[!IMPORTANT]
>
>* 如果網站允許iFrame內嵌，則支援URL。
>* 支援私用Web URL，但某些驗證流程可能無法運作，端視伺服器設定而定。
>* 目前不支援Youtube和圖片URL。<br>
>如需詳細資訊，請參閱[ Frame.io](https://help.frame.io/en/articles/12893213-html-review-for-frame-io#:~:text=of%20the%20page.-,What%20types%20of%20URLs%20are%20supported%3F,-URLs%20are%20supported)支援的URL型別。


若要新增網頁連結：

1. 前往您要新增網站的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。
1. 按一下&#x200B;**新增**，然後選取&#x200B;**網頁連結**。
1. 在&#x200B;**檔名稱**&#x200B;欄位中輸入名稱，然後在&#x200B;**URL**&#x200B;欄位中輸入網站位址。
1. 按一下&#x200B;**新增**。
   ![將網頁連結新增為檔案](assets/web-url.png)

若要在網頁連結上要求核准，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

## 已知限制

* 在Frame.io中建立的網頁連結檔案發生暫時性問題。 如果您在Frame.io中建立網頁連結，然後在Workfront中對其建立核准，則檔案不會在Frame.io中開啟。 在Workfront中建立的網頁連結不受影響。 在此問題解決之前，請先在Workfront中建立網頁連結檔案，然後再開始核准。
* 您目前無法在Frame.io中建立網頁連結檔案的新版本。 如果您需要建立新版本的網頁連結檔案，請在Workfront中建立新版本。