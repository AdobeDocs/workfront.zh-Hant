---
product-area: projects
navigation-topic: create-tasks
title: 建立任務概述
description: 只有在建立專案後，才能在專案中建立工作。
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 建立任務概述

只有在建立專案後，才能在專案中建立工作。

例如，建立項目後，您可能需要添加任務並修改任務以組織項目計畫。 如需建立專案的詳細資訊，請參閱 [建立專案](../../../manage-work/projects/create-projects/create-project.md). 有關建立任務的資訊，請參閱 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

本文說明建立任務時所適用的考量事項、限制及預設值。

## 在專案上建立任務的方式

您可以透過下列方式在專案上建立任務：

* 從頭開始，如 [在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* 將任務複製到相同的項目或新項目，或複製同一項目上的任務，如 [複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* 將任務從項目移動到其他項目，如 [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## 建立任務時的限制

如果您擁有正確的存取權和權限，即可在專案上建立工作。 但是，以下是您可能無法建立任務的情況：

* 您的Adobe Workfront管理員或組管理員必須在「項目首選項」區域中啟用向處於「完成」或「無效」狀態的項目添加任務。 有關設定項目首選項的資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 無法向處於「待批准」狀態的項目添加任務。

## 項目上允許的最大任務數

一個專案最多可包含5,000個工作。 當您接近限制時、達到限制時，以及嘗試超過限制時，專案上會顯示警告訊息。

根據實施此限制時專案中的任務數，您的Workfront例項在單一專案中可能允許超過5,000個任務。

如果您能在單一專案中納入超過5,000個工作，請注意下列事項：

* Workfront環境的任務限制已設為您最大專案中的目前任務數量，加上10%的額外值。

   例如，若您Workfront例項中的專案包含10,000個工作，則整個Workfront例項中每個專案的上限為11,000個工作。

* 較小的項目可提高效能，並最大限度地減少大型項目帶來的管理挑戰。

## 將任務添加到項目時，任務預設值

有兩種類型的預設資訊，Workfront會在您建立任務時自動更新這些資訊：

* 系統級預設資訊

   您的Workfront管理員或組管理員在「項目首選項」的「任務和問題」區域中為任務建立系統級預設值。 有關任務和問題首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 或 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* 專案層級預設資訊

   本節的其餘部分說明項目級預設值，作為項目經理，您可以為添加到項目的所有新任務定義這些預設值

將任務新增至專案時，根據專案的設定方式，Workfront可能會自動將核准程式或自訂表單附加至該任務。

如需依預設設定專案以新增這些項目的相關資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md) 文章。

在定義與項目級別添加到項目的任務關聯的預設資訊時，請考慮以下事項：

* 您必須具有項目的「管理」權限，才能定義任務審批流程和自定義表單的預設設定。
* 所有新任務都會使用核准程式和編輯專案時定義的自訂表單來建立。
* 使用「編輯任務」框添加任務時，可以修改這些預設設定，但在內嵌編輯中添加任務時則不能。
* 您可以為範本中的任務定義核准程式和自訂表單。

   * 從此範本建立專案時，核准程式和自訂表單會自動套用至專案。
   * 將模板附加到現有項目後，項目將保留原始任務批准流程和自定義表單設定（如果已定義）。 如果未定義，範本中的設定會成為專案的設定。
   * 將模板附加到現有項目時，從模板添加到項目的任務將保留其在模板上具有的批准流程和自定義表單設定，而不考慮項目上的任務設定。

   如需將範本附加至專案的詳細資訊，請參閱 [將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* 複製專案時，任務預設設定會轉移至新專案。

   如需複製專案的相關資訊，請參閱 [複製專案](../../../manage-work/projects/manage-projects/copy-project.md).

* 將任務從一個項目複製到另一個項目，並且目標項目具有不同的任務預設設定時，複製的任務將保留原始項目的預設設定，除非在複製過程中清除了這些設定。
* 在同一個項目上複製任務時，自定義表單和批准流程將轉移到重複任務。

   有關複製和複製任務的資訊，請參見[ [複製和複製任務](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

* 將任務移到另一個項目時，無論新項目上的任務預設設定如何，預設任務設定都將保存在原始項目的任務上。

   有關移動任務的資訊，請參閱 [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md).
