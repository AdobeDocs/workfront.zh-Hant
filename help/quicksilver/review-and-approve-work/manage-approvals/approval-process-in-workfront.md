---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 核准程序概觀
description: 您可以建立核准程式並將其附加至物件，以確保指定的使用者在物件進行之前先檢閱某些變更。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '1804'
ht-degree: 0%

---

# 核准程序概觀

<!-- Audited: 12/2023 -->

您可以建立核准程式並將其附加至物件，以確保指定的使用者在物件進行之前先檢閱某些變更。

這適用於Adobe Workfront中的下列物件型別：

* 工作專案（專案、任務或問題、範本、範本任務）
* 文件
* 校樣

本文包含與工作專案相關之核准流程的一般資訊。
如需建立核准流程的指示，請參閱[建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

## 工作專案的核准流程型別

如果您是Adobe Workfront管理員或具有核准流程管理存取權的使用者，則可以為專案、任務和問題建立以下核准流程：

* **系統層級全域核准程式**：使用者可以將這些連結附加到下列任一項：

   * 核准區段中的專案、任務或問題
   * 在編輯專案方塊中的任務預設核准流程區域
   * 在預設核准流程區域中專案的佇列詳細資訊或佇列主題區段中。 專案必須啟用為請求佇列。

* **群組層級全域核准程式**：使用者可以將這些內容附加至下列專案：

   * 屬於「核准」區段中與核准流程相關聯之群組的專案、任務或問題
   * 在任務預設核准流程區域中屬於與核准流程相關聯之群組的專案的「編輯專案」方塊中
   * 在預設核准流程區域中專案的佇列詳細資訊或佇列主題區段中。 專案必須啟用為請求佇列，且必須屬於與核准流程關聯的群組。

  如需有關建立系統層級或群組層級核准流程的資訊，請參閱[建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

* **單一使用核准程式**：用於單一專案、任務、問題、範本或範本任務。 此型別的核准程式只會影響與其關聯的物件，而無法與任何其他物件關聯。

  如需有關建立單一使用核准流程的資訊，請參閱[將新的或現有的核准流程與工作建立關聯](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

>[!NOTE]
>
>本文使用「全域核准流程」一詞來區分「單次使用核准流程」。 全域核准流程可重複使用。
>
>「群組層級全域核准流程」一詞是指可重複用於專案的核准流程，其狀態僅與特定群組相關聯。

For information about creating a system-level approval process or a group-level approval process see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considerations about approval processes

* You must create the project, task, issue, template, or template task before the approval process can be associated with them.
* An approval process is always associated with two essential things:

   * Each approval process corresponds to a certain work item status in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.

     >[!TIP]
     >
     >
     >   
     >   
     >   * You can associate a group-level approval with a global or a group-level status.
     >   * You cannot change the status of an item using an approval process to a status other than the one associated with the approval process.
     >   
     >   
     >     For example, if you have a task approval associated with the status of In Progress, the task automatically changes its status to In Progress when the approval is granted. It cannot automatically change its status to Completed or any other status that is not associated with the approval.
     >   
     >   
     >

   * The entities associated with an approval process can be users, job roles, or teams. Users are ultimately responsible for accepting or rejecting the approval. You can assign approvals to users who fulfill a certain role on the project. For example, you can assign an approval to a Project Owner, or Sponsor. For more information, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     存在下列情況：

      * When you assign an approval to job roles, any user on the Project Team who is associated with the job role can make a decision on the approval. The role associated with the approval can be either their Primary Role or any Other Roles.

        For information about the Project Team, see [Project Team overview](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * When you assign an approval to a team, any member of that team can make a decision on the approval. The team associated with the approval can be either their Home Team or any of their Other Teams.

        For information about a user&#39;s roles and teams, see [Edit a user&#39;s profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* When you create a work item, it does not automatically have an approval process attached. You must attach one manually if you want to use one. For information about attaching an approval process to an item, see [Associate a new or existing approval process with work](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* The Workfront administrator or a user with administrative access to approval processes can create a system-level global approval processes for use throughout the system. A group administrator with administrative access to approval processes can create a group-level global approval process for use only by a certain group that they manage.
* If you don&#39;t want to use a predefined system-level or group-level global approval process for a work item, you can create and attach a single-use approval process to it when you have Manage permissions to the object for which you want to attach the approval process.

  >[!NOTE]
  >
  >You can use a single-use approval process only once for the specific item for which it was created. You can associate global statuses as well as group-level statuses for single-use approval processes for projects, tasks, issues, templates, and template tasks.

* When attaching a group-level approval process to an item using group-level custom statuses, changing the Group of the project might create a conflict between the approval statuses of the previous group and those existing at the system level. Consider removing the group-level approval processes on the project, or its tasks or issues before updating the group. For information about creating group-level approval processes, see [Group-level approval processes](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). For information about creating custom group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). For information about updating the Group of a project, see [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).

## The approval process workflow

This section explains the following about approving work items:

* [How approval processes rely on statuses](#how-approval-processes-rely-on-statuses)
* [How a typical workflow uses an approval process](#how-a-typical-workflow-uses-an-approval-process)

### How approval processes rely on statuses {#how-approval-processes-rely-on-statuses}

Attaching a status to an approval process ensures that the item moves through departments in the right order.

**Example:** You could attach an approval process to the Marketing Department status that requires approval by the Finance department. Then, when someone changes the status for a work item to &quot;Marketing Department,&quot; the item can&#39;t move to that department until the Finance department signs off on it.

For more information about statuses for work items, see the following articles:

* [Access the list of system project statuses](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Access the list of system task statuses](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Access the list of system issue statuses](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### How a typical workflow uses an approval process {#how-a-typical-workflow-uses-an-approval-process}

The following scenario illustrates how an approval process helps users approve work as a Workfront object progresses through a workflow of several steps in this order:

1. The Workfront administrator or a user with administrative access to Approval Processes creates an approval process for a project, task, or issue.

   >[!NOTE]
   >
   >您可以將專案核准流程附加至範本，將任務核准流程附加至範本任務。 執行此動作後，當有人使用範本建立專案時，核准流程就會分別變成專案或任務核准流程。 附加到範本或範本任務的一次性使用核准流程仍然是專案和任務的一次性使用核准流程。

1. 擁有專案、任務或問題管理許可權的使用者會將核准流程附加到專案，或建立專案的單次使用核准。
1. 指定給工作專案的使用者會將其狀態變更為啟動核准流程的狀態，而核准流程隨即開始。 （建立核准程式的人定義了狀態與核准程式之間的關係。）
1. 指定的核准者會收到有關未決核准流程的通知，並複查工作專案。
1. 核准程式會在指定的核准者核准該程式的所有步驟後結束。 或者，如果他們拒絕步驟，則狀態會重設為預先定義的狀態，或建立問題。 （建立核准流程的人會定義在拒絕後要執行哪些自動步驟。）

**範例：**&#x200B;廣告團隊已建立名為「準備列印」的狀態，以及名為「Designer/撰稿人簽章」的核准程式，此狀態與其相關聯。 此核准流程已設定為：

* 需要團隊的設計師和撰稿人的核准
* 當有人將工作專案的狀態變更為準備列印時啟動

傳單專案所有者會將Designer/撰稿人簽章核准程式附加至傳單專案。

當專案上的人員將狀態變更為「準備列印」時，撰稿人和設計人員會收到通知，要求他們核准或拒絕該專案。 在核准程式中，當他們考慮是否核準時，專案狀態將顯示為準備列印 — 未決核准。

他們在Workfront中核准傳單後，專案狀態會變更為「準備列印」。

## 舊版檔案核准流程


舊版檔案核准用於更一般的核准。 意見反應會以聊天格式擷取在「更新」索引標籤上。 您可以使用核准按鈕來核准、拒絕或核准變更。

若要在檔案上傳至Workfront後新增核准者，請參閱[請求舊版檔案核准](../../review-and-approve-work/manage-approvals/request-document-approvals.md)。

>[!NOTE]
>
>Workfront中目前有數個檔案核准選項。 如需詳細資訊，請參閱[檔案核准的可用功能](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)。


## 校訂核准流程

校訂核准用於更深入的審查，通常包括更複雜的工作流程。 意見是透過校訂檢視器中的標籤工具擷取。 您可以使用核准按鈕來核准、拒絕或核准變更。

若要將自動化工作流程新增至檔案校訂，並將工作流程中的某些使用者指定為校訂的核准者，請參閱[使用自動化工作流程建立進階校訂](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)。

## 配置工作專案核准流程的設定

作為Workfront管理員，您可以為系統中的工作專案核准流程設定全域設定。 這些設定會決定核准流程的各種規則，例如核准決定應該允許保持開啟的時間長短，或者您如何在系統中管理核准委派。 如需核准程式設定的詳細資訊，請參閱[設定全域核准設定](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)。
