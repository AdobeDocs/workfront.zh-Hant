---
product-area: projects
navigation-topic: task-information
title: 更新任務平準延遲
description: 有時候，專案上的任務排程之間可能會發生衝突。 您可以重新排程資源與工作，讓所有工作都能在現實的排程內完成，以平準資源或解決資源衝突。 如需有關平準任務的資訊，請參閱甘特圖中的平準資源。
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 3%

---

# 更新任務平準延遲

有時候，專案上的任務排程之間可能會發生衝突。 您可以重新排程資源與工作，讓所有工作都能在現實的排程內完成，以平準資源或解決資源衝突。 如需有關平準工作的資訊，請參閱[甘特圖中的平準資源](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md)。

身為專案經理或任務受指派人，您也可以在個別任務上新增「平準延遲」，以說明任何資源或排程衝突。 換言之，一項任務可能會延遲排程，以確保Adobe Workfront在排程任務時能以更實際的排程克服資源衝突。

將平準延遲新增至任務會調整任務的「預計完成日期」。 如需有關預計完成日期的資訊，請參閱[專案、任務和問題的預計完成日期總覽](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權 </p> <p>貢獻或更高的專案許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to Tasks </p> <p>Contribute or higher permissions to Projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 將平準延遲新增至任務

1. 移至您要為其新增「平準延遲」的工作。
1. 按一下工作名稱右側的&#x200B;**更多圖示**，然後按一下&#x200B;**編輯**。

1. 按一下&#x200B;**設定**。

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. 指定&#x200B;**平準延遲** （以小時為單位），然後選擇時間單位。\
   這是資源因資源衝突而延遲啟動工作的時間。

   從下列時間單位選項中選取：

   * 分鐘
   * 小時。 這是預設值。
   * 日
   * 週
   * 月
   * 經過的分鐘數
   * 經過的時數
   * 經過的天數
   * 經過的週數
   * 經過的月數

   >[!TIP]
   >
   >經過的時間是任務期間的時間單位。 這是任務的計劃開始日期與計畫完成日期之間的時間，包括假日、週末和休假。 換句話說，經過的時間就是行事曆的天數。

1. 按一下&#x200B;**儲存**。 

 
