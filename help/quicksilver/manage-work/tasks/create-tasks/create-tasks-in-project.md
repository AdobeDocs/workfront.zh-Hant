---
product-area: projects
navigation-topic: create-tasks
title: 在專案中建立任務
description: 您只能在建立專案之後在專案中建立任務。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 0%

---

# 在專案中建立任務

<!-- Audited: 10/2024 -->

您可以透過下列方式在Adobe Workfront中建立任務：

* 建立專案後，從頭開始建立專案中的任務。

  建立專案後，您可以新增任務並加以修改以組織專案計畫。 如需建立專案的詳細資訊，請參閱[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

* 將範本新增至專案以建立任務。

  如需詳細資訊，請參閱[將範本附加至專案](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

* 建立個人任務並將其移至專案。

  您可以執行下列其中一項作業來建立個人工作：

   * 建立隨選工作請求並將其傳送給使用者
   * 在首頁區域中建立待辦事項

  如需有關建立不在專案上的個人任務的資訊，請參閱[建立個人任務](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)。

  您可以將個人任務移至專案中，這些任務就會變成工作任務。

本文說明如何從頭開始建立任務，以及如何將個人任務移至專案。

您也可以以下列方式建立任務：

* 透過複製或複製現有任務。 如需詳細資訊，請參閱[複製和複製工作](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。
* 將任務從一個專案移動到另一個專案。 如需詳細資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

## 存取需求

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront授權</p> </td> 
   <td><p>標準</p> 
   <p>工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務與專案的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>為專案貢獻許可權，並可新增任務或以上專案</p> <p>建立任務時，您會自動收到該任務的「管理」許可權</p> <p> 如需工作許可權的相關資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共用工作</a>。 </p> <p>如需要求其他許可權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求存取物件。</a></p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在專案中建立任務

在專案中建立任務類似於在範本上建立任務。 將範本任務新增到範本時，您可以遵循下述步驟。

若要在專案上建立任務：

1. 前往您要建立任務的專案。
1. 按一下左側面板中的&#x200B;**工作**。
1. （視條件而定）如果您目前正在敏捷檢視中檢視工作清單，請按一下右上角的&#x200B;**清單檢視**&#x200B;圖示![](assets/list-view-in-agile-view-for-tasks.png)以顯示工作清單。
1. （選擇性）按一下&#x200B;**計畫模式**&#x200B;圖示![](assets/nwe-plan-mode-icon-task-list.png)並選取&#x200B;**手動儲存**，然後選取&#x200B;**標準**&#x200B;或&#x200B;**時間表計畫**。 這會停用預設啟用的&#x200B;**自動儲存**&#x200B;選項。

   ![選取手動儲存](assets/manual-save-option.png)

   >[!TIP]
   >
   >選取「手動儲存」時，您可以回覆變更。

1. 執行下列任一項作業來建立新作業：

   * 按一下工作清單頂端的&#x200B;**新增工作**。
   * 按一下工作清單底部的&#x200B;**新增更多工作**。

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. （視條件而定）如果您按一下&#x200B;**新增工作**，請執行下列動作：

   1. 在&#x200B;**新增任務**&#x200B;方塊內的有限欄位清單中指定任何欄位，如果要快速建立任務，請按一下&#x200B;**建立任務**。

      或

      若要更新工作的所有欄位，請按一下[其他選項] **&#x200B;**&#x200B;以開啟[建立工作] **方塊**。

      ![](assets/nwe-create-task-small-screen-350x272.png)

      **建立任務**&#x200B;方塊開啟。

      ![](assets/create-task-larger-box-nwe-350x244.png)


      >[!NOTE]
      >
      >視您的Workfront管理員如何設定版面配置範本而定，建立任務方塊中的欄位可能會顯示您環境中的不同欄位。 如需詳細資訊，請參閱[使用配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   1. 在「建立任務」方塊的左側面板中，指定下列區域的資訊：

      * 任務名稱
      * 概觀
      * 指派
      * 自訂表單
      * 財務
      * 設定

        如需定義任務上所有任務相關欄位的詳細資訊，請參閱[編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

   1. （條件式與選擇性）如果您希望工作重複發生，請更新&#x200B;**重複發生頻率**&#x200B;欄位。 如需建立週期性工作的詳細資訊，請參閱[建立週期性工作](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md)。
   1. （選擇性）按一下左側面板中的&#x200B;**檔案**，將檔案附加到新工作，然後按一下&#x200B;**新增或連結檔案**，將檔案從您的電腦、其他服務新增到工作，或從您的電腦或其他服務連結檔案和資料夾。

1. （視條件而定）如果您在步驟5中按一下&#x200B;**新增更多工**，請使用內嵌編輯開始輸入任務資訊，然後按Enter鍵。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   我們建議使用此選項，尤其是在將多個任務新增至清單時。

   ![](assets/add-more-tasks-inline.png)

1. （視條件而定）執行下列任一項作業：

   * 如果您在步驟5中按一下&#x200B;**新增任務**，請按一下&#x200B;**建立任務**&#x200B;以儲存您的變更並將新任務新增至專案。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * 如果您在步驟5中按一下&#x200B;**新增更多工**，請執行下列動作：

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. 按一下瀏覽器中的任意位置以提交變更，或按Enter鍵。
      1. （選擇性）在工作清單中，選取新建的工作，然後按一下&#x200B;**縮排**。

         這會使新任務成為先前任務的子任務或子任務。

         如需有關子系任務的詳細資訊，請參閱文章[建立子任務](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md)中的「從任務子任務建立子任務」一節。

      1. （視條件而定）如果您在按&#x200B;**新增更多工作**&#x200B;後停用&#x200B;**自動儲存**&#x200B;選項，您可以執行下列動作：

         * 隨時按一下&#x200B;**復原**&#x200B;以迴轉您上次的變更，或按一下&#x200B;**取消**&#x200B;以迴轉您對工作清單所做的所有變更。
         * 如果您先前已按一下&#x200B;**復原**，請按一下&#x200B;**取消復原**&#x200B;以重新套用您取消的上次變更。
         * 按一下&#x200B;**儲存**&#x200B;以儲存您對工作清單所做的變更。
   1. （選擇性）在工作清單中，按一下&#x200B;**前置任務**&#x200B;區段，將前置任務新增至工作。 如需詳細資訊，請參閱[使用前置任務區域建立前置任務關係](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md)。
   1. （選擇性）在工作清單中，按一下&#x200B;**子工作**&#x200B;區段以新增子工作。 如需詳細資訊，請參閱[建立子工作](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md)。

## 將個人任務移至專案以建立任務

1. （視條件而定）確定您或其他使用者已建立個人任務。

   如需詳細資訊，請參閱[建立個人工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)。
1. 建立個人任務篩選器，並將其套用至任務報告或清單。

   如需詳細資訊，請參閱[篩選：個人工作](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md)。

   ![](assets/personal-tasks-report.png)
1. 按一下個人工作報告中的工作名稱以開啟它。

   Workfront會將個人任務儲存在未列出的個人專案中，此專案一律根據以下模式命名：「&lt;使用者的全名>的任務」。 例如，個人專案可以命名為「Rick&#39;s Tasks」。

1. 從工作頁面，按一下&#x200B;**更多功能表** ![](assets/more-icon.png)，然後按一下&#x200B;**移動**。 如需關於移動任務的詳細資訊，請參閱[移動任務](/help/quicksilver/manage-work/tasks/manage-tasks/move-tasks.md)。

   在您移動完任務後，該任務會顯示在您選取的專案上。 專案時間表可能受新任務的時間表影響。
