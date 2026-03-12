---
product-area: documents
navigation-topic: approvals
title: 新增其他核准者或稽核者至檔案核准工作流程
description: 您可以將其他核准者或稽核者新增至已有待核准的檔案。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 2%

---

# 新增其他核准者或稽核者至檔案核准工作流程

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

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
   <td> <p>任何</p> </td> 
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


## 從生產環境的「檔案詳細資訊」頁面新增其他核准者或稽核者

1. 按一下檔名稱，移至檔案頁面，然後在版本下拉式選單中選取您要新增核准者或稽核者的檔案版本。 預設會選取最新版本。

1. 在左側面板中選取&#x200B;**核准**。 此處列出所有現有核准者和稽核者。

1. 若要新增核准者，請確定已核取&#x200B;**核准者**&#x200B;核取方塊，然後開始輸入&#x200B;**檢閱者**&#x200B;文字方塊。 您可以依名稱新增Workfront使用者或團隊。 如果您要新增檢閱者，只需取消勾選&#x200B;**核准者**&#x200B;核取方塊，再輸入即可。

1. 重複上一步驟以新增其他核准者或稽核者。

## 從您生產環境中的「檔案摘要」，新增其他核准者或稽核者

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。

1. 按一下您需要的檔案，檔案摘要面板隨即開啟。

1. 在版本下拉式選單中，選取您想要新增核准者或稽核者的檔案版本。 預設會選取最新版本。

1. 向下捲動至「檔案摘要」面板中的&#x200B;**核准**&#x200B;區段，其中列出所有現有的核准者和稽核者。 若要新增核准者，請確定已核取&#x200B;**核准者**&#x200B;核取方塊，然後開始輸入&#x200B;**檢閱者**&#x200B;文字方塊。 您可以依名稱新增Workfront使用者或團隊。 如果您要新增檢閱者，只需取消勾選&#x200B;**核准者**&#x200B;核取方塊，再輸入即可。

1. 重複上一步驟以新增其他核准者或稽核者。

<div class="preview">

## 在舊版檔案區域的預覽環境中，從檔案摘要新增其他核准者或稽核者

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存的詳細資訊，請參閱[Workfront儲存與Adobe企業儲存的比較](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)。

若要從「檔案摘要」新增其他核准者或稽核者：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板將會開啟。

1. 在版本下拉式選單中，選取您想要新增核准者或稽核者的檔案版本。 預設會選取最新版本。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**編輯工作流程**。

   ![編輯核准工作流程](assets/edit-approval-in-legacy.png)

1. 找到您要新增核准者或稽核者的階段，然後在文字方塊中新增使用者名稱或電子郵件。 如有需要，您也可以新增整個團隊。

1. 在新增其名稱后，選擇其為核准者或稽核者。

   ![核准者或檢閱者下拉式清單](assets/choose-approver-or-reviewer.png)

1. 重複步驟5至6以新增其他核准者或稽核者。
儲存之後，新增的參與者會收到電子郵件通知，告知檔案需要其核准或稽核。

</div>


## 從新檔案區域中的檔案摘要新增其他核准者或稽核者

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 如需企業儲存的詳細資訊，請參閱[企業儲存概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。


1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下檔案，然後按一下頁面右側的&#x200B;**核准**&#x200B;圖示。

   ![在檔案摘要中新增核准者](assets/approvals-icon-new.png)


1. 按一下&#x200B;**編輯工作流程**。

1. 找到您要新增核准者或稽核者的階段，然後在文字方塊中新增使用者名稱或電子郵件。 如有需要，您也可以新增整個團隊。

1. 在新增其名稱后，選擇其為核准者或稽核者。

   ![核准者或檢閱者下拉式清單](assets/choose-approver-or-reviewer.png)

1. 重複步驟5至6以新增其他核准者或稽核者。
儲存之後，新增的參與者會收到電子郵件通知，告知檔案需要其核准或稽核。







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
