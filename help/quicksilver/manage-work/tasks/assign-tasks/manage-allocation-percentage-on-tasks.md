---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任務的使用者或角色配置百分比
description: 配置百分比代表指定資源計畫在一天內處理一項任務的時間量。 這是在任務持續期間中配置資源的當日百分比（根據使用者或專案排程）。
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 管理任務的使用者或角色配置百分比

配置百分比代表指定資源計畫在一天內處理一項任務的時間量。 這是在任務持續期間中配置資源的當日百分比（根據使用者或專案排程）。

>[!NOTE]
>
>指派使用者工作時，其根據排程的可用性會影響任務和問題的計畫和預計日期。 如需排程的相關資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p> 
   <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>貢獻或更高的任務許可權</p> <p>編輯許可權以更新在編輯任務方塊中的分配百分比</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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

   ![修改配置百分比](assets/advanced-assignments-allocation-percentage.png)

1. 按一下「**儲存**」。
