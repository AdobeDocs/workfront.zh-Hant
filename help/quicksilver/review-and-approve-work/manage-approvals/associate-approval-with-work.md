---
product-area: projects
navigation-topic: approvals
title: 將新審批流程或現有審批流程與工作關聯
description: 本文說明如何將審批流程與工作項目關聯。 有關將批准與校樣或文檔關聯的資訊，請參閱以下文章。
author: Courtney and Alina
feature: Work Management
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 7dbb9ca9b26f17710a7897e98dca109b5c886bd7
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# 將新審批流程或現有審批流程與工作關聯

本文說明如何將審批流程與工作項目關聯。 有關將批准與校樣或文檔關聯的資訊，請參閱以下文章：

* [使用自動化工作流程建立進階校樣](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [請求文檔批准](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

您可以將全域或一次性使用的核准流程與Adobe Workfront中的工作項目建立關聯。 存在下列情況：

* 將現有全局審批流程與項目、任務、問題、模板或模板任務關聯。 系統中的所有群組都可以使用某些全域核准程式。 群組層級的全域核准程式僅適用於特定群組。
* 建立一次性審批流程，並將其與現有項目、任務、問題、模板或模板任務關聯。

>[!NOTE]
>
>本文使用「全域核准程式」一詞，來區分「單一使用核准程式」。 可重複使用全域核准程式。
>
>「組級全局審批流程」一詞是指可重複用於項目且狀態僅與特定組關聯的審批流程。

如需核准程式的更一般資訊，請參閱 [核准流程概述](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

如需建立全域核准程式的相關資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯對項目、任務、問題或模板的訪問權限或更高權限</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理對項目、任務、問題或模板的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 關於將審批流程與工作項關聯的注意事項

除了下述考量事項外，我們建議您重新審視Workfront中核准程式的一般考量事項。 如需詳細資訊，請參閱 [核准流程概述](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* 您必須先建立項目、任務、問題、模板或模板任務，然後審批流程才能與它們關聯。
* 當您將審批流程附加至某個已傳遞且該項目當前為狀態的項目時，將不觸發審批流程，並且不會向審批人發送任何通知。

   **範例：** 如果任務處於「完成」狀態，並且您附加了與「完成」狀態關聯的審批流程，則不會觸發審批。

* 將審批流程附加到項目的第一個狀態時（通過使用任務和項目的模板，使用問題的「隊列設定」設定，或為新任務定義項目的「任務設定」），如果重新調用提交的審批，則會跳過審批流程。 在這種情況下，批准者不會接收任何通知。

   有關回調批准的詳細資訊，請參閱 [查看批准](../../review-and-approve-work/manage-approvals/view-approvals.md).

   >[!TIP]
   >
   >任務或問題的第一個狀態為「新建」。 專案的第一個狀態是您的Workfront管理員在系統的「專案偏好設定」中選取的狀態。 如需詳細資訊，請參閱 [配置系統範圍的項目首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 批准進程與對象的關聯不會記錄在對象的「更新」區域中。
* 您不能將審批流程與父任務關聯。
* 將使用者、團隊或角色新增為核准者時，不會自動將權限授予與該核准相關聯的物件。 觸發核准步驟時，使用者會收到物件的權限。 否則，必須先與對象共用，才能做出批准決策。

以下各節介紹將審批流程與項目、任務或問題關聯的不同方法。

## 將全局審批流程與工作項關聯 {#associate-a-global-approval-process-with-a-work-item}

您可以將全局審批流程與工作項（項目、任務、問題、模板、模板任務）關聯。

與工作項關聯的組或系統中的所有組必須可以使用全局審批流程。

>[!NOTE]
您可以將項目批准流程附加到模板，並將任務批准流程附加到模板任務。 執行此操作後，當某人使用模板建立項目時，審批流程將分別變成項目或任務審批流程。 附加到模板或模板任務的一次性審批流程仍然是項目和任務的一次性審批流程。

如需Workfront管理員如何為系統中的所有群組設定全域核准程式，以及群組管理員如何為群組建立核准程式的相關資訊，請參閱 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
您也可以修改全域核准程式以符合您的特定需求。 如需詳細資訊，請參閱 [修改全局批准流程以用於特定對象](#modify-a-global-approval-process-for-use-on-a-specific-object) 這篇文章。

要將現有全局審批流程與項目、任務、問題、模板或模板任務關聯，請執行以下操作：

1. 轉到要關聯審批流程的工作項。
1. 按一下 **核准** 中。

   您可能需要按一下 **顯示更多**，然後按一下 **核准**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   隨即顯示所選的核准程式。

1. 展開 **使用現有** 下拉式功能表，然後選取現有的核准程式。

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   隨即顯示所選的核准程式。

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. 按一下&#x200B;**儲存**。
1. （可選）如果要修改附加至項目的現有審批，請按一下「編輯審批流程」。 這會將全域核准程式變更為單一使用的核准程式。 如需詳細資訊，請參閱 [修改全局批准流程以用於特定對象](#modify-a-global-approval-process-for-use-on-a-specific-object) 這篇文章。

## 修改全局批准流程以用於特定對象 {#modify-a-global-approval-process-for-use-on-a-specific-object}

您的Workfront管理員或群組管理員會建立全域核准程式供您使用，如 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

修改附加至項目的全局審批流程與修改一次性審批流程相同。

您可以修改全局審批流程以符合與其關聯的項目、任務或問題的任何特定需求。

>[!IMPORTANT]
修改全局審批流程時，它將變成一次性審批流程，只能用於修改該流程的對象。 全局批准流程保持不變。
修改全域核准程式時，請考量下列限制：
* 系統僅會為您正在與審批流程關聯的項目、任務或發放修改審批流程。
* 管理員對原始全局審批流程所做的任何將來更改都不會反映在您修改的全局審批流程上。
>


要修改已附加到物料的審批流程，請執行以下操作：

1. 將全局批准流程添加到項目、任務或問題。

   如需指示，請參閱 [將全局審批流程與工作項關聯](#associate-a-global-approval-process-with-a-work-item) 這篇文章。

   >[!IMPORTANT]
   確定您按一下 **儲存** 新增核準時。

1. 新增全域核准程式後，按一下 **編輯**&#x200B;圖示 ![](assets/edit-icon.png) 位於核准頁面的右上角。 此動作會將全域或群組層級的核准程式轉換成單一使用的核准程式。
1. 對現有審批流程進行任何更改。 如需詳細資訊，請參閱 [將一次性審批流程與項目、任務、問題、模板或模板任務關聯](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) 這篇文章。
1. 按一下 **儲存**，然後按一下 **儲存** 再次確認您要將全局批准流程轉換為僅可用於此對象的一次性批准流程。

## 將一次性審批流程與項目、任務、問題、模板或模板任務關聯 {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

您可以建立僅用於特定項目、任務或問題的一次性審批流程。

您也可以將一次性使用的審批流程與模板或模板任務關聯，以便該流程可用於從模板建立的項目和任務。

>[!NOTE]
您可以將一次性審批流程與項目、任務、問題、模板或模板任務的任何系統級或組級狀態相關聯。 如需Workfront狀態的相關資訊，請參閱 [建立或編輯狀態](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

以此方式建立核准程式可讓您建立自訂核准程式，以符合您的需求。 但是，將來不能將審批流程與其他工作項關聯。

或者，您也可以修改特定項目的全局審批流程，該流程也將變成一次性審批流程。 如需詳細資訊，請參閱 [修改全局批准流程以用於特定對象](#modify-a-global-approval-process-for-use-on-a-specific-object) 這篇文章。

要建立一次性審批流程，請執行以下操作：

1. 轉到要關聯審批流程的項目、任務、問題、模板或模板任務。
1. 按一下 **核准** 中。

   您可能需要按一下 **顯示更多** > **核准**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. 按一下 **建立單次使用**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. 完成文章「建立工作項目的系統級或群組級全域核准流程」一節中從步驟6開始的步驟 [建立工作項的審批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   附加一次性使用的核准程式後，會顯示為「`<Custom>`&quot;在模板和模板任務的編輯框內的批准進程欄位中。 如需編輯範本或範本工作的相關資訊，請參閱下列文章：
   * [編輯專案範本](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   * [編輯模板任務](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)


   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## 從工作項目中刪除或刪除審批流程

您可以刪除全局或組級審批流程，也可以從以前與其關聯的項目、任務或問題中刪除一次性審批流程。

存在下列情況： 

* 移除全域或群組層級的核准程式不會刪除核准。 核准仍可供日後使用。
* 刪除單一使用者核准程式會從Workfront中刪除該程式，且無法復原。

要從工作項中刪除或刪除審批流程：

1. 轉到項目、任務、問題、模板或模板任務，以刪除先前添加的審批流程。
1. 按一下 **核准** 中。

   您可能需要按一下 **顯示更多** > **核准**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. 根據與項目關聯的核准類型，在「核准」區段的右上角按一下下列其中一個圖示：

   * **移除**&#x200B;圖示 ![](assets/remove-icon---x-in-circle.png) 全域或群組層級核准。
   * **刪除**&#x200B;圖示 ![](assets/delete.png) 單次使用核准。

1. 按一下 **移除** 或 **刪除** 確認。

   批准過程將從工作項中刪除。

## 自動將審批流程與工作項目關聯

您可以使用以下工作流自動將審批流程與工作項目關聯：

* 對於項目和任務，可以使用模板關聯審批流程。 您可以將現有的審批流程附加到「模板審批」頁簽或「模板任務審批」頁簽。 有關將現有審批與工作項關聯的資訊，請參閱 [將全局審批流程與工作項關聯](#associate-a-global-approval-process-with-a-work-item) 這篇文章。
* 對於現有項目上的新任務，您可以在「編輯項目」框的「任務設定」區域中關聯全局審批流程或組級全局審批流程。 如需詳細資訊，請參閱文章中的「工作設定」一節 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).
* 對於問題，您可以將現有的審批流程與請求隊列關聯，以便將審批與添加到項目的每個新問題關聯。 如需設定請求佇列的相關資訊，請參閱 [建立請求佇列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
