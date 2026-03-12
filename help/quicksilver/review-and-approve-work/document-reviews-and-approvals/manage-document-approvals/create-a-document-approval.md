---
product-area: documents
navigation-topic: approvals
title: 建立檔案核准工作流程
description: 您可以在Adobe Workfront中請求其他使用者的檔案核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: 149c8adcf886f837bc94ac78f8a3ea54c47e375c
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 2%

---

# 建立檔案核准工作流程

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

您可以在Adobe Workfront中請求其他使用者或團隊核准檔案，或請求他們稽核檔案而無需核准。

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
   <td> <p>管理與請求存取或核准相關聯的物件存取權 </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 從生產環境中的檔案頁面建立檔案檢閱或核准請求

1. 將滑鼠停留在檔案上，然後按一下「檔案詳細資訊」。
   ![檔案詳細資料](assets/doc-details.png)

1. 在檔名稱附近，在版本下拉式清單中選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 按一下左側面板中的&#x200B;**核准**。

1. （選用）設定核准的截止日期。 若在指定期限前72小時通知使用者和團隊。

1. 若要新增核准者，請按一下&#x200B;**核准者**&#x200B;並開始輸入使用者或團隊名稱。

1. 若要新增檢閱者，請按一下&#x200B;**檢閱者**&#x200B;核取方塊並開始輸入使用者或團隊名稱。

   ![新增核准者與截止日期](assets/add-approver-and-deadline.png)

1. 重複上一步驟以新增其他核准者或稽核者。

## 從生產環境中的檔案摘要面板建立檔案檢閱或核准請求

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。

1. 按一下您需要的檔案，該檔案的「檔案摘要」左側面板隨即開啟。

1. 在版本下拉式清單中選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 向下捲動至[檔案摘要]窗格中的&#x200B;**核准**&#x200B;區段，然後按一下[新增]。****

![在檔案摘要中新增核准者](assets/doc-summary-add-approvers.png)

1. （選用）設定核准的截止日期。 若在指定期限前72小時通知使用者和團隊。

1. 若要新增核准者，請按一下&#x200B;**核准者**&#x200B;並開始輸入使用者或團隊名稱。

1. 若要新增檢閱者，請按一下&#x200B;**檢閱者**&#x200B;核取方塊並開始輸入使用者或團隊名稱。

   ![新增核准者與截止日期](assets/add-approver-and-deadline.png)

1. 重複上一步驟以新增其他核准者或稽核者。

<div class="preview">

## 在舊版檔案區域的預覽環境中，從「摘要」面板建立核准工作流程

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存的詳細資訊，請參閱[Workfront儲存與Adobe企業儲存的比較](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)。

若要建立核准工作流程：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下您需要的檔案，該檔案的「檔案摘要」面板隨即開啟。

1. 在版本下拉式清單中選取您要建立核准的檔案版本。 預設會選取最新版本。

1. 向下捲動至&#x200B;**核准**&#x200B;區段，然後按一下&#x200B;**建立工作流程**。


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
   <td><strong>到期日（選擇性）</strong></td>
   <td>設定核准的到期日。 使用者與團隊會收到電子郵件通知，通知時間為指定到期日前72小時或24小時。</td>
   </tr>
   </table>

1. （選擇性）重複上一步驟，視需要新增其他階段。

   >[!NOTE]
   >
   >如果您新增多個階段，核准工作流程會依階段列出的順序進行。 完成所有必要的決定後，下一個階段會開始，而上一個階段會鎖定。

   ![檔案詳細資料](assets/new-stage.png)

</div>

## 從新檔案區域的摘要面板建立核准工作流程

如果您的組織使用企業儲存空間，當您存取Workfront中的檔案時，將會看到新檔案區域。 如需企業儲存的詳細資訊，請參閱[企業儲存概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

若要建立核准工作流程，請執行下列步驟：

1. 前往包含檔案的專案、任務或問題，然後在左側面板中選取&#x200B;**檔案**。

1. 按一下檔案，然後按一下頁面右側的「核准」圖示。

   ![在檔案摘要中新增核准者](assets/approvals-icon-new.png)

1. 按一下「**建立工作流程**」，然後填寫下列詳細資料：

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
