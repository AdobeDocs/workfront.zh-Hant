---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任務狀態
description: 您可以更新任務的狀態，以通知其他人該任務在何處（以及整個專案）及其進行方式。
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# 更新任務狀態

您可以更新任務的狀態，以通知其他人該任務在何處（以及整個專案）及其進行方式。

預設狀態為「新增」、「進行中」和「完成」。 您的Adobe Workfront管理員可為您的組織新增自訂狀態。 如需詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

您可以手動更新任務狀態，也可以讓Workfront在某些動作發生時自動更新。

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

您必須具有下列存取權才能手動更新任務：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 更新任務狀態的注意事項

* 將任務標示為「完成」時，任務的完成百分比會更新為100%。
* 父系任務存在下列情況：
   * 當專案的摘要完成模式設定為自動且子任務未完成時，您無法將父系任務的狀態更新為完成。
   * 當專案的「摘要完成模式」設定為「手動」，且子任務已完成或未完成時，您可以將父系任務的「狀態」更新為「完成」。

  如需詳細資訊，請參閱 [編輯專案](../manage-projects/edit-projects.md).

## 手動更新任務狀態

當您更新任務狀態時，也可以鍵入有關新狀態的說明，並變更其他任務資訊，例如到期日。

1. 移至您要更新其狀態的指定任務。
1. 按一下 **狀態** 欄位並選取新狀態。
1. （選擇性）執行下列任一項作業，提供更新的其他資訊，然後按一下 **更新** 或者，如果任務具有 **完成** 狀態，按一下 **完成：**

   * 若要新增更新的相關附註，請前往 **更新** 區域並按一下 **開始新的更新**，然後輸入您的附註。

   * 若要通知特定使用者有關更新資訊，請在 **通知** 當您鍵入有關更新的註記時出現的方塊。 如需詳細資訊，請參閱 [標籤其他人的更新](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 若要更新工作的狀態，請按一下 **選取條件** 右側 **通知** 方塊（當您鍵入有關更新的備註時，這些選項就會出現），然後選取最能反映目前任務條件的條件。

   * 若要更新任務的認可日期，請展開 **認可日期** 下拉式行事曆，並選取新的認可日期。
   * 若要提供任務完成的視覺化指示，請拖曳完成百分比下的泡泡，或按兩下以輸入百分比值。\
     ![](assets/drag-the-progress-bar-350x155.png)

## 自動更新任務狀態

當下表所列動作發生時，Workfront會自動將任務的現有狀態更新為其他狀態。

>[!NOTE]
>
>下表中的狀態是預設的系統狀態。 您的Workfront管理員或群組管理員可重新命名Workfront執行個體中的狀態。 如需有關在Workfront中建立和管理狀態的資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td>新增或進行中</td> 
   <td>完成</td> 
  </tr> 
  <tr> 
   <td>將任務完成百分比從100%更新為較低數字</td> 
   <td>完成</td> 
   <td>進行中</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>按一下「開始工作」按鈕以接受處理指派給您的工作</span> </td> 
   <td><span>新增</span> </td> 
   <td> <p>任何與您主團隊設定中的[開始工作]按鈕關聯的狀態。</p> <p>有關將「處理它」按鈕取代為「開始任務」按鈕的資訊，請參閱 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將處理它按鈕取代為開始按鈕</a></span>.</p> <p>秘訣： <span>按一下</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">「復原」按鈕</span>按一下「開始任務」後，狀態會恢復為「新增」。 </p> </td> 
  </tr> 
 </tbody> 
</table>
