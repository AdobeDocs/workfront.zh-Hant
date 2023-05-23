---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '篩選：僅顯示處於審批狀態的項目'
description: 您只能顯示當前處於「待批」狀態的特定狀態的項目。 這對於具有批准狀態的任何其它對象都同樣適用。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# 篩選器：僅顯示處於審批狀態的物料

您只能顯示當前處於「待批」狀態的特定狀態的項目。 這對於具有批准狀態的任何其它對象都同樣適用。

您可以將以下對象置於批准狀態：

* 任務
* 問題
* 專案

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

## 僅顯示處於審批狀態的物料

1. 例如，轉到要為項目清單自定義的篩選器。
1. 按一下 **添加篩選器規則** 為 **狀態** 的子菜單。\
   例如，在項目報告中，添加 **狀態相等計畫**，如果只顯示狀態為 **計畫 — 待批**。

1. 按一下 **切換到文本模式**。
1. 修改

   ```
   status
   ```

   添加行 **:A** 至狀態的3個字母鍵：
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. 按一下 **完成**，則 **保存篩選器**。

   該清單僅顯示處於「計畫 — 待批」狀態的項目。
