---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案」
description: 您可以將具有3個字母鍵NST的任務狀態指派給群組A （已命名的新狀態）。 您可能有另一個任務狀態指派給群組B，也命名為New Status ，帶有3個字母的索引鍵NES。 雖然2個狀態的名稱可以相同，但3個字母的程式碼永遠都是唯一的。 如需群組狀態的詳細資訊，請參閱建立或編輯群組狀態。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 篩選：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案

您可以讓任務狀態指派給群組A （名稱為&#x200B;*新狀態*，包含3個字母的索引鍵&#x200B;*NST*）。 您可能有另一個工作狀態指派給群組B，也命名為&#x200B;*新狀態*，其索引鍵為&#x200B;*NES。*&#x200B;雖然2個狀態的名稱可以相同，但3個字母的程式碼永遠都是唯一的。\
如需群組狀態的詳細資訊，請參閱[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

使用篩選產生器，您無法識別具有相同名稱的2個狀態。 您必須使用「文字模式」來區分2種狀態。

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

## 當狀態與不同群組相關聯時，依相同名稱狀態顯示專案

1. 例如，移至您要自訂的篩選器以取得工作清單。\
   這也適用於專案和問題。
1. 按一下清單物件的&#x200B;**狀態**&#x200B;欄位的&#x200B;**新增篩選規則**。\
   例如，在任務報告中，如果您只想顯示狀態為&#x200B;**新狀態**&#x200B;的任務，請新增&#x200B;**狀態等於新狀態**。

   >[!TIP]
   >
   >請注意，對於名為「新狀態」的狀態，您只有一個選項。

1. 按一下&#x200B;**切換到文字模式**。\
   應顯示下列程式碼：
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >此處只顯示一個狀態。 狀態行會顯示其中一個狀態的3個字母鍵之一。

1. 新增下列2行程式碼，以新增篩選器中缺少的狀態：
   <pre>OR:1:狀態=NES<br>OR:1:狀態_模式=in</pre>

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存篩選器**。

   清單會顯示群組A的「新狀態」狀態與群組B的「新狀態」狀態任務。
