---
product-area: documents
navigation-topic: approvals
title: 上傳新檔案版本並請求核准
description: 您可以上傳新檔案版本，並向Adobe Workfront中的其他使用者請求核准。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---

# 上傳新檔案版本並請求核准

如果標示的檔案需要在先前的稽核中工作，您可以將新版本上傳到原始檔案並開始另一輪核准。 上傳檔案的新版本後，先前版本即會鎖定。

如果新版本的檔案名稱與先前版本的檔案名稱不同，則Workfront會顯示具有較新檔案名稱的檔案。

當新版本新增到具有未完成核准的檔案時，先前版本的核准顯示為「已撤回」。 即使部分參與者尚未做出決定，先前的核准流程也會關閉。

如果刪除了最新的檔案版本，先前的版本仍會保持鎖定。 如果您需要編輯先前的版本，則必須手動解除鎖定。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前：要求或以上</p>
   或
   <p>新增：投稿人或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>編輯與檔案關聯之物件的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

+++

## 使用拖放功能來新增版本

>[!NOTE]
>
>Internet Explorer無法使用拖放功能。

1. 前往檔案上傳所在區域。
1. 從您的案頭或單獨的瀏覽器索引標籤，將檔案的新版本拖曳到Workfront中現有版本的上方。

   拖曳新版本時，您可以將游標停留在Workfront檔案資料夾上以開啟。 然後，您就可以將檔案拖曳至熒幕的頂端或底部，上下捲動。

1. 將新版本拖放到&#x200B;**檔案**&#x200B;索引標籤上的現有檔案上。

1. 上傳檔案後，按一下檔案並開啟檔案摘要面板。

1. 向下捲動至[檔案摘要]窗格中的&#x200B;**核准**&#x200B;區段，然後按一下[新增]。****

![在檔案摘要中新增核准者](assets/doc-summary-add-approvers.png)

1. （選用）設定核准的截止日期。 若在指定期限前72小時通知使用者和團隊。

1. 若要快速新增先前版本的稽核者和核准者，請按一下下列其名稱旁的新增按鈕。
   <!--need screenshot when working-->

1. （選擇性）從核准者/稽核者變更角色。

1. 若要新增核准者和稽核者，請按一下[稽核者] ****&#x200B;或[核准者] ****，然後開始輸入使用者或團隊。

   ![新增核准者與截止日期](assets/add-approver-and-deadline.png)
