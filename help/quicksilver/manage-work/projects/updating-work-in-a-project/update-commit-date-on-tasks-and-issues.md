---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任務和問題的提交日期
description: 您可以手動更新任務或分配給您的問題的提交日期。 有關Adobe Workfront中「提交日期」的詳細資訊，請參閱「提交日期」概述。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 更新任務和問題的提交日期

您可以手動更新任務或分配給您的問題的提交日期。 如需Adobe Workfront中「提交日期」的詳細資訊，請參閱 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 存取需求

<!--drafted for P&P

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
   <td> 
   For the current licenses:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   For legacy licenses:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>工作或更高</p> 
   <p>請求或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和問題的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務或問題的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

在開始之前，必須將您分配給任務或需要更新的提交日期的問題。

## 更新任務和問題的提交日期

對於任務和問題，更新提交日期相同。

1. 轉至您被指派為 **任務所有者**.

   有關查找問題或任務的任務所有者的詳細資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. 按一下任務或問題標題中的「工作」

   或

   按一下 **啟動任務** 或 **開始問題** 如果已在您的環境中自定義「工作」按鈕，以表示您現在正在處理工作項。

   此時，任務或問題的提交日期和計畫完成日期相同。

1. （可選）如果按一下「開始任務」或「開始問題」，請按一下 **還原** 在畫面的左下角。 刪除提交日期。

   有關用「開始」按鈕替換「工作在It」按鈕的資訊，請參閱  [將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

   >[!TIP]
   >
   >按一下「 」後，無法使用還原您的選擇以開始工作的選項 **努力**.

1. 按一下 **更新** 在左側面板中，按一下 **開始新更新** >**提交日期**

   或

   按一下 **任務詳細資訊** 或 **問題詳細資訊** 在左側面板中，按兩下 **提交日期** 從日曆中選取新日期，然後按一下 **儲存變更**.
   ![](assets/commit-date-calendar-picker-in-updates-stream-nwe-350x452.png)

   進行此變更後，會發生下列事項： 

   * 提交日期和計畫完成日期不再相同。

      相反，任務或問題的「提交日期」和「預計完成日期」是相同的。

      ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * 從「更新」(Updates)區域選擇新日期時，將自動保存更改。
   * 項目所有者會收到通知，您已為任務或問題建議了新的提交日期，此時可以更新任務或問題的計畫完成日期，以符合您建議的提交日期。

      ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

      如需此變更所觸發的通知和更新的相關資訊，請參閱區段 [通過更改提交日期觸發的通知和更新](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) 在文章中 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
