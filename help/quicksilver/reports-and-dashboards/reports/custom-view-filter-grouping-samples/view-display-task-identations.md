---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：在任務清單中顯示任務縮進'
description: 在此任務視圖中，您可以向「任務名稱」列添加代碼，以根據項目的「工作細分結構」顯示縮進的任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 視圖：在任務清單中顯示任務縮進

在此任務視圖中，您可以向「任務名稱」列添加代碼，以根據項目的「工作細分結構」顯示縮進的任務。

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## 在任務清單的列中顯示任務縮進

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖**。

1. 按一下 **添加列** 並在 **在此列中顯示** 欄位，然後在清單中顯示時選擇它。

1. 在新列中，按一下 **切換到文本模式**。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本

   ```
   valuefield=
   ```

   並用以下代碼替換：

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. 按一下 **保存**，則 **保存視圖**。
