---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 透過拖放在工作負載平衡器中指派工作
description: 您可以透過拖放工作專案給正確的使用者，使用Adobe Workfront工作負載平衡器指派工作專案。
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# 透過拖放在工作負載平衡器中指派工作

您可以透過拖放工作專案給正確的使用者，使用Adobe Workfront工作負載平衡器指派工作專案。

如需使用工作負載平衡器指派工作給使用者的一般資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中指派工作的總覽。[

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫，以指派資源區域中的工作負載平衡器中的工作；</br>
       工作，指派團隊或專案的工作負載平衡器工作</p></td>
  </tr>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li>資源管理</li> 
     <li>專案</li> 
     <li>任務</li> 
     <li>問題</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>Contribute許可權或以上至專案、任務和問題，包括進行指派</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 透過拖放方式指派專案

您可以從「未指派的工作」區域指派專案給使用者，也可以在「已指派的工作」區域將已指派的專案重新指派給其他使用者。

1. 前往您要指派工作的工作負載平衡器。

   您可以使用資源區域、專案或團隊層級的工作負載平衡器將工作指派給使用者。 如需有關工作負載平衡器在Workfront中的位置的詳細資訊，請參閱[找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

1. （選擇性）移至&#x200B;**未指派的工作**&#x200B;區域並套用篩選器以檢視未指派給使用者的任務和問題

   或

   移至&#x200B;**指派的工作**&#x200B;區域，並展開使用者的名稱以檢視指派給他們的工作專案（如果您要重新指派其專案）。

1. （視條件而定）在專案的工作負載平衡器中，按一下&#x200B;**顯示所有使用者**&#x200B;圖示![](assets/show-all-users-icon-project-workload-balancer.png)以顯示所有Workfront使用者。

   這會顯示您有權檢視的所有使用者。

   同時身為專案團隊成員且已指派至專案中專案的使用者，其名稱右側的「指派的工作」區域會顯示專案圖示。

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* 顯示所有使用者選項僅在專案的工作負載平衡器中可用。
   >* 使用篩選器只顯示對您重要的使用者。 例如，使用篩選器以僅顯示您團隊或群組中的使用者。



1. 按一下表示計畫或預計時間表的工作專案列，並將其拖曳至&#x200B;**已指派**&#x200B;區域中的使用者名稱上。

   將滑鼠懸停在上方以將工作專案放置到的使用者會醒目提示。

   >[!TIP]
   >
   >您暫留在工作專案上之使用者的計畫時數會即時更新其每日計畫時數，以指出新增專案對其整體配置可能產生的影響。

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. 準備就緒後，將所選工作專案拖放到與指派區域中的使用者名稱相同的行中。 專案已指派，而已分配的「計畫時數」已針對具有工作專案新時數的使用者更新。

   如果專案被指派給使用者無法完成的工作角色，該專案會顯示在「已指派的工作」區域中使用者名稱之下，並且還會留在「未指派的工作」區域中，以表示與其關聯的工作角色尚未被使用者取代。

   >[!TIP]
   >
   >* 如果您在設定區域中啟用了「依專案分組」 ，則指派的任務會顯示在對應的專案下。 如果停用此設定，則指派的任務會顯示在使用者區域中。
   >
   >
   >     專案會根據工作負載平衡器條件顯示以排序工作專案。 如需詳細資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。
   >
   >
   >* 如果您啟用了在工作負載平衡器顯示專案的所有使用者，並將專案指派給之前未指派給專案專案的使用者，則該使用者會新增到專案團隊。 如需詳細資訊，請參閱[管理專案團隊](../../manage-work/projects/planning-a-project/manage-project-team.md)。


1. （選擇性）按一下已指派工作區域中的使用者名稱下的工作專案列，然後將其拖放到未指派工作區域上以取消指派。 使用者會取消指派此專案，但該專案可能仍會指派給工作角色，若是如此，該專案會顯示在「未指派的工作」區域中。 如果專案被指派給其他使用者，該專案會保留在「已指派工作」區域中，位於仍被指派的使用者名稱下。
1. （選擇性）按一下&#x200B;**顯示配置圖示** ![](assets/show-allocations-icon-small.png)，然後按一下&#x200B;**更多功能表** ![](assets/qs-more-menu.png) > **編輯配置**。

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   或

   按兩下每日或每週配置，以修改將使用者配置給工作專案的時間量。

   如需有關在工作負載平衡器中修改使用者配置的資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理使用者配置一文[中的「修改使用者配置」一節。

   如需有關使用工作負載平衡器從工作專案移除指派的資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md)中取消指派工作。[

