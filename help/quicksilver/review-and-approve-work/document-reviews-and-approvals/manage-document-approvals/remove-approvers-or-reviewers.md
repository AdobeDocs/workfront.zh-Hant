---
product-area: documents
navigation-topic: approvals
title: 從檔案核准工作流程中移除核准者或稽核者
description: 您可以從檔案中移除個別核准者或稽核者。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 2%

---

# 從檔案核准工作流程中移除核准者或稽核者

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

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


## 從您生產環境的「檔案詳細資訊」頁面中移除核准者或稽核者

1. 按一下檔名稱，移至檔案頁面，然後在版本下拉式清單中選取您要移除核准的檔案版本。 預設會選取最新版本。

1. 在左側面板中選取&#x200B;**核准**。

1. 將游標暫留在您要移除的核准者或檢閱者名稱上，然後按一下其名稱后面出現的&#x200B;**刪除**&#x200B;圖示![刪除圖示](../assets/delete.png)。

   核准或稽核請求被移除，且核准者會收到不再需要其核准的通知。 也會移除其核准相關的共用存取權。

1. （選擇性）若要將核准者降級給檢閱者，而非將其完全移除，請取消勾選與其名稱一致的&#x200B;**核准者**&#x200B;核取方塊。

1. 重複上一步驟以移除任何其他核准者或稽核者。

## 從您生產環境的檔案摘要中移除核准者或稽核者

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 在版本下拉式清單中選取您要移除核准者或稽核者的檔案版本。 預設會選取最新版本。

1. 向下捲動至檔案摘要面板中的&#x200B;**核准**&#x200B;區段。 將游標暫留在您要移除的核准者或檢閱者名稱上，然後按一下其名稱后面出現的&#x200B;**刪除**&#x200B;圖示![刪除圖示](../assets/delete.png)。

   核准或稽核請求被移除，且核准者會收到不再需要其核准的通知。 也會移除其核准相關的共用存取權。

1. （選擇性）若要將核准者降級給檢閱者，而非將其完全移除，請取消勾選與其名稱一致的&#x200B;**核准者**&#x200B;核取方塊。

1. 重複上一步驟以移除任何其他核准者或稽核者。


<div class="preview">

## 在舊版檔案區域的預覽環境中，從核准工作流程中移除核准者或稽核者

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存的詳細資訊，請參閱[Workfront儲存與Adobe企業儲存的比較](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)。

若要從核准工作流程中移除核准者或稽核者：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 向下捲動至檔案摘要面板中的&#x200B;**核准**&#x200B;區段。

1. 按一下&#x200B;**編輯工作流程**。

1. 找到您要移除的參與者，然後按一下其名稱旁的&#x200B;**移除**&#x200B;圖示。

   核准或稽核請求被移除，且核准者會收到不再需要其核准的通知。 也會移除其核准相關的共用存取權。

   ![編輯核准工作流程](assets/edit-approval-in-legacy.png)

1. （可選）若要將核准者的角色變更為稽核者（或反之），請按一下使用者名稱旁的下拉式功能表，然後選取新角色。

1. 重複上一步驟以移除任何其他核准者或稽核者。

</div>


## 在新檔案區域中移除核准者或稽核者至核准工作流程

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 如需企業儲存的詳細資訊，請參閱[企業儲存概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

若要建立核准工作流程，請執行下列步驟：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下檔案，然後按一下頁面右側的&#x200B;**核准**&#x200B;圖示。

   ![在檔案摘要中新增核准者](assets/approvals-icon-new.png)


1. 按一下&#x200B;**編輯工作流程**。

1. 找到您要移除的參與者，然後按一下其名稱旁的&#x200B;**移除**&#x200B;圖示。

   核准或稽核請求被移除，且核准者會收到不再需要其核准的通知。

1. （可選）若要將核准者的角色變更為稽核者（或反之），請按一下使用者名稱旁的下拉式功能表，然後選取新角色。

1. 重複上一步驟以移除任何其他核准者或稽核者。

   ![從階段中移除參與者](assets/add-or-remove-participants.png)
1. 按一下「**儲存**」。