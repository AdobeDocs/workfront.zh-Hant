---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 通過拖放來分配工作負載平衡器中的工作
description: 通過將工作項拖放給正確的用戶，可以使用Adobe Workfront工作負載平衡器來分配工作項。
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 1%

---

# 通過拖放來分配工作負載平衡器中的工作

<!--remove production and preview preferences at release-->

通過將工作項拖放給正確的用戶，可以使用Adobe Workfront工作負載平衡器來分配工作項。

有關使用工作負載平衡器為用戶分配工作的一般資訊，請參見 [工作負載平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>在使用團隊或「資源配置」區域中的工作負載平衡器時進行計畫 </p>
   <p>使用項目的工作負載平衡器時工作 </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯對以下項目的存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>將權限或更高版本貢獻給包括「進行分配」的項目、任務和問題</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 拖放以指派項目

您可以從「未分配的工作」區域將項目分配給某個用戶，或者可以在「已分配的工作」區域中將已分配的項目重新分配給另一個用戶。

1. 轉到要分配工作的工作負載平衡器。

   您可以在資源區域、項目或團隊級別使用工作負載平衡器為用戶分配工作。 有關工作負載平衡器在Workfront中的位置的詳細資訊，請參見 [找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. （選用）前往 **未分配的工作** 區域和套用篩選器，以檢視未指派給使用者的工作和問題

   或

   前往 **已分配的工作** 區域，並展開用戶的名稱以查看分配給他們的工作項目（如果要重新分配其項目）。

1. （條件性）在項目的工作負載平衡器中，按一下 **顯示所有用戶** 圖示 ![](assets/show-all-users-icon-project-workload-balancer.png) 以顯示所有Workfront使用者。

   這會顯示您有權檢視的所有使用者。

   也是項目團隊的一部分，並且已分配給項目上的項目的用戶在「已分配的工作」區域中其名稱的右側有項目表徵圖。

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* 「顯示所有用戶」選項僅在項目的工作負載平衡器中可用。
   >* 使用篩選器只顯示對您而言重要的使用者。 例如，使用篩選器只顯示來自您團隊或群組的使用者。




1. 按一下工作項的欄，指明計畫時間軸或預計時間軸，並將其拖曳至 **已指派** 的上界。

   您暫留的使用者會反白顯示將工作項目放置到的。

   >[!TIP]
   >
   >您暫留在更新上的用戶的計畫小時數，即時顯示工作項的每日計畫小時數，以指明添加新項可能對其整體分配產生什麼影響。

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. 準備就緒後，將所選工作項與分配區域中的用戶名放在同一行中。 系統會為用戶分配物料，並更新已分配的計畫小時數，其中包含工作物料的新小時數。

   如果將項目分配給用戶無法履行的作業角色，則該項目將顯示在「已分配的工作」區域中用戶名下，並且它仍保留在「未分配的工作」區域中，以指明與其關聯的作業角色尚未被用戶替換。

   >[!TIP]
   >
   >* 如果在「設定」區域中啟用了「按項目分組」，則分配的任務將顯示在相應的項目下。 如果禁用了該設定，則分配的任務將顯示在用戶區域中。
      >
      >
      >     該項根據工作項排序的工作負載平衡器標準顯示。 如需詳細資訊，請參閱 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* 如果啟用了「顯示項目的工作負載平衡器中的所有用戶」，並將項目分配給先前未分配給項目上項目的用戶，則用戶將添加到項目組。 如需詳細資訊，請參閱 [管理專案團隊](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. （可選）在「已分配的工作」區域中按一下用戶名稱下的工作項目欄，然後將其拖動到「未分配的工作」區域上以取消分配。 該項目從用戶未分配，但可能仍被分配給作業角色，在這種情況下，它會顯示在「未分配的工作」區域中。 如果將項目分配給其他用戶，則該項目將保留在「已分配的工作」區域中，其名稱為仍被分配的用戶。
1. （選用）按一下 **顯示分配表徵圖** ![](assets/show-allocations-icon-small.png)，然後按一下 **更多功能表** ![](assets/qs-more-menu.png) > **編輯分配**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   或

   按兩下每日或每週分配，以修改用戶分配給工作項的時間量。

   有關在工作負載平衡器中修改用戶分配的資訊，請參閱文章中的「修改用戶分配」部分 [在工作負載平衡器中管理用戶分配](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   有關使用工作負載平衡器從工作項中刪除分配的資訊，請參見 [在工作負載平衡器中取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

