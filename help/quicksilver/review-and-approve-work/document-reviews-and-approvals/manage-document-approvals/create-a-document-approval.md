---
product-area: documents
navigation-topic: approvals
title: 建立檔案稽核或核准請求
description: 您可以在Adobe Workfront中請求其他使用者的檔案核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: 6daf68aee442b3322d186e649e7797cc2e911145
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 建立檔案稽核或核准請求

您可以在Adobe Workfront中請求其他使用者或團隊核准檔案，或請求他們稽核檔案而無需核准。

>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准流程的資訊，請參閱下列文章： [工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視專案、任務、問題、範本、Portfolio、方案、報告、儀表板和行事曆、檔案的或更高存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理與請求存取或核准相關聯的物件存取權 </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 從檔案頁面建立檔案檢閱或核准請求

1. 將滑鼠停留在檔案上，然後按一下「檔案詳細資訊」。
   ![](assets/doc-details.png)


1. 在檔名稱附近，在版本下拉式清單中選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 按一下 **核准** 在左窗格中。

1. （選用）設定核准的截止日期。 若在指定期限前72小時通知使用者和團隊。

1. 若要新增核准者，請按一下 **核准者** 並開始輸入使用者或團隊名稱。

1. 若要新增稽核者，請按一下 **檢閱者** 核取方塊，並開始輸入使用者或團隊名稱。

   ![](assets/add-approver-and-deadline.png)

1. 重複上一步驟以新增其他核准者或稽核者。

## 從「檔案摘要」窗格建立檔案稽核或核准請求

1. 前往包含檔案的專案、任務或問題，然後選取「 」 **檔案**.

1. 按一下您需要的檔案，將會開啟該檔案的[檔案摘要]窗格。

1. 在版本下拉式清單中選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 向下捲動至 **核准** 區段，然後按一下 **新增**.

![](assets/doc-summary-add-approvers.png)

1. （選用）設定核准的截止日期。 若在指定期限前72小時通知使用者和團隊。

1. 若要新增核准者，請按一下 **核准者** 並開始輸入使用者或團隊名稱。

1. 若要新增稽核者，請按一下 **檢閱者** 核取方塊，並開始輸入使用者或團隊名稱。

   ![](assets/add-approver-and-deadline.png)

1. 重複上一步驟以新增其他核准者或稽核者。

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)
-->
