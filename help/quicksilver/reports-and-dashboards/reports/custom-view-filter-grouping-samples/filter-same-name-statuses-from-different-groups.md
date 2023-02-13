---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''篩選：在狀態與不同組關聯時按相同名稱狀態顯示項'
description: 您可以使用3個字母的鍵NST將任務狀態分配給組A命名的新狀態。 您可能已將另一個任務狀態分配給組B，該組名為New Status,3個字母的鍵為NES。 雖然2個狀態的名稱可以相同，但3個字母的代碼始終是唯一的。 有關組狀態的詳細資訊，請參閱建立或編輯組狀態。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 篩選：在狀態與不同組關聯時按相同名稱狀態顯示項

您可以將任務狀態指派給已命名的 *新狀態* 帶3個字母的鍵 *NST*. 您可能已將另一個任務狀態指派給B組，也命名為 *新狀態* 帶3個字母的鍵 *NES。* 雖然2個狀態的名稱可以相同，但3個字母的代碼始終是唯一的。\
如需群組狀態的詳細資訊，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

使用篩選產生器時，您無法識別具有相同名稱的2種狀態。 您必須使用「文字模式」來區分兩種狀態。

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

## 在狀態與不同組關聯時按相同名稱狀態顯示項

1. 移至您要自訂的篩選器，以取得工作清單。\
   對於專案和問題，也同樣適用。
1. 按一下 **新增篩選規則** 針對 **狀態** 清單對象的欄位。\
   例如，在任務報表中，新增 **狀態等於新狀態**，如果您只想顯示狀態為 **新狀態**.

   >[!TIP]
   >
   >請注意，您只有一個狀態選項名為「新狀態」。

1. 按一下 **切換到文本模式**.\
   應顯示下列程式碼：

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >此處只顯示一個狀態。 狀態行顯示其中一個狀態的3個字母鍵之一。

1. 新增下列2行程式碼，以新增篩選器中遺失的狀態：

   <pre>或:1:status=NES<br>或:1:status_Mod=in</pre>

1. 按一下 **完成**，然後 **儲存篩選**.

   清單會顯示組A中狀態為「新狀態」和組B狀態為「新狀態」的任務。
