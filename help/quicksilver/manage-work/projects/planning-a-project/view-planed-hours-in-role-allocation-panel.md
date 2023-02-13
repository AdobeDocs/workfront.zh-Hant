---
product-area: projects
navigation-topic: plan-a-project
title: 在「角色分配」面板中查看項目計畫小時數
description: 您可以在項目的「角色分配」面板中查看分配給項目中工作項的所有作業角色的角色分配。
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 在「角色分配」面板中查看項目計畫小時數

您可以在項目的「角色分配」面板中查看分配給項目中工作項的所有作業角色的角色分配。

>[!NOTE]
>
>本文涉及在項目的「角色分配」面板中查看與項目任務和問題及其分配的「計畫小時數」相關的職務角色。 有關在使用Adobe Workfront方案計畫員時使用「職責分配」面板協調計畫小時數與方案小時數的資訊，請參閱：
>
>* [在任務清單中顯示項目和方案的角色分配](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [在工作負載平衡器中顯示項目和方案的角色分配](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  您必須擁有方案計畫員許可證，才能在「角色分配」面板中查看方案小時數。 有關方案計畫員的資訊，請參閱 [開始使用方案規劃器](../../../scenario-planner/get-started-with-scenario-planning.md) .

## 存取需求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

您必須具備下列條件：

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
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高權限存取專案</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須具備下列條件：

* 分配給作業角色或與作業角色關聯的用戶的任務或問題。

   >[!TIP]
   如果未分配任務或問題、分配給團隊或分配給沒有職務角色的用戶，則「職責分配」面板中項目的「計畫小時數」為零。

* 持續時間超過零的任務和問題。

## 在「角色分配」面板中查看項目計畫小時數

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **專案**.
1. 按一下專案的名稱以存取。 這會開啟「專案」頁面。
1. 在左側面板中按一下下列其中一項：

   * **任務**
   * **工作負載平衡器**

1. 按一下 **顯示角色分配** 圖示 ![](assets/show-role-allocation-icon.png).

   「角色分配」面板隨即顯示。

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. 請參閱 **角色分配** 面板： |欄位 |說明| |—|—| | **工作角色** |分配給項目上的任務和問題的作業角色。 這些角色可以是直接分配給任務和問題的作業角色，或與分配給項目任務和問題的用戶相關聯的作業角色。  | | **計畫小時數** |分配給任務角色或與項目上的任務角色相關聯的用戶的任務和問題的計畫小時總數。 |



