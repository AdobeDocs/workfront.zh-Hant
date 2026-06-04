---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中取消指派工作
description: 您可以在Adobe Workfront工作負載平衡器，將使用者從已指派工作區域的工作專案取消指派，或將他們重新指派給其他使用者、角色或團隊。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
TQID: https://experienceleague.adobe.com/AREKzNODjF60azs3tXIndVE9QuXXw-14Qlv2nUl9Po4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 382
ht-degree: 7%

---

# 在工作負載平衡器中取消指派工作

您可以在Adobe Workfront工作負載平衡器，將使用者從已指派工作區域的工作專案取消指派，或將他們重新指派給其他使用者、角色或團隊。

您可以手動、拖放或大量解除工作專案的使用者指派。 本文會說明如何手動解除指派使用者。

如需透過拖放來取消指派使用者的資訊，請參閱[透過拖放在工作負載平衡器中指派工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

如需大量取消指派使用者的詳細資訊，請參閱[使用工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)大量指派工作。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>計畫：在資源區域使用工作負載平衡器；工作，使用團隊或專案的工作負載平衡器</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li>資源管理</li> 
     <li>專案</li> 
     <li>任務</li> 
     <li>問題</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>包含進行指派的專案、任務和問題的貢獻許可權或更高</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作負載平衡器中取消指派工作專案

您可以從使用者取消指派專案，並將它們移動到「未指派的工作」區域，或重新指派給其他使用者。

若要取消指派使用者的工作專案，請執行下列動作：

1. 在工作負載平衡器中，移至&#x200B;**指派的工作**&#x200B;區域並展開使用者。
1. 執行下列其中一項：

   * 在使用者的區域中尋找您要取消指派的專案，按一下該專案，然後將其拖放至「已取消指派」區域或其他使用者的區域中。
   * 按一下工作專案名稱右側的&#x200B;**更多**&#x200B;圖示![更多圖示](assets/more-icon-task-list.png)，按一下&#x200B;**將此指派給**，然後移除指派給工作專案的實體名稱或輸入其他名稱，然後按一下&#x200B;**儲存**。

     ![將此指派給](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   如果專案符合該區域的篩選條件，且未指派給任何其他使用者，則會顯示在「未指派的工作」區域中；如果專案指派給其他使用者，則會顯示在使用者區域中。

   如需有關在工作負載平衡器中篩選資訊的資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)中的篩選資訊[。
