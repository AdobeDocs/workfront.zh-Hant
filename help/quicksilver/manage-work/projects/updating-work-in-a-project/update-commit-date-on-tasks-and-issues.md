---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任務和問題的認可日期
description: 您可以手動更新指派給您的任務或問題的認可日期。 如需Adobe Workfront中認可日期的詳細資訊，請參閱認可日期總覽。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---


# 更新任務和問題的認可日期

{{highlighted-preview}}

您可以手動更新指派給您的任務或問題的認可日期。 如需Adobe Workfront中認可日期的詳細資訊，請參閱 [認可日期總覽](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 存取需求

<!--Audited: 01/2024-->

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

您必須被指派給需要更新其認可日期的任務或問題，才能編輯任務或問題的認可日期。

## 更新任務和問題的認可日期


您可以在Workfront的下列區域中更新任務或問題的認可日期：

* 任務或問題的詳細資訊區段
* <span class="preview">任務或問題標題</span>

  <span class="preview">您的Workfront或群組管理員必須將認可日期新增到版面配置範本的任務或問題標題，以從任務或問題頁面檢視它。
如需詳細資訊，請參閱 [使用版面配置範本自訂物件標頭](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

更新認可日期對於任務和問題而言是相同的。

>[!NOTE]
>
>您可以要求系統或群組管理員將認可日期欄位新增到您的摘要面板，使其更易於在Workfront的各個區域更新。
>
>如需詳細資訊，請參閱下列文章：
>
>* [摘要概觀](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [使用版面配置範本自訂首頁和摘要](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. 前往指派給您的任務或問題 **所有者**.

   如需尋找問題或任務之任務負責人的詳細資訊，請參閱區段 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. <span class="preview">（有條件且選用）如果您的Workfront或群組管理員將認可日期新增到您的任務或問題標題，請按一下 **認可日期** 欄位，然後從日曆中選取日期。 如果「認可日期」不在標題中，請繼續下列步驟。 </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

1. 按一下 **任務詳細資訊** 或 **問題詳細資訊** 在左側面板中。
1. 按一下 **概觀** 以展開它。
1. 更新 **認可日期** 欄位。

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. 按一下「**儲存變更**」。

   進行此變更後，會發生下列情況：

   * 任務或問題的認可日期和計畫完成日期不再相同。

     相反，任務或問題的認可日期和預計完成日期變為相同。

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Workfront應用程式內通知會通知專案所有者，您已建議任務或問題的新認可日期。
   * 更新區段會通知專案所有者，您已建議新的認可日期，他們現在可以更新任務或問題的規劃完成日期，以符合您建議的認可日期。

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     如需關於此變更所觸發的通知和更新的資訊，請參閱文章中的「變更認可日期所觸發的通知和更新」一節 [認可日期總覽](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->