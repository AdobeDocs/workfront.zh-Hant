---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任務的使用者或角色配置百分比
description: 配置百分比代表指定資源計畫在一天內處理一項任務的時間量。 這是在任務持續期間中配置資源的當日百分比（根據使用者或專案排程）。
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# 管理任務的使用者或角色配置百分比

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽」環境中供所有客戶使用，或在「生產」環境中供啟用快速發行的客戶使用。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<span class="preview">如需目前版本的相關資訊，請參閱[2024年第三季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md)。</span>

配置百分比代表指定資源計畫在一天內處理一項任務的時間量。 這是在任務持續期間中配置資源的當日百分比（根據使用者或專案排程）。

>[!NOTE]
>
>指派使用者工作時，其根據排程的可用性會影響任務和問題的計畫和預計日期。 如需排程的相關資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

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
   <td> <p>編輯任務的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>Contribute或更高的任務許可權</p> <p>編輯許可權以更新在編輯任務方塊中的分配百分比</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 修改任務百分比分配的考量事項

* 依預設，使用者會獲得相等百分比的時間分配給指派給他們的任務。
* 只有在任務的「期間型別」是已計算的工作或投入比導向時，您才能手動修改指派給任務的使用者與工作角色的分配百分比。

  如需詳細資訊，請參閱[任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

* 您無法修改指派給任務的團隊的百分比配置。
* 您無法修改指派給問題的使用者和職位角色的百分比分配。

## 修改任務的使用者或角色百分比分配

1. 移至您要變更其資源配置百分比的任務。
1. 按一下工作名稱旁的&#x200B;**更多**&#x200B;功能表![](assets/qs-more-icon-on-an-object.png)，然後按一下&#x200B;**編輯**。

   或

   按一下工作標題中的&#x200B;**工作總攬**&#x200B;區域，然後按一下&#x200B;**進階**。

1. 確定任務的&#x200B;**期間型別**&#x200B;是下列其中一項：

   * 已計算的工作
   * 投入比導向

   >[!TIP]
   >
   >* 對於計算的指派期間型別，Workfront會使用以下公式來計算每個受指派人的配置百分比： `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`。
   >* 對於「簡單期間型態」，您可以估計指派給每項資源的時數，而非配置百分比。

1. 按一下&#x200B;**工作分派**，然後修改每個工作受指派人的&#x200B;**分派**。

   您只能修改使用者與職務角色指派的配置百分比。

   您無法修改指派給任務的團隊配置百分比。

   生產環境中的影像範例：
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">預覽環境中的範例影像：</span>
   ![修改配置百分比](assets/advanced-assignments-allocation-percentage.png)

1. 按一下「**儲存**」。
