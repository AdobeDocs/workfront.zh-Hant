---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任務狀態
description: 您可以更新任務的狀態，以通知其他人任務的位置（和總體項目）及其進展情況。
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# 更新任務狀態

您可以更新任務的狀態，以通知其他人任務的位置（和總體項目）及其進展情況。

預設狀態為「新」、「進行中」和「完成」。 您的Adobe Workfront管理員可為貴組織新增自訂狀態。 如需詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

您可以手動更新任務狀態，也可以讓Workfront在發生某些動作時自動更新。

## 存取需求

<!--drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列存取權，才能手動更新工作：

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 手動更新任務狀態

在更新任務狀態時，您也可以鍵入有關新狀態的說明，並更改其他任務資訊，如到期日。

1. 轉到要為其更新狀態的任務。
1. 按一下 **狀態** 欄位，然後選擇新狀態。
1. （可選）執行下列任一操作以提供有關更新的其他資訊，然後按一下 **更新** 或，如果任務具有 **完成** 狀態，按一下 **完成：**

   * 若要新增有關更新的附註，請前往 **更新** 按一下 **開始新更新**，然後輸入您的備注。

   * 若要通知特定使用者有關更新的資訊，請在 **通知** 框中，此框將在您鍵入有關更新的備注時顯示。 如需詳細資訊，請參閱 [在更新時標籤其他人](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 要更新任務的條件，請按一下 **選擇條件** 至 **通知** 框（當您鍵入有關更新的備注時，這些框將顯示），然後選擇最能反映任務當前條件的條件。

   * 要更新任務的提交日期，請展開 **提交日期** 下拉日曆，然後選擇新的提交日期。
   * 要提供任務完成的視覺指示，請拖動「完成百分比」下的氣泡，或按兩下該氣泡以輸入百分比值。\
      ![](assets/drag-the-progress-bar-350x155.png)

## 自動更新任務狀態

當下表中列出的動作發生時，Workfront會自動將任務的現有狀態更新為不同狀態。

>[!NOTE]
>
>下表中的狀態為預設系統狀態。 您的Workfront管理員或群組管理員可以重新命名Workfront例項中的狀態。 如需在Workfront中建立和管理狀態的相關資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>動作</td> 
   <td>原始狀態</td> 
   <td>新狀態</td> 
  </tr> 
  <tr> 
   <td>將任務完成百分比更新為100%</td> 
   <td>新的或正在進行中</td> 
   <td>已完成</td> 
  </tr> 
  <tr> 
   <td>將任務完成百分比從100%更新為較低的數字</td> 
   <td>已完成</td> 
   <td>進行中</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>按一下「開始任務」按鈕以接受處理分配給您的任務</span> </td> 
   <td><span>新增</span> </td> 
   <td> <p>與「主團隊」設定中的「開始任務」按鈕關聯的任何狀態。</p> <p>有關用「開始任務」按鈕替換「Work On It」按鈕的資訊，請參閱 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕</a></span>.</p> <p>提示： <span>按一下</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">還原按鈕</span>按一下「開始任務」後，狀態會回復為「新建」。 </p> </td> 
  </tr> 
 </tbody> 
</table>
