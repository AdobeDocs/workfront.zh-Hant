---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任務和問題的認可日期
description: 您可以手動更新指派給您的任務或問題的認可日期。 如需Adobe Workfront中認可日期的詳細資訊，請參閱認可日期總覽。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 更新任務和問題的認可日期

您可以手動更新指派給您的任務或問題的認可日期。 如需Adobe Workfront中認可日期的詳細資訊，請參閱 [認可日期總覽](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 存取需求

<!--Audited: 01/2024-->

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
   <td> 
   對於新授權：
   <ul>
   <li><p>任務的標準</p> </li>
   <li><p>問題的貢獻者或以上版本</p></li>
   </ul>
   對於目前的授權：
<ul>
   <li><p>工作或更高的任務</p></li> 
   <li><p>要求或更高版本的問題</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務和問題的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務或問題的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先決條件

開始之前，您必須被指派給需要更新認可日期的任務或問題。

## 更新任務和問題的認可日期

更新認可日期對於任務和問題而言是相同的。

1. 前往指派給您的任務或問題 **所有者**.

   如需尋找問題或任務之任務負責人的詳細資訊，請參閱區段 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. 按一下 **任務詳細資訊** 或 **問題詳細資訊** 在左側面板中。
1. 按一下 **概觀** 以展開它。
1. 更新 **認可日期** 欄位。

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. 按一下「**儲存變更**」。

   進行此變更後，會發生下列情況： 

   * 任務或問題的認可日期和計畫完成日期不再相同。

     相反，任務或問題的認可日期和預計完成日期變為相同。

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * 如果您使用舊版更新區域，則會通知專案所有者，您已為任務或問題建議新的認可日期，並且此時可以更新任務或問題的規劃完成日期，以符合您建議的認可日期。 新的評論體驗不支援此功能。 如需詳細資訊，請參閱 [新的評論體驗](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     如需此變更所觸發之通知和更新的相關資訊，請參閱區段 [變更認可日期所觸發的通知和更新](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) 在文章中 [認可日期總覽](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
