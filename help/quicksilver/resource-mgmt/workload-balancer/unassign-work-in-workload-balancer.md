---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作負載平衡器中取消分配工作
description: 您可以在Adobe Workfront Workload Balancer的「已分配的工作」區域中從工作項取消分配用戶，或將它們重新分配給其他用戶、角色或團隊。
author: Alina
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 2%

---

# 在工作負載平衡器中取消分配工作

您可以在Adobe Workfront Workload Balancer的「已分配的工作」區域中從工作項取消分配用戶，或將它們重新分配給其他用戶、角色或團隊。

您可以透過拖放或大量手動取消指派工作項目中的使用者。 本文說明如何手動取消指派使用者。

如需透過拖放方式取消指派使用者的資訊，請參閱 [通過拖放來分配工作負載平衡器中的工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

如需大量取消指派使用者的詳細資訊，請參閱 [使用工作負載平衡器批量分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對以下項目的存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>將權限或更高版本貢獻給包括「進行分配」的項目、任務和問題</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

 

## 在工作負載平衡器中取消分配工作項

您可以從用戶中取消分配項目並將其移到「未分配的工作」區域，或將其重新分配給其他用戶。

要從用戶取消分配工作項：

1. 在工作負載平衡器中，轉到 **已分配的工作** 區域和展開使用者。
1. 執行下列任一項作業：

   * 在用戶區域中查找要取消分配的項，按一下該項，然後將其拖放到「未分配」區域或其他用戶區域中。
   * 按一下 **更多** 圖示 ![](assets/more-icon-task-list.png) 在工作項名稱的右側，按一下 **將此項指派給**，然後刪除分配給工作項的實體的名稱或輸入其他名稱，然後按一下 **儲存**.

      ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)
   如果項目與該區域的篩選條件匹配，並且未分配給任何其他用戶，則該項目將顯示在「未分配的工作」區域中；如果項目被分配給其他用戶，該項目則顯示在用戶區域中。

   有關在工作負載平衡器中篩選資訊的資訊，請參見 [篩選工作負載平衡器中的資訊](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
