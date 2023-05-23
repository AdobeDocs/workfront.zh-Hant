---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：帶有指向證明的連結的文檔報告」'
description: '''查看：帶有指向證明的連結的文檔報告」'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 視圖：帶有指向證明的連結的文檔報告

在此文檔視圖中，可以插入指向文檔當前版本證明的連結。

![](assets/view-document-with-proof-link-350x92.png)

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 查看包含證明連結的文檔報告

要應用此視圖，請執行以下操作：

1. 轉到文檔清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 按一下 **添加列**。
1. 按一下 **切換到文本模式**。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >將「您的域」替換為您的實際Workfront域。 例如，如果您公司的Workfronturl是 *Company.my.workfront.com*&#x200B;你的域名是&quot;公司&quot;

1. 按一下 **保存**，則 **保存視圖**。
1. 鍵入視圖的名稱，然後按一下 **保存視圖**。
1. （可選）要確保只顯示帶校樣的文檔，請執行以下操作來添加篩選器：

   1. 按一下 **篩選** 下拉菜單，然後按一下 **新建篩選器**。
   1. 按一下 **添加篩選器規則** 然後開始鍵入Proof Owner，然後選擇 **證明所有者ID** 清單中顯示。
   1. 選擇 **不為空** 按鈕。
   1. 按一下 **保存篩選器**，鍵入篩選器的名稱，然後按一下 **保存篩選器**。

1. 按一下「校樣連結」列中的連結，以訪問文檔上一版本的校樣。
