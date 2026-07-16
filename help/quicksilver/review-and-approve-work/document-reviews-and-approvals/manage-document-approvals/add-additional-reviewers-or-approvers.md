---
product-area: documents
navigation-topic: approvals
title: 新增其他核准者或稽核者至檔案核准工作流程
description: 您可以將其他核准者或稽核者新增至已有待核准的檔案。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
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
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 2%

---

# 新增其他核准者或稽核者至檔案核准工作流程

您可以將其他核准者或稽核者新增至已有待核准的檔案核准工作流程。

>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准程式的資訊，請參閱[工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存空間管理核准的任何Workfront套件</p>
<p>使用Adobe雲端儲存空間管理核准的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>投稿人或以上</p>
   <p>評論或以上</p> 
   <p>如果您使用Frame.io整合，您必須有Standard授權才能建立核准工作流程。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案、任務、問題、範本、投資組合、計畫、報告、儀表板、行事曆和檔案的或更高存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視或更高的存取許可權以存取與要求存取或核准相關聯的物件 </p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++



<!--
## Add additional approvers or reviewers in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document will open.

1. Select the version of the document you would like to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**.

   ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## 在舊版檔案區域中新增其他核准者或稽核者

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存體的詳細資訊，請參閱[Adobe雲端儲存體與舊版Workfront儲存體之間的差異](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

若要從「檔案摘要」新增其他核准者或稽核者：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案。 隨即開啟該檔案的檔案摘要面板。

1. 在版本下拉式選單中，選取您要新增核准者或稽核者的檔案版本。 預設會選取最新版本。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**編輯工作流程**。 「請求核准」對話方塊會以上次儲存核准的模式開啟：「基本」用於單階段核准，或「進階」用於具有平行路徑的多階段核准和核准。

1. 新增使用者、團隊或電子郵件：

   * 在[基本]模式中，在&#x200B;**新增名稱或電子郵件**&#x200B;欄位中輸入名稱或電子郵件。
   * 在[進階]模式中，選取包含您要更新的階段的路徑，然後在階段的&#x200B;**新增名稱或電子郵件**&#x200B;欄位中輸入名稱或電子郵件。

1. 對於您新增的每個人，選擇他們是要核准者還是檢閱者。

   ![核准者或檢閱者下拉式清單](assets/choose-reviewer-or-approver.png)

1. 按一下「**儲存**」。 您新增的參與者會收到電子郵件通知，告知檔案需要其核准或稽核。

>[!TIP]
>
>若要將基本模式核准重新建構為多階段或多路徑核准，請按一下右上角的&#x200B;**移至進階**。 您現有的參與者會保留為路徑1，階段1。 儲存後，無法切換回基本模式。 如需詳細資訊，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

<!--
## Add additional approvers or reviewers in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. Click **Edit workflow**.

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## 從新檔案區域中的檔案摘要新增其他核准者或稽核者

如果您的組織使用Adobe雲端儲存空間，當您存取Workfront中的檔案時，將會看到新的檔案區域。 如需Adobe雲端儲存空間的詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

若要從「檔案摘要」新增其他核准者或稽核者：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下檔案，然後按一下頁面右側的&#x200B;**核准**&#x200B;圖示。

   ![在檔案摘要中新增核准者](assets/approvals-icon-new.png)

1. 按一下&#x200B;**編輯工作流程**。 「請求核准」對話方塊會以上次儲存核准的模式開啟：「基本」用於單階段核准，或「進階」用於具有平行路徑的多階段核准和核准。

1. 新增使用者、團隊或電子郵件：

   * 在[基本]模式中，在&#x200B;**新增名稱或電子郵件**&#x200B;欄位中輸入名稱或電子郵件。
   * 在[進階]模式中，選取包含您要更新的階段的路徑，然後在階段的&#x200B;**新增名稱或電子郵件**&#x200B;欄位中輸入名稱或電子郵件。

1. 對於您新增的每個人，選擇他們是要核准者還是檢閱者。

   ![核准者或檢閱者下拉式清單](assets/choose-reviewer-or-approver.png)

1. 按一下「**儲存**」。 您新增的參與者會收到電子郵件通知，告知檔案需要其核准或稽核。

>[!TIP]
>
>若要將基本模式核准重新建構為多階段或多路徑核准，請按一下右上角的&#x200B;**移至進階**。 您現有的參與者會保留為路徑1，階段1。 儲存後，無法切換回基本模式。 如需詳細資訊，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。
