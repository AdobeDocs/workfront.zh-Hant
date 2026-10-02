---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: 在Creative Cloud應用程式中使用Workfront檔案
description: 從Photoshop、Illustrator和InDesign開啟、編輯和儲存Workfront檔案，並請求核准。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: deeb63ceccc28b8f376713d4a6fb6c103ab4e06b
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 4%
---
# 在Creative Cloud應用程式中使用Workfront檔案

在Workfront專案面板中提供Creative Cloud專案後，您可以直接從Photoshop、Illustrator或InDesign處理其檔案。

## 先決條件

* 您的組織必須採用支援Adobe雲端儲存空間的Workfront版本。
* Workfront與Photoshop、Illustrator或InDesign必須有權使用同一個Adobe Identity Management System (IMS)組織。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront版本</td> 
   <td>工作流程Ultimate，已啟用Adobe雲端儲存空間</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>
      <p>檢視專案的存取權，以便在Creative Cloud專案面板中檢視</p>
      <p>編輯專案的存取權以新增、編輯或刪除專案</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 存取Workfront專案

Workfront專案中的「檔案」資料夾結構會反映在「專案」面板中。 當您從專案資料夾開啟檔案、編輯該檔案並儲存時，您的變更會出現在Workfront中。

>[!NOTE]
>
>專案面板不支援舊版Workfront儲存專案：僅限Adobe雲端儲存專案。


若要存取Photoshop、Illustrator或InDesign中的Workfront專案：

1. 開啟Photoshop、Illustrator或InDesign。
1. 在應用程式左側的&#x200B;**專案**&#x200B;面板中，選取您要開啟的Workfront專案。

   ![列於專案面板中的Workfront專案](assets/cc-projects.png)

1. 開啟專案中的檔案以進行編輯。 儲存變更後，它們會自動儲存回Workfront專案。


>[!TIP]
>
>若要編輯Photoshop、Illustrator或InDesign無法開啟的檔案型別，例如Word或Excel檔案，請改用Adobe Cloud Drive。 如需詳細資訊，請參閱[Adobe Cloud Drive總覽](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)。

## 請求對檔案的核准

您可以在Workfront中新增檔案核准，新增至您從Photoshop、Illustrator、InDesign或Adobe Cloud Drive上傳的任何檔案，就像任何其他檔案一樣。 如需詳細資訊，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

<!--
need to verify
Creating an approval on a Creative Cloud document also creates a new version of the document. For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md#view-the-current-file-during-an-approval).
-->