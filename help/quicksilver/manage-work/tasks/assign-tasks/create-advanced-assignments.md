---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 建立高級分配
description: 您可以使用「高級分配」來管理任務或發放分配。
author: Alina
feature: Work Management
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# 建立高級分配

您可以使用「高級分配」來管理任務或發放分配。

在進行高級分配時，您可以調整以下分配資訊：

* 將用戶分配給任務或問題（這可在高級分配之外完成）。
* 調整並重新分配每個受託人分配的小時數。
* 確定應將哪個用戶指定為任務或問題的所有者或主要受託人。
* 指定每個用戶在處理任務或問題時正在履行的角色。

>[!NOTE]
>
>在將用戶分配到工作時，根據其計畫提供的可用性會影響任務和問題的計畫日期和預計日期。 如需排程的相關資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Adobe Workfront中您可以進行進階指派的區域

本文介紹如何訪問任務或問題題頭中的「預先分配」。

此外，您還可以在Workfront的以下區域執行進階指派：

* 在清單和報表中，當「工作總攬」欄位顯示在視圖中時。
* 編輯任務時在「工作總攬」部分中。 如需詳細資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 在任務或問題題頭的「工作總攬」區域中。
* 在工作負載平衡器中。 如需詳細資訊，請參閱 [使用工作負載平衡器手動分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和問題的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為任務或問題貢獻或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 進行高級分配

1. 轉到要分配任務或問題的項目。
1. 按一下 **工作** 或 **問題** 在左側面板中，按一下清單中的任務或問題名稱。

   >[!TIP]
   >
   >如果分配了兩個或多個人員，則可以直接在任務或問題清單上進行高級分配。 按一下內部 **分配** 欄位，然後按一下 **人員表徵圖** 開啟「高級分配」窗口。 跳到步驟5以繼續建立高級分配。\
   >![](assets/nwe-advanced-assignments-350x55.png)   >

1. 按一下 **指派給** 在 **分配** 欄位（在任務或問題的標題中）

   或

   如果已分配任務或問題，請按一下分配的名稱。

1. 按一下 **進階**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 在 **搜索人員、角色和團隊** 欄位中，開始鍵入用戶、角色或團隊的名稱，然後在名稱出現在下拉清單中時按一下該名稱。

   >[!NOTE]
   >
   >如果用戶名包含特殊字元，則必須在搜索欄位中包含特殊字元。

1. （可選）繼續在 **搜索人員、角色或團隊** 框，向任務或問題添加多個資源。

   >[!TIP]
   >
   >* 您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >
   >* 新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。
   >
   >
   >* 如果在停用前已指派使用者、工作角色或團隊，則他們仍會指派給工作項目。 在此情況下，我們建議：
      >   
      >   * 將工作項重新分配給活動資源。
      >   * 將已停用團隊中的用戶與活動團隊關聯，並將工作項重新分配給活動團隊。


1. 針對 **受託人** 欄，指定下列資訊：


   * **擁有者**:將滑鼠指標暫留在受託人的名稱上，然後按一下 **設為主要** （在「責任人」欄位中）。 綠色複選框表示指定的用戶是任務或問題的主要聯繫人。 Adobe Workfront會將您指派給任務或問題的第一個使用者或工作角色標示為「擁有者」或「主要指派」。 不能將團隊指定為任務或問題的主要所有者。

      >[!IMPORTANT]
      >
      >根據您的Workfront管理員或組管理員如何設定項目首選項，Workfront可能會使用任務所有者的計畫來計算分配給任務的多個用戶時的任務時間線。 有關多個任務分配者的資訊，請參閱文章中的「為任務分配多個用戶」部分 [指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **分配** :當任務的「持續時間類型」為「簡單」時，請指定每個用戶或作業角色應分配給該任務的小時數。 每個使用者的所有指派小時數總和等於 **計畫小時數** 欄位。 在所有其他情況下，指定您希望受託人花費在解決任務或問題上的時間（或分配）百分比。

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

      >[!TIP]
      >
      >
      >   
      >   
      >   * 手動修改任務的分配分配後，任務的「計畫時數」可能會相應更新。 有關詳細資訊，請參閱文章中的「在管理用戶分配時更新任務計畫小時數」部分 [計畫小時數概觀](../../../manage-work/tasks/task-information/planned-hours.md).
      >   * 您不能手動修改問題上的分配分配。
      >   * 不能手動修改分配給任務的團隊的分配。


   * **受託人的角色：** 選擇用戶在完成此分配時應使用的角色。  預設會顯示使用者的主要角色。 按一下「受託人的角色」(Assignee&#39;s Role)框中的以選擇其他角色。  當您先將任務或問題分配給某個角色，然後添加可以履行該角色的用戶作為第二個分配時，系統會為那些能夠履行已分配給該任務和問題的角色的用戶篩選建議用戶清單。

      ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   * **持續時間類型**:這僅適用於任務。 按一下「持續時間類型」的名稱，然後從下拉式選單中選取「持續時間類型」。 如需持續時間類型的相關資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **持續時間：** 當您具有任務的「管理」權限時，可以更新該任務的此欄位。

      如需詳細資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 在批量編輯分配資訊時，將出現一個類似的對話框來分配用戶、小時數、分配和任務所有者。

   * **計畫小時數**:當「期間類型」為「計算分配」或「簡單」時，請更新「計畫小時數」。 每個資源的分配百分比或小時數因此平均分配。 Workfront會在計算「工作」或「工作」時計算「計畫小時數」。 如需詳細資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

      ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. 按一下&#x200B;**儲存**。
