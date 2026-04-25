---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: 檔案摘要概覽
description: The Summary allows you to interact with important information directly from the documents list.
author: Courtney
feature: Digital Content and Documents
exl-id: 7a4a4bd3-ad60-4d84-b4b0-332c2a4eb8fb
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 5%

---

# 檔案摘要概覽

<!--Audited: April, 2024-->

You can use the Summary panel to access and update important information directly from the documents list.


+++ 展開以檢視這篇文章中所述功能的存取權要求。


## 存取權要求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存來管理檔案的任何Workfront套件</p>
<p>使用Adobe企業儲存體管理檔案的任何Workflow套件</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 授權</td> 
   <td> <p>投稿人或以上</p> 
   <p>要求或更高版本</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p>  </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>View access to the object associated with the document</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Summary for documents in the legacy documents experience

如果您的組織位於舊版Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需有關舊版Workfront儲存體的詳細資訊，請參閱[舊版Workfront儲存體與Adobe企業儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md)。

### Open the Summary view in the legacy documents experience

{{step1-to-documents}}

1. 在&#x200B;**檔案**&#x200B;頁面上，選取清單中的檔案。

1. 在頁面的右上角，按一下&#x200B;**開啟摘要**&#x200B;圖示![開啟摘要圖示](assets/qs-summary-in-new-toolbar-small.png)。 The **Document Summary** side panel opens.

   ![Summary details](assets/document-summary-panel.png)

   After you open the Summary, it will remain open on this page (even if you click on other documents) until you manually close it.


### 詳細資料

Use the Details section to view high-level overview information and interact with custom forms. Click Details at the top of the section to go to the full Document Details page.

* [概觀](#overview)
* [自訂表單](#custom-forms)

#### 概觀 {#overview}

Expand the Overview section to view or download an image thumbnail, open a proof, update the basic description, check the document out and more.

![Document summary overview](assets/details-section.png)

#### 自訂表單 {#custom-forms}

Use the Custom Forms section to add, edit, or view any custom forms associated with the document. Begin typing the name of the custom form to add it to the document. For more information, see [Add or edit a custom form to a document](../../documents/managing-documents/add-custom-form-documents.md).

![Add a custom form in document summary](assets/custom-forms-section.png)

### 更新

Use the Updates section to view an update someone made on the document or proof. The summary shows the first 2 comments made. For more information on updates, see [Comment on a proof](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md).

![Updates section in Summary panel](assets/updates-section.png)

### 核准

Use the Approvals section to ask for a document approval. You can also remind someone about an approval, resubmit the approval and cancel the previous decision, or delete the approval. Document approvers can use the Summary to make a decision.

Proof approvals must be added in the Proof Workflow. For more information on approvals, see

* [Approving work](../../review-and-approve-work/manage-approvals/approving-work.md)
* [請求文件核准](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

![Document summary approvals](assets/approvals-section.png)

### 版本

Use the Versions section to view the number of versions created for a specific document. Click the More icon ![More icon](assets/more-icon.png) to do the following:

* Open a proof.
* Download a proof or document.
* Preview a browser-supported document.
* Go to the Document Details.
* Delete a proof or document.

![Document summary versions](assets/versions-section.png)

## 新檔案體驗中的檔案摘要

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 如需企業儲存的詳細資訊，請參閱[Adobe企業儲存概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

### 詳細資料

使用詳細資訊區段檢視高階總覽資訊並與自訂表單互動。

![新檔案中的檔案摘要詳細資訊](assets/summary-details.png)

### 核准

使用核准區段來建立核准工作流程。 您也可以提醒參與者核准或刪除核准。 檔案核准者可以存取Frame.io檢視器或使用「摘要」做出決定。

如需有關核准和Frame.io的詳細資訊，請參閱

* [開始使用統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [建立檔案檢閱或核准要求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

![新檔案中的檔案摘要核准](assets/summary-approvals.png)


<!-- resubmit the approval and cancel the previous decision, or delete the approval. Document approvers can use the Summary to make a decision.-->


### 版本

使用「版本」區段可檢視針對特定檔案建立的版本數目。 按一下「更多」圖示以執行下列動作：

* 重新命名版本
* 檢視檔案詳細資訊
* 請求核准特定版本
* 在 Frame.io 中開啟
* 下載版本
* 共用版本
* 刪除版本

![新檔案中的檔案摘要版本體驗](assets/summary-versions.png)

### 歷史記錄

使用「歷史記錄」區段可檢視與檔案相關的所有活動清單。

![新檔案中的檔案摘要歷程記錄體驗](assets/summary-history.png)