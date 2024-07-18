---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：包含校訂連結的檔案報告」
description: 「檢視：包含校訂連結的檔案報告」
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# 檢視：包含校訂連結的檔案報告

在此檔案檢視中，您可以插入指向檔案目前版本的校訂的連結。

![](assets/view-document-with-proof-link-350x92.png)

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
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 檢視檔案報告，其中包含校訂連結

若要套用此檢視：

1. 移至檔案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 按一下「**新增欄**」。
1. 按一下&#x200B;**切換到文字模式**。
1. 暫留在文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 移除您在&#x200B;**文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >將「您的網域」取代為您的實際Workfront網域。 例如，如果貴公司的Workfront URL是&#x200B;*Company.my.workfront.com*，則您的網域是「公司」。

1. 按一下&#x200B;**儲存**，然後按一下&#x200B;**儲存檢視**。
1. 輸入檢視的名稱，然後按一下&#x200B;**儲存檢視**。
1. （選用）若要確保只顯示包含校樣的檔案，請執行以下動作來新增篩選器：

   1. 按一下&#x200B;**篩選器**&#x200B;下拉式功能表，然後按一下&#x200B;**新增篩選器**。
   1. 按一下&#x200B;**新增篩選規則**&#x200B;並開始輸入校訂擁有者，然後選取&#x200B;**校訂擁有者ID**（當它顯示在清單中時）。
   1. 針對篩選修飾元選取&#x200B;**Is Not Blank**。
   1. 按一下&#x200B;**儲存篩選**，輸入篩選的名稱，然後按一下&#x200B;**儲存篩選**。

1. 按一下校訂連結欄中的連結以存取檔案最新版本的校訂。
