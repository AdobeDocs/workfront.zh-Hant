---
product-area: templates
navigation-topic: templates-navigation-topic
title: 專案範本概觀
description: 您可以使用專案範本來擷取與組織中專案相關的大部分可重複流程、資訊和設定。
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# 專案範本概觀

<!-- Audited: 12/2023 -->

您可以使用專案範本來擷取與組織中專案相關的大部分可重複流程、資訊和設定。

您可以定義任務、佇列主題、自訂表單、在範本中附加檔案。

建立範本後，您可以將範本附加至現有專案，也可以使用範本建立新專案。 範本上的所有資訊都會轉移至使用它建立的專案。

## 在Adobe Workfront中使用範本的優點

以下是建立專案使用範本的一些優點：

* 它可讓您在建立重複的新專案時節省時間和精力。
* 您對於範圍相似的專案擁有一致的資訊。
* 在報告專案時，這個用法很有幫助。 例如，您可以報告共用相同範本的專案、比較其進度並找出完成方式的改善。
* 除了定義未來的專案設定外，您還可以為範本上的未來專案新增下列資訊：

   * 任務
   * 文件
   * 核准
   * 佇列詳細資訊
   * 佇列主題
   * 主題群組
   * 路由規則
   * 自訂Forms
   * 公司和群組資訊

## 建立範本的最佳實務

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

建立範本時，請考量下列事項：

* 不要將使用者指派給範本任務。 雖然您可以讓任務保持未指派狀態，我們建議您為任務指派工作角色。 這可讓您瞭解在使用範本建立專案時，哪些使用者可指派至任務。
* 一律提供範本任務的「持續時間」和「計畫時數」值。 專案中的每個任務都應該與任務可以保持開啟狀態的持續時間相關聯，並且與任務實際完成需要多少時間的計畫小時值相關聯。 在Workfront中使用資源管理工具時，沒有此資訊的任務無法正確編列資源預算。

  如需有關「持續時間」的資訊，請參閱下列文章：

   * [任務期間與期間型別概觀](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [專案期間概觀](../../../manage-work/projects/planning-a-project/project-duration.md)

  如需計畫時數的詳細資訊，請參閱[計畫時數總覽](../../../manage-work/tasks/task-information/planned-hours.md)。

* 當您對未來的專案計畫有完整的清晰瞭解時，在最後的任務之間新增前置任務關係。 將前置任務新增至範本任務與將前置任務新增至專案中的任務類似。

  如需有關將前置任務新增至任務的資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

* 指出該範本可供日後共用的對象，以及從該範本建立的專案可供共用的對象。 如需共用範本的相關資訊，請參閱[共用專案範本](../../../manage-work/projects/create-and-manage-templates/share-project-template.md)。
* 使用全域核准流程，並儘可能將其新增至您的範本和範本任務。 這樣可節省任務或未來專案需要經過相同核准的時間。

  如需關於建立核准的資訊，請參閱[建立工作專案的核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

  如需將核准程式關聯至工作專案的資訊，請參閱[將新的或現有的核准程式與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

## 建立範本的方法

您可以透過下列方式建立新範本：

* 從頭開始。\
  如需從頭開始建立新範本的詳細資訊，請參閱[建立專案範本](../../../manage-work/projects/create-and-manage-templates/create-template.md)。

* 從現有專案，透過將專案另存為範本。\
  如需從現有專案建立範本的詳細資訊，請參閱[從專案建立範本](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md)。

* 透過從另一個範本複製它。\
  如需有關複製現有範本的詳細資訊，請參閱[複製專案範本](../../../manage-work/projects/create-and-manage-templates/copy-template.md)。

* 使用範例範本。\
  如需使用範例範本建立範本的詳細資訊，請參閱[從範例建立專案範本](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md)。
