---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任務上的用戶或角色分配百分比
description: 分配百分比表示分配的資源計畫在一天內處理任務的時間量。 它是在整個任務期間分配資源的工作日百分比（根據用戶或項目計畫）。
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# 管理任務上的用戶或角色分配百分比

分配百分比表示分配的資源計畫在一天內處理任務的時間量。 它是在整個任務期間分配資源的工作日百分比（根據用戶或項目計畫）。

>[!NOTE]
>
>在將用戶分配到工作時，根據其計畫提供的可用性會影響任務和問題的計畫日期和預計日期。 如需排程的相關資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>編輯對任務的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為任務貢獻或更高權限</p> <p>編輯權限以在「編輯任務」框中更新分配百分比</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 有關修改任務百分比分配的考量

* 依預設，系統會為指派給使用者的任務分配相同的時間百分比。
* 只有當任務的「持續時間類型」為「計算工作」或「工作驅動」時，您才能手動修改分配給任務的用戶和任務角色的分配百分比。

   如需詳細資訊，請參閱 [任務持續時間和持續時間類型概覽](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* 不能修改分配給任務的團隊的百分比分配。
* 無法修改分配給問題的用戶和作業角色的百分比分配。

## 修改任務的用戶或角色百分比分配

1. 轉到要更改百分比分配的資源的任務。
1. 按一下 **更多** 功能表 ![](assets/qs-more-icon-on-an-object.png) 在任務名稱旁，按一下 **編輯**.

   或

   按一下 **分配** 區域，然後按一下 **進階**.

1. 確保 **持續時間類型** 任務的以下內容之一：

   * 已計算的工作
   * 投入比導向

   >[!TIP]
   >
   >* 對於「計算的分配持續期間類型」，Workfront使用以下公式計算每個受託人的分配百分比： `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* 對於「簡單持續時間類型」，您可以估計分配給每個資源的小時數，而不是分配百分比。


1. 按一下 **分配**，然後修改 **分配** 每個任務受託人。

   您只能修改用戶和職務角色分配的分配百分比。

   不能修改分配給任務的組的分配百分比。

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. 按一下&#x200B;**儲存**。
