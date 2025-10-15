---
product-area: projects
navigation-topic: task-duration
title: 使用簡單期間型別更新任務的計畫時數和期間
description: 依預設，Adobe Workfront會根據計畫時數的數量，以簡單期間型別計算任務的期間。 不過，您也可以在Workfront的特定區域中手動編輯規劃時數與簡單期間任務的期間。
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# 使用簡單期間型別更新任務的計畫時數和期間

依預設，Adobe Workfront會根據計畫時數的數量，以簡單期間型別計算任務的期間。 不過，您也可以在Workfront的特定區域中手動編輯規劃時數與簡單期間任務的期間。

您可以內嵌或在「工作總攬」區域的任務層級編輯具有「簡單期間型別」之任務的計畫時數與期間。

如需有關內嵌編輯資訊的詳細資訊，請參閱[在Adobe Workfront中內嵌編輯清單中的專案](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)。

本文說明如何在任務層級的「工作總攬」區域中，以「簡單期間型別」更新任務的計畫時數與期間。

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
   <td><p>標準或更高</p> 
   <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視或更高專案存取權</p> <p>編輯任務的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理對任務的存取 </p></td> 
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
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 使用簡單期間型別更新任務的計畫時數和期間

>[!IMPORTANT]
>
>在您手動更新簡單期間任務上的期間後，Workfront會停止根據計畫時數計算期間。

若要在「進階工作總攬」方塊中使用「簡單期間型別」編輯任務的計畫時數與期間：

1. 在任務清單中，按一下您要變更持續時間型別的工作名稱。
1. 執行下列其中一項：

   * 按一下工作名稱旁的&#x200B;**更多**&#x200B;圖示![](assets/qs-more-icon-on-an-object.png)，按一下&#x200B;**編輯**，然後按一下&#x200B;**指派**。
   * 按一下指派給&#x200B;**的**&#x200B;或任務標題工作分派區域的名稱，然後按一下&#x200B;**進階**。

1. 為所有指派輸入&#x200B;**計畫時數**&#x200B;的總值，例如10小時。 計畫時數總計平均分配給指派給任務的所有資源。
1. （選擇性）手動調整指派給任務的每個資源的計畫時數。 任務更新的計畫時數總數，以反映個別指派給您資源的新時數。
1. 輸入工作&#x200B;**工期**&#x200B;的值，例如2天。

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 按一下「**儲存**」。
