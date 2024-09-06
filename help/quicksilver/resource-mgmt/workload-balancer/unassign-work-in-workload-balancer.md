---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中取消指派工作
description: 您可以在Adobe Workfront工作負載平衡器，將使用者從已指派工作區域的工作專案取消指派，或將他們重新指派給其他使用者、角色或團隊。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 196d0aa4ed67cf564c823625515ef49d811e0e06
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 2%

---

# 在工作負載平衡器中取消指派工作

您可以在Adobe Workfront工作負載平衡器，將使用者從已指派工作區域的工作專案取消指派，或將他們重新指派給其他使用者、角色或團隊。

您可以手動、拖放或大量解除工作專案的使用者指派。 本文會說明如何手動解除指派使用者。

如需透過拖放來取消指派使用者的資訊，請參閱[透過拖放在工作負載平衡器中指派工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

如需大量取消指派使用者的詳細資訊，請參閱[使用工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)大量指派工作。

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
       <p>目前：計畫，在資源區域使用工作負載平衡器時；</br>
       工作，使用團隊或專案的工作負載平衡器時</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li>資源管理</li> 
     <li>專案</li> 
     <li>任務</li> 
     <li>問題</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>Contribute許可權或以上至專案、任務和問題，包括進行指派</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作負載平衡器中取消指派工作專案

您可以從使用者取消指派專案，並將它們移動到「未指派的工作」區域，或重新指派給其他使用者。

若要取消指派使用者的工作專案，請執行下列動作：

1. 在工作負載平衡器中，移至&#x200B;**指派的工作**&#x200B;區域並展開使用者。
1. 執行下列其中一項：

   * 在使用者的區域中尋找您要取消指派的專案，按一下該專案，然後將其拖放至「已取消指派」區域或其他使用者的區域中。
   * 按一下工作專案名稱右側的&#x200B;**更多**&#x200B;圖示![](assets/more-icon-task-list.png)，按一下&#x200B;**將此指派給**，然後移除指派給工作專案的實體名稱或輸入其他名稱，然後按一下&#x200B;**儲存**。

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   如果專案符合該區域的篩選條件，且未指派給任何其他使用者，則會顯示在「未指派的工作」區域中；如果專案指派給其他使用者，則會顯示在使用者區域中。

   如需有關在工作負載平衡器中篩選資訊的資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)中的篩選資訊[。
