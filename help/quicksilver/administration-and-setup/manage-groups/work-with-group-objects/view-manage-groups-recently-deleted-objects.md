---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 檢視和管理群組最近刪除的專案
description: 當您檢視在「群組」區域中管理的群組時，可以檢視、篩選、還原和匯出其最近刪除的工作專案、檔案和範本。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 1%

---

# 檢視及管理群組最近刪除的專案

當您在「群組」區域中檢視您管理的群組時，可以下列方式檢視和處理其最近刪除的專案、任務、問題、檔案和範本：

* 檢視、篩選及分組最近刪除的專案的清單
* 還原您選取的最近刪除的專案
* 匯出最近刪除的專案的清單

如果您的群組之上有任何群組，其管理員也可以為您的群組執行下列動作。 Workfront管理員也是如此（適用於任何群組）。

如需有關已刪除專案的詳細資訊，請參閱[管理已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td>
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
  <tr> 
   <td role="rowheader">物件許可權</td>
   <td>已刪除的專案必須與群組或其任何子群組相關聯。</td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視及管理群組最近刪除的專案

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

1. 按一下群組的名稱。
1. 在左側面板中，按一下&#x200B;**最近刪除的**。
1. 開啟下列其中一個標籤，您可在其中檢視和管理群組最近刪除的專案：

   * 專案
   * 任務
   * 問題
   * 文件
   * 範本

   每個標籤會列出屬於目前群組或其子群組且在過去30天內刪除的對應物件型別專案。

   >[!NOTE]
   >
   >如果有人刪除了專案，則會一併刪除專案的所有個別任務、問題和檔案。 這些標籤不會個別顯示在任務、問題、檔案或範本標籤上。 不過，還原專案也會將所有這些子物件還原至專案。
   >
   >
   >如果有人個別刪除任務、問題、檔案或範本，您可以在適當的索引標籤上檢視和管理它。

1. 完成下列任一動作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>還原物件</p> </td> 
      <td> <p>選取最多10個物件，然後按一下[還原]。<strong></strong></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>匯出標籤上的整個物件清單</p> </td> 
      <td> <p>按一下<strong>匯出</strong>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>變更清單中資訊的顯示</p> </td> 
      <td> <p>在清單的右上角，使用<strong>篩選器</strong>來根據您提供的條件定義顯示內容。 使用<strong>檢視</strong>定義哪些欄位會顯示為欄。 使用<strong>分組</strong>將專案分組為類別。</p> </td> 
     </tr> 
    </tbody> 
   </table>
