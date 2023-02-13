---
product-area: projects
navigation-topic: manage-issues
title: 指派問題
description: 您可以指派問題給使用者、角色和團隊，指出負責完成問題的人員。 有關分配問題的一般資訊，請參閱修改問題分配概覽。
author: Alina
feature: Work Management
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 0%

---

# 指派問題

您可以指派問題給使用者、角色和團隊，指出負責完成問題的人員。 如需指派問題的一般資訊，請參閱 [修改問題分配概覽](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
>
>如果在停用前已指派使用者、工作角色或團隊，則他們仍會指派給工作項目。 在此情況下，我們建議：
>
>* 將工作項重新分配給活動資源。
>* 將已停用團隊中的用戶與活動團隊關聯，並將工作項重新分配給活動團隊。


除了本文之外，建議您閱讀下列文章，以取得指派問題的詳細資訊：

* [修改問題分配概覽](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md)
* [修改清單中多個問題的用戶分配](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [建立高級分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [進行智慧分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [智慧分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [工作負載平衡器中分配工作的概述](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

您可以在個別問題層級將問題指派給一或多個資源，或一次將多個資源指派給多個問題。

指派問題和工作在Adobe Workfront中類似。 有關分配任務的一般資訊，請參閱 [修改任務分配概覽](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯問題的存取權</p> <p>查看或更高程度地訪問項目和任務</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取層級問題的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予問題的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理問題的權限</p> <p>將權限貢獻至您要複製問題的項目，並提供新增問題的功能。</p> <p> 如需授予問題權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a></p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 指派給工作角色、團隊和使用者的多項考量事項

為工作項分配多個資源時，請考慮以下事項：

* 使用者可以有多個與其設定檔相關聯的工作角色。 有關將用戶與作業角色關聯的資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 通常會先將任務或問題指派給一個或多個作業角色或團隊。 當專案準備好開始時，也可能需要將其指派給使用者。

   如果將任務或問題指派給一或多個角色，然後您又指派一個使用者，Adobe Workfront會根據下列規則決定要與其他使用者建立關聯的作業角色（如果有的話）:

   * 如果只分配了一個作業角色，並且該角色與用戶的主角色匹配，則該任務或問題僅分配給完成其主角色的用戶。
   * 如果分配了多個角色，且至少有一個角色與用戶的輔助角色匹配，則任務或問題將分配給履行其中一個「其他角色」(如果有多個匹配，則Workfront會隨機選擇)的用戶，以及已分配的任何其他角色。
   * 如果分配了一個或多個作業角色，並且沒有與用戶角色匹配的角色，則將任務或問題分配給該角色或角色以及該用戶。

* 如果將任務或問題分配給某個團隊，並且您也分配了某個用戶，則任務或問題將同時分配給該團隊和該用戶。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## 指派單一問題

1. 轉至要指派的問題。
1. 按一下 **指派給** 在問題標題的右上角， **分配** 區域

   或

   如果已分配問題，請按一下當前分配的名稱。

   ![](assets/nwe-assign-to-button-in-header-350x77.png)

1. 執行下列任一項作業：

   * 開始鍵入要指派的用戶、角色或團隊的名稱，然後在清單上出現時按一下。

      ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

   * （條件性）按一下 **建議的分配** 清單
   * 按一下&#x200B;**指派給我** 指派給自己
   * 按一下 **進階**

      建立高級分配對於任務和問題類似。 有關如何進行高級分配的資訊，請參閱 [建立高級分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

      >[!TIP]
      >
      >新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。


1. 按一下 **儲存** 完成指派問題。
1. （選用）按一下 **X圖示** 在問題題頭的「工作總攬」(Assignments)區域中的工作總攬名稱旁邊，以刪除工作總攬。

## 在清單中指派問題

當清單的視圖中顯示任何分配欄位時，您可以在清單或報告中分配問題。 這是指派問題的更快方式。

視檢視中顯示的欄位而定，您可以指派下列實體給問題：

| 選項 | 已分配的實體 |
|---|---|
| **指派給** | 指派一個使用者 |
| **已指派** | 指派一個使用者 |
| **指派** | 指派使用者、工作角色或團隊。 |

若要指派清單中的問題：

1. 轉到視圖中具有「已分配」、「已分配」或「分配」欄位的問題清單。
1. 要分配問題，請執行以下操作之一：

   * 按一下內部 **指派給** 或 **已指派** 欄位，並開始輸入您要指派給問題的作用中使用者名稱，然後在問題顯示於清單時按一下。

      ![](assets/assigned-to-field-task-list-nwe.png)

   * 按一下內部 **分配** 欄位，並開始輸入要指派給問題的作用中使用者、工作角色或作用中團隊的名稱，然後在清單中顯示時按一下。

      ![](assets/assignments-field-task-list-nwe.png)
   >[!TIP]
   >
   >新增使用者指派時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。


1. （條件性）在「工作總攬」欄位中顯示時，按一下 **人員表徵圖** ![](assets/teams.png) 在「工作總攬」(Assignments)框的右上角，開啟「高級工作總攬」(Advanced Assignments)框並建立高級工作總攬。 如需詳細資訊，請參閱 [建立高級分配](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >不能從「已分配至」或「已分配」欄位進行高級分配。

1. 將指派者新增至問題後，按Enter或按一下頁面上的任何位置，以儲存您的變更。

## 大量指派問題

1. 前往您要大量指派的問題清單。
1. 在清單中選取數個問題。
1. 按一下 **編輯圖示** ![](assets/qs-edit-icon.png).

   此 **編輯問題** 對話框。

1. 在 **分配** ，選擇 **受託人** ，然後開始鍵入要分配給所有問題的用戶、作業角色或團隊的名稱。

   >[!IMPORTANT]
   >
   >如果已指派任何問題，您在此處指出的資源會新增至問題，而非取代問題上的現有資源。

1. （選用）選取 **問題所有者** 欄，指出在您為問題分配多個資源時，哪個資源是問題的主要受託人或責任人。 這不適用於團隊。
1. （選用）從 **選擇角色** 中的下拉式功能表 **受託人的角色** 欄。 如果您未選取角色，Workfront會自動選取使用者的主要角色。

1. （可選）如果要從所有問題中刪除現有的受分配者，請執行以下操作之一：

   1. 開始鍵入要從問題中刪除的用戶、角色或團隊的名稱，然後在清單上顯示時選擇它，然後按一下 **刪除受託人** 添加要刪除的附加分配。
   1. 按一下 **刪除所有現有受分配者** 從所有選定問題中刪除所有受分配者。

1. 按一下 **儲存變更**.
1. （可選和條件性）當「已指派給」或「工作總攬」欄位顯示在問題清單中時，請按一下其中一欄內的問題，然後按一下 **X圖示** 在受託人名稱旁，將其從問題中移除。
