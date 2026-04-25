---
product-area: documents
navigation-topic: approvals
title: 從檔案核准工作流程中移除核准者或稽核者
description: 您可以從檔案中移除個別核准者或稽核者。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 3%

---

# 從檔案核准工作流程中移除核准者或稽核者

在指派核准者或稽核者後，您可以從資產或檔案中移除個別核准者或稽核者。

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
<p>使用Adobe企業儲存體管理核准的任何Workflow套件</p>  </td> 
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
   <td> <p>檢視專案、任務、問題、範本、投資組合、計畫、報告、儀表板和行事曆、檔案的或更高存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理與請求存取或核准相關聯的物件存取權 </p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 從舊版檔案區域的核准工作流程中移除核准者或稽核者

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存的詳細資訊，請參閱[Workfront儲存與Adobe企業儲存的比較](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)。

若要從核准工作流程中移除核准者或稽核者：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 向下捲動至檔案摘要面板中的&#x200B;**核准**&#x200B;區段。

1. 按一下&#x200B;**編輯工作流程**。

1. Locate the participant you want to remove, then click the **Remove** icon next to their name.

   The approval or review request is removed and the approver receives a notification that their approval is no longer needed. Their approval-related share access is also removed.

   ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. (Optional) To change the role of an approver to a reviewer, or vice versa, click the drop-down menu next to the username, and select the new role.

1. Repeat the previous step to remove any additional approvers or reviewers.

</div>


## Remove approvers or reviewers to an approval workflow in the new document area

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 For more information about enterprise storage, see [Enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create a an approval workflow:

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. 按一下&#x200B;**編輯工作流程**。

1. Locate the participant you want to remove, then click the **Remove** icon next to their name.

   The approval or review request is removed and the approver receives a notification that their approval is no longer needed.

1. (Optional) To change the role of an approver to a reviewer, or vice versa, click the drop-down menu next to the username, and select the new role.

1. Repeat the previous step to remove any additional approvers or reviewers.

   ![remove participants from a stage](assets/add-or-remove-participants.png)

1. 按一下「**儲存**」。