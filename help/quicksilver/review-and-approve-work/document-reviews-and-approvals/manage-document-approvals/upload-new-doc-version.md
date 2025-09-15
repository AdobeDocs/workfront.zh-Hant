---
product-area: documents
navigation-topic: approvals
title: 上傳新檔案版本並請求核准
description: 您可以上傳新檔案版本，並向Adobe Workfront中的其他使用者請求核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 42fbb40cb8a0f3c70e22fd04bd3d0ce625f58fec
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 上傳新檔案版本並請求核准

如果標示的檔案需要在先前的稽核中工作，您可以將新版本上傳到原始檔案並開始另一輪核准。 上傳檔案的新版本後，先前版本即會鎖定。

如果新版本的檔案名稱與先前版本的檔案名稱不同，則Workfront會顯示具有較新檔案名稱的檔案。

當新版本新增到具有未完成核准的檔案時，先前版本的核准顯示為「已撤回」。 即使部分參與者尚未做出決定，先前的核准流程也會關閉。

如果刪除了最新的檔案版本，先前的版本仍會保持鎖定。 如果您需要編輯先前的版本，則必須手動解除鎖定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p>
   <p>投稿人或以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>編輯與檔案關聯之物件的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用拖放功能來新增版本

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
   >   擁有Standard授權的使用者可以從「設定」區域建立可繼續使用的核准範本。 如需詳細資訊，請參閱[建立資產和檔案的核准範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。


1. （選用）設定核准的截止日期。 若在指定期限前72小時通知使用者和團隊。

1. 新增所有檢閱者和核准者後，請按一下&#x200B;**提交請求**。 系統會透過電子郵件通知參與者。

   ![提交新版本以供核准](assets/add-previous-participants.png)


