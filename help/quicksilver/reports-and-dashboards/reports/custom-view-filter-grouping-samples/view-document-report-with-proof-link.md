---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 檢視：包含校訂連結的檔案報告
description: 檢視：包含校訂連結的檔案報告
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---

# 檢視：包含校訂連結的檔案報告

<!--Audited: 11/2024-->

在此檔案檢視中，您可以插入指向檔案目前版本的校訂的連結。

![](assets/view-document-with-proof-link-350x92.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視檔案報告，其中包含校訂連結

若要套用此檢視：

1. 移至檔案清單。
1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。
1. 按一下「**新增欄**」。
1. 按一下&#x200B;**切換到文字模式**，然後按一下&#x200B;**編輯文字模式**。
1. 移除您在&#x200B;**編輯文字模式**&#x200B;方塊中找到的文字，並取代為下列程式碼：

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

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**。
1. （選擇性）更新檢視名稱，然後按一下&#x200B;**儲存檢視**。
1. （選用）若要確保只顯示包含校樣的檔案，請執行以下動作來新增篩選器：

   1. 按一下&#x200B;**篩選器**&#x200B;下拉式功能表，然後按一下&#x200B;**新增篩選器**。
   1. 按一下&#x200B;**新增篩選器規則**&#x200B;並開始輸入「校訂所有者」，然後在其顯示在清單中時選取&#x200B;**校訂所有者ID**。
   1. 針對篩選修飾元選取&#x200B;**Is Not Blank**。
   1. 按一下「**儲存篩選器**」。
   1. （選擇性）更新篩選器名稱，然後按一下&#x200B;**儲存篩選器**。

1. 按一下校訂連結欄中的連結以存取檔案最新版本的校訂。
