---
product-area: projects
navigation-topic: create-tasks
title: 建立任務總覽
description: 您只能在建立專案之後在專案中建立任務。
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 建立任務總覽

您只能在建立專案之後在專案中建立任務。

例如，建立專案後，您可能會想要新增任務並加以修改以組織專案計畫。 如需建立專案的詳細資訊，請參閱[建立專案](../../../manage-work/projects/create-projects/create-project.md)。 如需有關建立任務的資訊，請參閱[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

本文會說明建立任務時適用的考量事項、限制及預設值。

## 在專案上建立任務的方法

您可以透過下列方式在專案上建立任務：

* 從頭開始，如[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)中所述。
* 將任務複製到相同專案或新專案，或複製相同專案上的任務，如[複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)中所述。
* 將任務從專案移動到另一個專案，如[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)中所述。

## 建立任務時的限制

當您擁有正確的存取權和許可權時，您便可以在專案上建立任務。 但是，在下列情況下，您可能無法建立任務：

* 您的Adobe Workfront管理員或群組管理員必須啟用將任務新增到專案偏好設定區域中處於完成或無法使用狀態的專案。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
* 您無法將任務新增到擱置核准中的專案。

## 專案允許的最大任務數量

一個專案最多可包含5,000個任務。 當您接近限制、達到限制以及如果您嘗試超過限制，專案上會顯示警告訊息。

根據套用此限制時您專案中的任務數量，您的Workfront執行個體可能允許在單一專案中超過5,000個任務。

如果您能在單一專案中包含超過5,000項任務，請注意下列事項：

* Workfront環境的任務限制設為您最大專案中的目前任務數量，外加額外10%。

  例如，如果Workfront執行個體中的專案包含10,000個任務，則您在整個Workfront執行個體中的每個專案限製為11,000個任務。

* 小型專案可改善效能，並最大程度降低大型專案所伴隨的管理挑戰。

## 將任務新增至專案時的任務預設值

建立任務時，Workfront會自動更新兩種型別的預設資訊：

* 系統層級預設資訊

  您的Workfront管理員或群組管理員會在專案偏好設定的「任務和問題」區域中建立任務的系統層級預設值。 有關任務和問題偏好設定的資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)或[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

* 專案層級的預設資訊

  本節的其餘部分說明您作為專案經理，可為所有新增至專案的新任務定義的專案層級預設值

當您將任務新增至專案時，Workfront可能會根據專案的設定方式，自動將核准流程或自訂表單附加至任務。

如需有關設定專案以依預設新增這些專案的資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)文章中的「任務」一節。

在專案層級定義要與新增至專案之任務相關聯的預設資訊時，請考慮下列事項：

* 您必須擁有專案的管理許可權，才能定義任務核准程式及自訂表單的預設設定。
* 所有新任務都是使用編輯專案時定義的核准程式和自訂表單建立的。
* 當您使用「編輯任務」方塊新增任務時，可以修改這些預設設定，但當您在內聯編輯中新增任務時則不能修改。
* 您可以定義範本中任務的核准流程及自訂表單。

   * 從此範本建立專案時，核准程式和自訂表單會自動套用至專案。
   * 當範本附加到現有專案時，專案會保留原始任務核准流程和自訂表單設定（如果已定義）。 如果未定義，則範本中的設定會成為專案的設定。
   * 當範本附加到現有專案時，從範本新增到專案的任務會保留它們在範本上的核准程式和自訂表單設定，無論專案上的任務設定為何。

  如需有關將範本附加到專案的資訊，請參閱[將範本附加到專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

* 當您複製專案時，任務預設設定會傳輸到新專案。

  如需有關複製專案的資訊，請參閱[複製專案](../../../manage-work/projects/manage-projects/copy-project.md)。

* 當您將任務從一個專案複製到另一個專案並且目標專案具有不同的任務預設設定時，複製的任務會保留原始專案的預設設定，除非在複製過程中清除這些設定。
* 當您在相同專案上複製任務時，自訂表單和核准流程會轉移到複製任務。

  如需有關複製和複製任務的資訊，請參閱[[複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

* 當您將任務移動到另一個專案時，預設任務設定將儲存在原始專案的任務上，無論新專案上的任務預設設定如何。

  如需關於移動任務的資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。
