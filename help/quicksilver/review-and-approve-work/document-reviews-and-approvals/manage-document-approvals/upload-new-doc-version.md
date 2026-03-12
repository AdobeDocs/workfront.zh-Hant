---
product-area: documents
navigation-topic: approvals
title: 上傳新檔案版本並請求核准
description: 您可以上傳新檔案版本，並向Adobe Workfront中的其他使用者請求核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 2%

---

# 上傳新檔案版本並請求核准

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

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
   <td> <p>任何</p> </td> 
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


## 使用拖放功能，在生產環境中新增版本

>[!NOTE]
>
>Internet Explorer無法使用拖放功能。


如果您需要對檔案執行另一輪稽核和核准，可以在Workfront中建立新的檔案版本。

您可以新增先前的參與者、新參與者或兩者的組合。 您可以在「檔案詳細資訊」頁面上檢視先前版本和參與者的相關資訊。

若要新增版本：

1. 導覽至Workfront中的檔案。
1. 將新檔案拖放至上一個檔案的頂端。 這會自動建立新版本。

1. 檔案上傳完成後，請選取檔案，然後按一下&#x200B;**檔案詳細資料**。
   ![開啟檔案詳細資料頁](assets/open-doc-details.png)


1. 在左側面板中，按一下&#x200B;**核准**，然後按一下&#x200B;**新增**。

1. 若要新增所有先前的參與者，請按一下[全部新增]。**&#x200B;** 您也可以視需要新增參與者或移除先前的參與者。


1. 若要新增現有的核准範本，請按一下「範本」按鈕並開始輸入範本名稱。

   >[!TIP]
   >
   >   擁有Standard授權的使用者可以從「設定」區域建立可重複使用的核准範本。 如需詳細資訊，請參閱[建立檔案的核准工作流程範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。


1. （選用）設定核准的截止日期。 若在指定期限前72小時通知使用者和團隊。

1. 新增所有檢閱者和核准者後，請按一下&#x200B;**提交請求**。 系統會透過電子郵件通知參與者。

   ![提交新版本以供核准](assets/add-previous-participants.png)





<div class="preview">

## 使用拖放功能，在舊版檔案區域的預覽環境中新增版本

如果您的組織使用Workfront儲存空間，當您存取Workfront中的檔案時，將會看到舊版檔案區域。 如需Workfront儲存的詳細資訊，請參閱[Workfront儲存與Adobe企業儲存的比較](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)。

>[!NOTE]
>
>Internet Explorer無法使用拖放功能。


如果您需要對檔案執行另一輪稽核和核准，可以在Workfront中建立新的檔案版本。

您可以新增先前的參與者、新參與者或兩者的組合。 您可以在「檔案詳細資訊」頁面上檢視先前版本和參與者的相關資訊。

若要新增版本：

1. 導覽至Workfront中的檔案。
1. 將新檔案拖放至上一個檔案的頂端。 這會自動建立新版本。

1. 檔案上傳完成後，請選取檔案以開啟檔案摘要面板。 您會在面板頂端看到版本號碼。
   ![開啟檔案詳細資料頁](assets/open-doc-details.png)


1. 向下捲動至&#x200B;**核准**&#x200B;區段。

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



1. （可選）若要新增現有的核准範本，請從對話方塊左側選取範本。

   >[!TIP]
   >
   >   擁有Standard授權的使用者可以從「設定」區域建立可重複使用的核准範本。 如需詳細資訊，請參閱[建立檔案的核准工作流程範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。



1. 新增您需要的所有階段和參與者後，按一下&#x200B;**要求核准**。

   核准工作流程隨即開始，核准者會收到新檔案版本需要其核准的通知。 先前檔案版本已鎖定，並撤銷先前版本上的所有未完成核准。

   ![要求核准](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->



</div>

