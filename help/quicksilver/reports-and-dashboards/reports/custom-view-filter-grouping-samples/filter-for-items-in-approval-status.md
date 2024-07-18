---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選器：僅顯示處於核准狀態的專案」
description: 您只能顯示目前處於「未決核准」之特定狀態的專案。 對於任何其他具有核准狀態的物件，其運作方式都相同。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---

# 篩選：僅顯示處於核准狀態的專案

您只能顯示目前處於「未決核准」之特定狀態的專案。 對於任何其他具有核准狀態的物件，其運作方式都相同。

您可以將下列物件置於核准狀態：

* 任務
* 問題
* 專案

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 僅顯示處於核准狀態的專案

1. 例如，前往您要自訂專案清單的篩選器。
1. 按一下清單物件的&#x200B;**狀態**&#x200B;欄位的&#x200B;**新增篩選規則**。\
   例如，在專案報告中，如果您只想顯示處於&#x200B;**計畫 — 未決核准**&#x200B;狀態的專案，請新增&#x200B;**狀態等於計畫**。

1. 按一下&#x200B;**切換到文字模式**。
1. 修改

   ```
   status
   ```

   新增&#x200B;**：A**&#x200B;至狀態的3字母索引鍵後行：
   <pre>status=PLN：A<br>status_Mod=in</pre>

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存篩選器**。

   此清單只會顯示處於「計畫 — 未決核准」狀態的專案。
