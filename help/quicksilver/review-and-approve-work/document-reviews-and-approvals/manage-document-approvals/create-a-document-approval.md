---
product-area: documents
navigation-topic: approvals
title: Create a document approval workflow
description: You can request approval from other users for a document in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 3%

---

# Create a document approval workflow

You can request approval from other users or teams for a document in Adobe Workfront, or request they review a document without needing to approve it.

>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准程式的資訊，請參閱[工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>使用舊版Workfront儲存空間管理核准的任何Workfront套件</p>
<p>使用Adobe企業儲存體管理核准的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td>  
   <td>
   <p>投稿人或以上</p>
   <p>評論或以上</p>
   <p>If you are using the Frame.io integration, you must have a Standard license to create approval workflows.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, Templates, Portfolios, Programs, Reports, Dashboards, and Calendars, Documents</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>Manage access to the object associated with the request access or approval </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Create an approval workflow from the Summary panel in the legacy documents area

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Workfront Storage vs. Adobe enterprise storage](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

To create an approval workflow:

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. Click on the document you need and the Document Summary panel for that document opens.

1. Select the version of the document you would like to create an approval for in the version dropdown. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. 填寫以下詳細資料：

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>新增階段名稱。 您可以將名稱變更為描述性更強的名稱，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>需要一項決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。

   ![檔案詳細資料](assets/new-stage.png)


## Create an approval workflow from the Summary panel in the new document area

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 For more information about enterprise storage, see [Enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create a an approval workflow:

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. Click on the document, then click the Approvals icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>階段名稱</strong></td>
   <td>新增階段名稱。 您可以將名稱變更為描述性更強的名稱，例如<em>初始稽核</em>或<em>最終核准</em>。</td>
   </tr>
   <tr>
   <td><strong>新增姓名或電子郵件</strong></td>
   <td>開始輸入使用者或團隊名稱，以新增為核准者或稽核者。 如果您只有稽核者，他們將會收到通知並可以選擇完成稽核，但不需要或做出任何決定。</td>
   </tr>
   <tr>
   <td><strong>需要一項決定（選擇性）</strong></td>
   <td>第一個做出決定的人會完成階段。</td>
   </tr>
   <tr>
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。

   ![檔案詳細資料](assets/new-stage.png)



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
