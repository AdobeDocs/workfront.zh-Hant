---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新問題狀態
description: 您可以更新問題的狀態，以通知其他人該問題的位置及其進展情況。
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 3%

---

# 更新問題狀態

<!--Audited: 01/2024-->

您可以更新問題的狀態，以通知其他人該問題的位置及其進展情況。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>投稿人或以上</p>
   <p>要求或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理問題的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 問題狀態

以下是Workfront中問題的預設狀態：

* 新增
* 進行中
* 等待意見反應
* 保留
* 不會解決
* 重新處理
* 已關閉
* 已解決

您的Adobe Workfront管理員可以為您的組織新增問題的自訂狀態。 他們還可以根據問題型別提供狀態。

如需自訂狀態和問題型別的詳細資訊，請參閱以下文章：

* [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [建立問題](../../../manage-work/issues/manage-issues/create-issues.md)

您可以手動更新問題狀態，也可以讓Workfront在某些動作發生時自動更新。

## 手動更新問題狀態

您可以在Workfront的下列區域中更新問題狀態：

* 任務頁面上的問題標題。
* 編輯問題方塊。
* 問題頁面上的詳細資訊區段。
* 在問題清單或報告中，當狀態列位顯示在檢視中時。
* 在問題的摘要面板中。

若要手動更新問題標題中的問題狀態：

1. 移至您要更新其狀態的問題。
1. 按一下問題標題中的&#x200B;**狀態**&#x200B;欄位並選取新狀態。
1. 若要提供問題完成的視覺指示，請拖曳或按兩下問題標題中&#x200B;**完成百分比**&#x200B;下的泡泡

   或

   在問題標題的泡泡內按一下以輸入百分比。

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. （可選）執行下列任一項作業，以提供有關更新的其他資訊：

   * 若要新增關於更新的備註，請移至&#x200B;**更新**&#x200B;區段，然後按一下&#x200B;**新增註解**，然後輸入備註。

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 若要通知特定使用者有關更新，請在您輸入評論時顯示的&#x200B;**標籤人員或團隊**&#x200B;欄位中輸入其名稱。 如需詳細資訊，請參閱[標籤其他人的更新](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。
   * 若要更新問題的認可日期，請按一下&#x200B;**問題詳細資料**，然後編輯&#x200B;**認可日期**&#x200B;欄位。 如需詳細資訊，請參閱[編輯問題](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md)。


   >[!IMPORTANT]
   >
   >  只有問題受指派人可以更新認可日期。



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## 自動更新問題狀態

當下表所列動作發生時，Workfront會自動將問題的現有狀態更新為其他狀態。

>[!NOTE]
>
>下表中的狀態是預設的系統狀態。 您的Workfront管理員或群組管理員可重新命名Workfront執行個體中的狀態。 如需有關在Workfront中建立和管理狀態的資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>動作</b></td> 
   <td><b>原始狀態</b></td> 
   <td><b>新狀態</b></td> 
  </tr> 
  <tr> 
   <td>將問題完成百分比更新為100%</td> 
   <td>新增或進行中</td> 
   <td>已關閉</td> 
  </tr> 
  <tr> 
   <td>將問題完成百分比從100%更新為較低數字</td> 
   <td>已關閉 </td> 
   <td>進行中</td> 
  </tr> 
  <tr> 
   <td>更新附加到問題的解析物件的狀態</td> 
   <td>各種狀態</td> 
   <td> <p>各種狀態</p> <p>如需有關解析物件以及它們如何影響問題狀態的資訊，請參閱解析和可解析物件概覽<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">一文中的「將可解析物件的狀態與解析物件的狀態同步」一節。</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>按一下[開始問題]按鈕以接受處理指派給您的問題</span> </td> 
   <td><span>新增</span> </td> 
   <td> <p>任何與首頁團隊設定中開始問題按鈕相關的狀態。 </p> <p>有關將[處理它]按鈕取代為[開始問題]按鈕的資訊，請參閱<span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將[處理它]按鈕取代為[開始]按鈕</a></span><span>。</span> </p> <p>提示：按一下「開始問題」後按<span data-mc-conditions="QuicksilverOrClassic.Quicksilver">復原按鈕</span>會將狀態還原為「新增」。 </p> </td> 
  </tr> 
 </tbody> 
</table>
