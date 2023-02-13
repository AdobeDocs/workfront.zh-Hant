---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：連結至校樣的檔案報表'
description: '''檢視：連結至校樣的檔案報表'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 40c7142574c3491b7bdf8799c287db1c3f7e9e8c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 查看：包含校樣連結的檔案報表

在此文檔視圖中，可以插入指向文檔當前版本校樣的連結。

![](assets/view-document-with-proof-link-350x92.png)

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 查看包含校樣連結的文檔報告

要應用此視圖，請執行以下操作：

1. 轉到文檔清單。
1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 按一下 **添加列**.
1. 按一下 **切換到文本模式**.
1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >將「您的網域」取代為實際的Workfront網域。 例如，如果您公司的Workfront url是 *Company.my.workfront.com*，您的網域為「公司」。

1. 按一下 **儲存**，然後 **保存視圖**.
1. 輸入檢視的名稱，然後按一下 **保存視圖**.
1. （可選）若要確保只顯示帶校樣的文檔，請執行以下操作來添加篩選器：

   1. 按一下 **篩選** 下拉式功能表，然後按一下 **新增篩選**.
   1. 按一下 **新增篩選規則** 然後開始鍵入校樣所有者，然後選擇 **校樣擁有者ID** 顯示於清單中時。
   1. 選擇 **非空白** （針對篩選修飾詞）。
   1. 按一下 **儲存篩選**，輸入篩選器名稱，然後按一下 **儲存篩選**.

1. 按一下「校樣連結」欄中的連結，以存取最後一個版本的檔案校樣。
