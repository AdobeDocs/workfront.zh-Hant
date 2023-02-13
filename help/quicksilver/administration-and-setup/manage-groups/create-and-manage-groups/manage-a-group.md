---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，組，編輯，
navigation-topic: create-and-manage-groups
title: 管理群組
description: 作為組管理員，您可以從「設定」的「組」區域管理組。 如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# 管理群組

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

作為組管理員，您可以從「設定」的「組」區域管理組。 如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

>[!NOTE]
>
>當您被分配為組的管理員時，您將繼承組管理員角色下面的任何子組。 唯一可以管理子組的用戶是上面組的組管理員，以及分配給該子組的任何組管理員。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 管理群組成員

您可以將新增至您管理的群組，並將使用者和其他群組移除。 您也可以將群組成員指派為群組的管理員，並管理群組成員的使用者設定檔資訊。

如需指示，請參閱 [查看和管理組成員資格](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## 管理群組的詳細資訊

您可以查看和編輯您管理的組或子組的「組詳細資訊」頁。 此頁包括組的說明、業務主管和組管理員的名稱，以及一個選項，該選項允許您將組及其所有子組設為公共或私有。 此外，如果您的存取層級可讓您管理自訂表單，您可以將自訂表單附加至群組。

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

如需指示，請參閱 [檢視及管理群組的詳細資訊](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## 編輯、複製或刪除群組

不需離開您正在檢視之群組的主要頁面，即可快速編輯、複製或刪除

<!--
DRAFTED IN FLARE:
or deactivate

-->

組。

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **群組**.

   在隨即顯示的清單中，您可以看到您管理的群組，以及這些群組擁有的任何子群組。 Adobe Workfront管理員可以查看所有群組。

1. 選取群組，然後按一下「編輯」 ![](assets/edit-icon.png)，複製 ![](assets/copy-icon.png)，或刪除 ![](assets/delete.png) 表徵圖。

   如果您需要有關使用顯示方塊的資訊，請參閱下列其中一項：

   * **編輯**: [檢視及管理群組的詳細資訊](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **複製**: [複製現有組或子組以建立頂級組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) 在文章中 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **刪除**: [刪除群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## 配置組的項目、任務和問題首選項

如果您是組管理員，且您的組需要與系統級別上設定的項目、任務和問題首選項設定不同的項目、任務和問題首選項設定，則可以請Workfront管理員解鎖整個組織中所有組的首選項。 解除鎖定後，您（和所有其他群組的群組管理員）就可以為您管理的群組進行設定。

如需指示，請參閱 [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和  [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 列出、添加和配置子組

您可以在您管理的組下建立、查看、編輯、複製、更名、導出和刪除子組。

## 設定群組的事件通知

如果Workfront管理員解除鎖定為組織中的群組設定事件通知的功能，您可以為您管理的群組進行設定。 如需指示，請參閱 [檢視及設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## 建立和自訂群組的狀態

身為群組管理員，您可以為您管理的頂層群組建立自訂狀態。 這可讓您的群組獲得自主權，並有助於消除數十種全公司自訂狀態的需求。 (Workfront管理員也可以針對任何群組執行此動作。)

如果Workfront管理員已將頂層群組設定為允許自訂，您也可以自訂其系統狀態。

如需指示，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## 使用群組的專案

在「設定」的「組」區域中，查看所管理組的首頁時，可以對項目執行以下操作：

* 列出與組及其子組關聯、且已與您共用的項目，並處理（編輯、複製、刪除和導出）
* 為群組建立新專案

如需指示，請參閱 [建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## 檢視及管理群組的核准程式

在「組」區域中查看管理的組時，可以查看並處理組的管理員或其子組具有管理訪問權限的審批流程。

如需指示，請參閱 [組級審批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## 檢視及管理群組的版面範本

在「組」區域中查看管理的組時，可以查看並使用「佈局模板」，該組的管理員或其中一個子組具有管理訪問權限。

如需指示，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 查看和管理組成員的計畫

為組建立調度的組管理員必須指定管理員將管理該調度的組。 通常，這是正在為其建立調度的組，但如果組管理員管理多個組並指定其他組之一，則它可能是不同的組。

當您檢視所管理之群組的主要頁面時，如果將群組指定為管理員可編輯排程的群組，您可以從群組的頁面檢視及管理排程。

如需指示，請參閱 [建立和修改群組的排程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## 查看和管理組成員的時間表配置檔案

查看所管理組的首頁時，可以管理您和其他管理組的時間表配置檔案（或其子組之一），這些配置檔案具有編輯權限。 如需指示，請參閱 [建立和管理組的時間表配置檔案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## 查看和管理組的子組成員

查看所管理組的首頁時，可以查看和管理組子組中的所有用戶。 如需指示，請參閱 [查看和管理子組成員](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## 檢視及管理群組的團隊

在「組」區域中查看管理的組時，可以查看和處理與該組或其任何子組關聯的團隊。

如需指示，請參閱 [建立和修改群組的團隊](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## 檢視及管理群組的公司

在「組」區域中查看管理的組時，可以查看與該組或其任何子組關聯的公司，並與其合作。 如需指示，請參閱 [建立和修改群組的公司](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## 檢視及管理群組的產品組合和方案

當您在「群組」區域中檢視您管理的群組時，如果下列兩者皆為真，則可以檢視並使用產品組合和方案：

* 它們與您正在查看的組或其任何子組相關聯
* 您之所以有權檢視，是因為您已建立或已與您共用

如需指示，請參閱 [建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) 和 [建立、修改和查看組的程式](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## 停用或重新啟用群組

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

您可以將群組保留在其預設作用中狀態或將其停用。

當組當前未使用時，停用該組可能會很有用，因為當用戶搜索要與其他對象關聯的組時，他們不再在「預先輸入」欄位中看到該組。

有關使組處於非活動狀態或處於活動狀態的說明，請參閱 [停用或重新啟用群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
