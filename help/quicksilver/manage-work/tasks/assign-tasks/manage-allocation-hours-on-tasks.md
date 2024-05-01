---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任務的使用者和角色分配時數
description: 將使用者或角色指派給任務時，會為其分配特定時數的工作以完成任務。 當任務「期間型別」為「簡單」時，您可以手動修改指派給任務的每個使用者或工作角色的時數。
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: ad5d6bfda24119076df8336ed291c0ba63e2c88a
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# 管理任務的使用者和角色分配時數

{{highlighted-preview}}

將使用者或角色指派給任務時，會為其分配特定時數的工作以完成任務。 當任務「期間型別」為「簡單」時，您可以手動修改指派給任務的每個使用者或工作角色的時數。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>貢獻或更高的任務許可權</p> <p>編輯許可權以在編輯任務方塊中更新分配時數</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 修改任務分配時數的考量事項

>[!IMPORTANT]
>
>在您手動修改任務上每個指派的分配後，任務的計畫時數可能會相應地更新。 如需詳細資訊，請參閱區段 [管理使用者分派時更新任務計畫時數](../../../manage-work/tasks/task-information/planned-hours.md#update) 在文章中 [計畫時數概觀](../../../manage-work/tasks/task-information/planned-hours.md).

* 分配給指派給任務的個別資源的時數總計代表任務的計畫時數。
* 如果任務有一個使用者或角色指派，則分配給使用者或角色的時數與任務的計畫時數相符。
* 在多重指派的情況下，如果任務「期間型別」為「簡單」，則預設會為每個使用者或工作角色指派相等的時數，以處理任務。 如需詳細資訊，請參閱下列文章：

   * [任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [期間型別概觀：簡單](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 當任務具有「簡單期間型別」時，您可以手動變更每個使用者或職務角色的分配時數金額，以表示某些任務受指派人可能比其他任務受指派人有更多時間處理任務。
* 您無法修改分配給指派給任務的團隊的時數。
* 您無法手動修改問題的使用者或工作角色分配。
* 您還可以使用工作負載平衡器管理每日、每週或每月使用者對任務或問題的分配。 如需詳細資訊，請參閱 [在工作負載平衡器中管理使用者配置](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 修改任務的使用者或角色配置時數

1. 移至您要變更其指派時數的任務。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) 在任務名稱旁，然後按一下 **編輯**，然後 **指定任務**.

   或

   按一下 **指定任務** 區域，然後按一下 **進階**.

1. 確保 **期間型別** 任務的 **簡單**.
1. 修改 **配置** 適用於每個任務受指派人。 這些是整個任務期間此任務的每個工作分派的整體配置。 這也可能更新任務的整體計畫時數。

   生產環境中的影像範例：
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">預覽環境中的範例影像：</span>
   ![修改配置](assets/advanced-assignments-duration-type-allocations.png)

1. 按一下「**儲存**」。
