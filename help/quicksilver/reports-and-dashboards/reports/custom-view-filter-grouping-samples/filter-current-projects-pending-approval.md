---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：顯示您當前的項目等待審批'
description: 以下項目篩選器顯示處於「當前 — 待批」狀態的項目，其中登錄用戶是項目發起人或Portfolio經理。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 篩選器：顯示當前項目等待審批

以下項目篩選器顯示處於「當前 — 待批」狀態的項目，其中登錄用戶是項目發起人或Portfolio經理。

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改篩選器</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 篩選待審批的當前項目

要應用此篩選器：

1. 轉到項目清單。
1. 從 **篩選** 下拉菜單，選擇 **新建篩選器**。

1. 按一下&#x200B;**切換到文本模式**。
1. 在 **設定報表的篩選器規則** 複製並貼上以下代碼：
   <pre>status=CUR:A<br>ponsorID=$$USER.ID<br>或:a:status=CUR:A<br>或:a:portfolio:ownerID=$$USER.ID</pre>

1. 按一下 **保存篩選器**。
