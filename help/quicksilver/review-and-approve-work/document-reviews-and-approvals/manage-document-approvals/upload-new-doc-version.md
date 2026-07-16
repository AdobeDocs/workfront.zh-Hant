---
product-area: documents
navigation-topic: approvals
title: 上傳新檔案版本並請求核准
description: 您可以上傳新檔案版本，並向Adobe Workfront中的其他使用者請求核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 2%

---

# 上傳新檔案版本並請求核准

如果檔案在先前的稽核中被標籤為「需要工作」，您可以將新版本上傳到原始檔案並開始另一輪核准。 上傳檔案的新版本後，先前版本即會鎖定。

如果新版本的檔案名稱與先前版本的檔案名稱不同，則Workfront會顯示具有較新檔案名稱的檔案。

當新版本新增到具有未完成核准的檔案時，先前版本的核准顯示為「已撤回」。 即使部分參與者尚未做出決定，先前的核准流程也會關閉。

如果刪除了最新的檔案版本，先前的版本仍會保持鎖定。 如果您需要編輯先前版本，則必須手動解除鎖定。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存空間管理核准的任何Workfront套件</p>
<p>使用Adobe雲端儲存空間管理核准的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 授權</td> 
   <td> <p>要求或更高版本</p>
   <p>投稿人或以上</p>
   <p>如果您使用Frame.io整合，您必須有Standard授權才能建立核准工作流程。</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>編輯與檔案關聯之物件的存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## 使用拖放功能，在舊版檔案區域中新增新版本

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存體的詳細資訊，請參閱[Adobe雲端儲存體與舊版Workfront儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

>[!NOTE]
>
>Internet Explorer無法使用拖放功能。

如果您需要對檔案執行另一輪稽核和核准，可以在Workfront中建立新的檔案版本。 您可以新增先前的參與者、新參與者或兩者的組合。 您可以在「檔案詳細資訊」頁面上檢視先前版本和參與者的相關資訊。

依預設，會以基本模式開啟請求核准對話方塊，以進行單階段核准。 切換到進階模式以設定多階段核准或平行路徑。

若要新增版本並請求核准：

1. 導覽至Workfront中的檔案。

1. 將新檔案拖放至上一個檔案的頂端。 Workfront會自動建立新版本。

1. 檔案上傳完成後，請選取檔案以開啟檔案摘要面板。 版本編號會顯示在面板頂端。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。 **要求核准**&#x200B;對話方塊會在基本模式下開啟。

1. 設定核准工作流程。 如需欄位說明、進階模式切換和平行路徑流程，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 若要複製上一個檔案版本的相同檢閱者和核准者，請按一下[複製]。**&#x200B;**
1. 按一下&#x200B;**要求核准**。

   核准工作流程隨即開始，核准者會收到新檔案版本需要其核准的通知。 先前檔案版本已鎖定，並撤銷先前版本上的所有未完成核准。

## 使用拖放功能在新的檔案區域中新增新版本

如果您的組織使用Adobe雲端儲存空間，當您存取Workfront中的檔案時，將會看到新的檔案區域。 如需Adobe雲端儲存空間的詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

>[!NOTE]
>
>Internet Explorer無法使用拖放功能。

如果您需要對檔案執行另一輪稽核和核准，可以在Workfront中建立新的檔案版本。 您可以將核准工作流程新增至檔案的新版本。

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

依預設，會以基本模式開啟請求核准對話方塊，以進行單階段核准。 切換到進階模式以設定多階段核准或平行路徑。

若要新增版本並請求核准：

1. 導覽至Workfront中的檔案。

1. 將新檔案拖放至上一個檔案的頂端。 Workfront會自動建立新版本。

1. 檔案上傳完成後，請選取檔案以開啟「摘要」面板。 依預設，會選取檔案的最新版本。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。 **要求核准**&#x200B;對話方塊會在基本模式下開啟。

1. 設定核准工作流程。 如需欄位說明、進階模式切換和平行路徑流程，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 若要複製上一個檔案版本的相同檢閱者和核准者，請按一下[複製]。**&#x200B;**
1. 按一下&#x200B;**要求核准**。

   核准工作流程隨即開始，核准者會收到新檔案版本需要其核准的通知。 先前檔案版本已鎖定，並撤銷先前版本上的所有未完成核准。
