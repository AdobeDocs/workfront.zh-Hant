---
product-area: documents
navigation-topic: approvals
title: 一起使用統一核准和校訂
description: 您可以搭配校訂使用統一核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 0%

---

# 一起使用統一核准和校訂

Workfront中的統一核准引進了一組新功能，可幫助您檢閱和核准檔案。 您可以使用具有現有校訂檢視器的「統一核准」工作流程，將註解與標示新增至稽核中的檔案。

一起使用統一核准和校訂時，工作流程有一些主要差異：

* 參與者會顯示在檔案「摘要」中，而非校訂工作流程中。

* 檔案清單中的已傳送、已開啟、註解、決定(SOCD)詳細資料是校訂相關內容，不會反映檔案的決定狀態。

## 上傳檔案並建立校訂

1. 前往您要新增檔案的專案、任務或問題。
1. 按一下&#x200B;**檔案**&#x200B;標籤，然後按一下&#x200B;**新增**&#x200B;下拉式功能表。
或
將檔案拖放到檔案清單中。

   >[!NOTE]
   >
   >如果您在使用者設定檔中啟用&#x200B;**上傳檔案時自動產生校訂**，則系統會自動建立簡易校訂。

1. 將滑鼠停留在檔案上，然後按一下出現在檔名稱下方的&#x200B;**建立校訂**&#x200B;連結，並選取&#x200B;**簡單校訂**。 您需要建立簡單的校訂，因為您將不使用校訂工作流程進行核准。

被指派為參與者的使用者可以使用校訂檢視器在檔案上新增註釋和標示。 繼續下一節以瞭解如何新增稽核參與者。

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## 開啟檔案摘要並指派參與者

依預設，會以基本模式開啟請求核准對話方塊，以進行單階段核准。 切換到進階模式以設定多階段核准或平行路徑。

若要指派參與者，請執行下列動作：

1. 選取您上傳的檔案，並開啟檔案「摘要」。

   ![開啟檔案摘要](assets/open-doc-summary.png)

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。 **要求核准**&#x200B;對話方塊會在基本模式下開啟。

1. 設定核准工作流程。 如需欄位說明、進階模式切換和平行路徑流程，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 按一下&#x200B;**要求核准**。 系統會透過電子郵件通知參與者。

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## 視需要建立新版本

如果您需要另一輪的檢閱和核准，您可以建立新的校訂版本，並新增先前的參與者、新參與者或兩者的組合。 您可以在「摘要」檔案中檢視先前版本和參與者的相關資訊。

依預設，會以基本模式開啟請求核准對話方塊，以進行單階段核准。 切換到進階模式以設定多階段核准或平行路徑。

若要新增版本：

1. 將新檔案拖放到Workfront中的上一個檔案上。 Workfront會自動建立新版本。

1. 檔案上傳完成後，請選取檔案，然後按一下&#x200B;**建立校訂** > **簡單校訂**。

1. 再次選取檔案，然後開啟檔案「摘要」。

   ![開啟檔案摘要](assets/open-doc-summary.png)

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。 **要求核准**&#x200B;對話方塊會在基本模式下開啟。

1. 設定核准工作流程。 如需欄位說明、進階模式切換和平行路徑流程，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

1. 按一下&#x200B;**要求核准**。 系統會透過電子郵件通知參與者。

## 檢閱證明並作出決定

在所有指派的核准者選擇「已核准」之前，檔案不會移動到「已核准」狀態。

若要檢閱及核准檔案，請執行下列動作：

1. 前往檢閱電子郵件通知，然後按一下&#x200B;**前往檢閱**。

1. 進入Workfront後，按一下&#x200B;**前往校訂**。

1. 檢閱內容，並新增任何註解或標示。 如需如何使用校訂檢視器的詳細資訊，請參閱[在Adobe Workfront中檢閱校訂：文章索引](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。

1. 選擇下列其中一項決定：

   * **核准**：檔案不需要變更，且已可供使用。
   * **核准變更**：檔案需要變更，而且一旦完成變更即可使用。 不需要額外核准。
   * **需要工作**：檔案需要變更，而且尚未準備好使用。 完成指定的變更後，檔案必須上傳為新版本，並經過另一輪核准。 如需上傳新版本的詳細資訊，請參閱本文中的[視需要建立新版本](#create-a-new-version-as-needed)。

做出決定後，檔案所有者會透過電子郵件收到通知。