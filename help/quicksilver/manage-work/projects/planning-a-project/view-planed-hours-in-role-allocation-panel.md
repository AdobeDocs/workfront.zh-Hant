---
product-area: projects
navigation-topic: plan-a-project
title: 在角色分配面板中檢視專案計畫時數
description: 您可以在專案的「角色配置」面板中，檢視指派給專案中工作專案的所有職務角色的角色配置。
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 1%

---

# 在角色分配面板中檢視專案計畫時數

您可以在專案的「角色配置」面板中，檢視指派給專案中工作專案的所有職務角色的角色配置。

>[!NOTE]
>
>本文指的是檢視與專案上任務和問題相關的工作角色，及其在專案角色配置面板中的已配置計畫時數。 如需有關使用Adobe Workfront Scenario Planner時使用角色配置面板來協調計畫時數與方案時數的資訊，請參閱下列內容：
>
>* [顯示工作清單中專案和方案的角色分配](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [在工作負載平衡器](../../../scenario-planner/show-role-allocation-workload-balancer.md)中顯示專案和方案的角色分配
>
>  您必須有Scenario Planner授權，才能在「角色配置」面板中檢視方案時數。 如需Scenario Planner的相關資訊，請參閱[開始使用Scenario Planner](../../../scenario-planner/get-started-with-scenario-planning.md) 。
>

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
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視或更高專案存取權</p> <p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或更高的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

您必須具備下列條件：

* 指派給工作角色或與工作角色相關聯之使用者的任務或問題。

  >[!TIP]
  >
  >如果任務或問題被取消指派、指派給團隊或指派給沒有工作角色的使用者，則專案的「角色分配」面板中的計畫時數為零。

* 持續時間大於零的任務和問題。

## 在角色分配面板中檢視專案計畫時數

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**專案**。
1. 按一下專案名稱以存取。 如此將可開啟「專案」頁面。
1. 在左側面板中按一下下列其中一項：

   * **任務**
   * **工作量平衡工具**

1. 按一下&#x200B;**顯示角色配置**&#x200B;圖示![](assets/show-role-allocation-icon.png)。

   「角色配置」面板隨即顯示。

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. 檢閱&#x200B;**角色配置**&#x200B;面板中的下列資訊：

   | 欄位 | 說明 |
   |---|---|
   | **工作角色** | 指派給專案任務和問題的職位角色。 這些可以是直接指派給任務和問題的工作角色，或與指派給專案任務和問題的使用者相關聯的工作角色。 |
   | **規劃時數** | 從指派給工作角色或與專案工作角色相關聯之使用者的任務和問題所花費的總時數。 |

