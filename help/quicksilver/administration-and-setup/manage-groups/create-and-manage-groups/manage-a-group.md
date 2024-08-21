---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，群組，編輯，
navigation-topic: create-and-manage-groups
title: 管理群組
description: 作為群組管理員，您可以從「設定」的「群組」區域管理群組。 如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 0%

---

# 管理群組

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

作為群組管理員，您可以從「設定」的「群組」區域管理群組。 如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

>[!NOTE]
>
>當您被指派為群組的管理員時，您將繼承其下任何子群組的群組管理員角色。 唯一可以管理子群組的使用者是上方最上層群組的群組管理員，以及任何指派給子群組的群組管理員。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

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
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授與使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

+++

## 管理群組的成員資格

您可以在管理的群組中新增及移除使用者和其他群組。 您也可以將群組成員指派為群組的管理員，並管理群組成員的使用者設定檔資訊。

如需指示，請參閱[檢視和管理群組的成員資格](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md)。

## 管理群組的詳細資訊

您可以檢視並編輯您管理的群組或子群組的「群組詳細資訊」頁面。 此頁面包括群組說明、業務主管和群組管理員的姓名，以及可讓您將群組及其所有子群組設為公開或私人的選項。 此外，如果您的存取層級可讓您管理自訂表格，則可以將自訂表格附加至群組。

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

如需指示，請參閱[檢視和管理群組的詳細資料](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)。

## 編輯、複製或刪除群組

您無需離開所檢視群組的首頁面，即可快速編輯、複製或刪除群組。

{{step-1-to-setup}}

1. 按一下&#x200B;**群組**。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 選取群組，然後按一下「編輯![](assets/edit-icon.png)」、「複製![](assets/copy-icon.png)」或「刪除![](assets/delete.png)」圖示。

   如果您需要有關使用顯示的方塊的資訊，請參閱下列其中一項：

   * **編輯**： [檢視和管理群組的詳細資料](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **複製**： [複製發行項[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的現有群組或子群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group)，以建立最上層群組

   * **刪除**： [刪除群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## 設定群組的專案、任務和問題偏好設定

如果您是群組管理員，且您的群組需要與系統層級上設定的不同專案、任務和問題偏好設定設定，您可以要求Workfront管理員解鎖整個組織中所有群組的偏好設定。 解鎖後，您（以及所有其他群組的群組管理員）可以為您管理的群組設定它。

如需指示，請參閱[設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)和[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

## 列出、新增及設定子群組

您可以在管理的群組下建立、檢視、編輯、複製、重新命名、匯出和刪除子群組。

## 設定群組的事件通知

如果Workfront管理員解除鎖定為您組織中的群組設定事件通知的能力，則您可以為您管理的群組設定這些通知。 如需指示，請參閱[檢視並設定群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)的事件通知。

## 建立及自訂群組的狀態

作為群組管理員，您可以為您管理的最上層群組建立自訂狀態。 這賦予您的群組自主權，並有助於消除數十種全公司自訂狀態的需求。 (Workfront管理員也可以為任何群組執行此動作。)

如果Workfront管理員將頂層群組的系統狀態設定為允許自訂，您也可以自訂這些系統狀態。

如需指示，請參閱[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

## 使用群組的專案

在「設定」的「群組」區域中，當您檢視所管理群組的主要頁面時，可以對專案進行下列操作：

* 列出並處理（編輯、複製、刪除和匯出）與群組及其子群組相關聯且已與您共用的專案
* 為群組建立新專案

如需指示，請參閱[建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

## 檢視及管理群組的核准流程

當您檢視您在「群組」區域中管理的群組時，您可以檢視和處理群組的管理員或其子群組之一具有管理存取權的核准程式。

如需指示，請參閱[群組層級核准程式](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)。

## 檢視及管理群組的配置範本

當您檢視您在「群組」區域中管理的群組時，您可以檢視和使用配置範本，該群組或其子群組的管理員可對其擁有管理存取權。

如需指示，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 檢視及管理群組成員的排程

群組管理員為群組建立排程時，必須指定其管理員將管理排程的群組。 通常，這是為其建立排程的群組，但如果群組管理員管理多個群組並指定其他群組之一，則可能是不同的群組。

當您檢視您管理之群組的首頁時，如果該群組被指定為其管理員可以編輯排程的群組，則您可以從群組頁面檢視和管理排程。

如需指示，請參閱[建立和修改群組的排程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md)。

## 檢視和管理群組成員的時程表設定檔

當您檢視您管理之群組的首頁時，可以管理您和群組的其他管理員（或其中一個子群組）有權編輯的時程表設定檔。 如需指示，請參閱[建立和管理群組的時程表設定檔](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)。

## 檢視和管理群組的子群組成員

當您檢視所管理群組的首頁時，可以檢視和管理群組子群組中的所有使用者。 如需指示，請參閱[檢視和管理子群組成員](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)。

## 檢視及管理群組的團隊

當您在「群組」區域中檢視您管理的群組時，您可以檢視與群組或其任何子群組相關聯的專案團隊並與其合作。

如需指示，請參閱[建立和修改群組的團隊](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)。

## 檢視及管理群組的公司

當您檢視您在「群組」區域中管理的群組時，可以檢視與群組或其任何子群組相關聯的公司並加以使用。 如需指示，請參閱[建立和修改群組的公司](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md)。

## 檢視及管理群組的投資組合和計畫

當您檢視在「群組」區域中管理的群組時，如果符合下列兩項條件，您就可以檢視和使用投資組合和計畫：

* 它們與您正在檢視的群組或其任何子群組相關聯
* 您擁有檢視許可權，因為您已建立這些區段或與您共用這些區段

如需指示，請參閱[建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md)和[建立、修改和檢視群組的程式](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md)。

## 停用或重新啟用群組

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

您可以將群組保持在其預設作用中狀態或停用它。

當群組目前不在使用中時，停用該群組會很有用，因為當使用者搜尋要與其他物件關聯的群組時，他們不會再在預先輸入欄位中看到該群組。

如需讓群組停用或啟用的指示，請參閱[停用或重新啟用群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。
