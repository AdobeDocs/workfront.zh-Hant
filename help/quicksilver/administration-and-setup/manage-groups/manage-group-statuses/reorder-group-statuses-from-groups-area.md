---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 重新排序群組狀態
description: 作為群組管理員，您可以變更您管理之群組的專案、任務和問題狀態的順序。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 7%

---

# 重新排序群組狀態

作為群組管理員，您可以變更您管理之群組的專案、任務和問題狀態的順序。

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

>[!NOTE]
>
>* Workfront管理員可以在系統層級重新排序狀態。 這不會影響群組內的狀態順序。
>
>  但是，新建立的頂層群組內的狀態會繼承系統層級狀態的順序。 （新的子群組會繼承群組內上一層之狀態的順序。）
>
>* 您可以重新排序鎖定狀態。 如需有關鎖定狀態的資訊，請參閱[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

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
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 預設狀態順序

依預設，狀態會依下列順序顯示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">專案</th> 
   <th width="33.33%">任務</th> 
   <th width="33.33%">問題</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>目前</p> 
     <p>廢棄</p> 
     <p> 保留 </p> 
     <p> 計畫 </p> 
     <p> 完成 </p> 
     <p> 已請求 </p> 
     <p> 已核准 </p> 
     <p> 已拒絕 </p> 
     <p> 構想 </p> 
   </td> 
   <td> 
     <p>新增</p> 
     <p>進行中</p> 
     <p>完成</p> 
   </td> 
   <td> 
     <p>新增</p> 
     <p>進行中</p> 
     <p>重新處理</p> 
     <p>等待意見反應</p> 
     <p>保留</p> 
     <p>無法複製</p> 
     <p>已關閉</p> 
     <p>已解決</p> 
     <p>確認完成</p> 
     <p>不會解決</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## 在您管理的群組中重新排序任務和專案狀態

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組**，然後按一下群組的名稱。
1. 在左側面板中，按一下&#x200B;**狀態**。
1. 在顯示的狀態清單上方，按一下&#x200B;**專案**&#x200B;或&#x200B;**任務**&#x200B;標籤。

1. 以您想要的順序拖放狀態。

   新的狀態順序會自動儲存。

1. 若要測試新的狀態順序，請前往與群組相關聯的任務或專案，按一下右上角的狀態，並確定顯示的狀態是按照您設定的順序。

## 重新排序問題的狀態

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組**，然後按一下群組的名稱。
1. 在左側面板中，按一下&#x200B;**狀態**。
1. 按一下&#x200B;**問題**&#x200B;標籤。
1. （選擇性）選取問題型別（**錯誤報告**、**變更順序**、**問題**&#x200B;或&#x200B;**要求**）。

   >[!NOTE]
   >
   >* 您無法自訂主清單的狀態順序。
   >* 我們建議您以相同方式排序每個問題型別的狀態。 如需問題型別的詳細資訊，請參閱[設定要求型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 以您想要的順序拖放狀態。

   新的狀態順序會自動儲存。

1. 若要測試新的狀態順序，請前往與群組關聯的問題，按一下右上角的狀態，並確認顯示的狀態是按照您設定的順序。
