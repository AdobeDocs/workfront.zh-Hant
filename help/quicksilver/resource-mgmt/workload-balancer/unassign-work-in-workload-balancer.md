---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中取消指派工作
description: 您可以在Adobe Workfront工作負載平衡器，將使用者從已指派工作區域的工作專案取消指派，或將他們重新指派給其他使用者、角色或團隊。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# 在工作負載平衡器中取消指派工作

您可以在Adobe Workfront工作負載平衡器，將使用者從已指派工作區域的工作專案取消指派，或將他們重新指派給其他使用者、角色或團隊。

您可以手動、拖放或大量解除工作專案的使用者指派。 本文會說明如何手動解除指派使用者。

如需透過拖放來取消指定使用者的資訊，請參閱 [透過拖放在工作負載平衡器中指派工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

如需大量取消指派使用者的詳細資訊，請參閱 [使用工作負載平衡器大量指派工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>計畫，在資源區域使用工作負載平衡器</p>
   <p>工作，使用團隊或專案的工作負載平衡器時</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何變更您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>包含進行指派的專案、任務和問題的貢獻許可權或更高</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

 

## 在工作負載平衡器中取消指派工作專案

您可以從使用者取消指派專案，並將它們移動到「未指派的工作」區域，或重新指派給其他使用者。

若要取消指派使用者的工作專案，請執行下列動作：

1. 在工作負載平衡器，前往 **已指派的工作** 區域並展開使用者。
1. 執行下列其中一項：

   * 在使用者的區域中尋找您要取消指派的專案，按一下該專案，然後將其拖放至「已取消指派」區域或其他使用者的區域中。
   * 按一下 **更多** 圖示 ![](assets/more-icon-task-list.png) 在工作專案名稱的右側，按一下 **將此指派至**，然後移除指派給工作專案的實體名稱，或輸入其他名稱，然後按一下 **儲存**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   如果專案符合該區域的篩選條件，且未指派給任何其他使用者，則會顯示在「未指派的工作」區域中；如果專案指派給其他使用者，則會顯示在使用者區域中。

   如需有關在工作負載平衡器篩選資訊，請參閱 [在工作負載平衡器中篩選資訊](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
