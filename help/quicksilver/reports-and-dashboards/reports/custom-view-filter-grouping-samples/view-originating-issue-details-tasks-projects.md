---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：源項任務和項目的問題詳細資訊'
description: 將問題轉換為任務或項目時，將在任務或項目與問題之間建立解決對象關係。 此視圖顯示任務或項目完成時自動完成的問題的以下欄位 — 「編輯我」。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# 視圖：任務和項目的原始問題詳細資訊

將問題轉換為任務或項目時，將在任務或項目與問題之間建立解決對象關係。 此視圖顯示任務或項目完成時自動完成的問題的以下欄位：

* 名稱
* 輸入日期
* 計畫完成日期
* 實際完成日期
* 請求類型
* 發起方名稱
* 分配給用戶

![task_with_resolving_issue_fields_png](assets/task-with-resolving-issue-fields-350x38.png)

有關詳細資訊，另請參閱 [視圖：顯示任務和項目清單的原始問題資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md)。

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

## 查看任務和項目的原始問題詳細資訊

1. 轉到任務清單或項目清單。
1. 從 **視圖** 下拉菜單，選擇 **新建視圖**。

1. 在&#x200B;**列預覽** 框中，刪除除一個列之外的所有列。
1. 按一下其餘列的標題，然後按一下 **切換到文本模式**。
1. 將滑鼠移到文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 按一下 **保存視圖**。
