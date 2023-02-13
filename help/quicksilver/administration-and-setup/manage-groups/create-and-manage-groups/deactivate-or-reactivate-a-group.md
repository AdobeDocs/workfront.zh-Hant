---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 停用或重新啟用群組
description: 您可以停用您已不再使用的管理群組。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# 停用或重新啟用群組

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

您可以停用您已不再使用的管理群組。

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

## 停用或重新啟用群組

>[!IMPORTANT]
>
>停用群組時，其下的子群組也會停用。
>
>如果您需要重新啟用其中一個活動，可在執行下列任一操作後執行此操作：
>
>* 將其從其父組中刪除。 如需詳細資訊，請參閱 [從子組的父組中刪除子組，並使其成為頂級組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 在文章中 [管理子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* 將其移到活動組下。 如需詳細資訊，請參閱 [建立、移動、查看、編輯、複製、更名、導出或刪除子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) 在文章中 [管理子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，選取 **群組**.

   在隨即顯示的清單中，您可以看到您管理的群組，以及這些群組擁有的任何子群組。 Adobe Workfront管理員可以查看所有群組。

1. 按一下群組名稱以開啟其頁面。

1. 按一下「更多」功能表 ![](assets/more-icon.png) 在群組名稱旁，按一下 **停用** 或 **重新啟用**.

   >[!NOTE]
   >
   >如果群組是停用中群組的子群組，則「處於作用中狀態」選項（預覽中的「重新啟用」選項）無法使用。 必須先將其從父組中刪除，或將其移到活動的組下，然後才能重新激活它，如上面的「重要」備注中所述。

1. （條件性）如果要停用群組，請按一下 **停用** 在 **停用群組** 框。

## 非作用中群組的考量事項

請考量下列關於您停用的群組（透過停用「已啟用」選項）的資訊，其說明於 [停用或重新啟用群組](#View) 這篇文章。

* 停用組也會停用其下的所有子組。 這包括您在停用後新增的子群組。

   有關在此情況下重新激活子組的資訊，請參見 [關於在非活動父組下重新激活子組](#about-reactivating-a-subgroup-below-an-inactive-parent-group) 這篇文章。

* 前往「設定」中的「群組」區域時，清單中只能看到使用中群組，因為「使用中」是預設篩選條件 ![](assets/filter-nwepng.png) 為了它。 如果您想查看您管理的所有群組，包括非作用中群組，可使用「全部」篩選。 或者，使用「非作用中」篩選器只列出非作用中的篩選器。

   如需清單中篩選器的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* 停用群組不會變更下列項目：

   * 組與對象的關聯。 關聯的對象仍像以前一樣運行，沒有任何更改。

      例如，如果項目與您停用的組關聯，則項目將繼續使用組的首選項和狀態，而不會進行任何更改。

   * 您可以在設定的群組頁面中建立新物件，例如核准、團隊或公司。 預設情況下，新對象與非活動組相關聯。
   * 您身為管理員，可在篩選器和報表中尋找群組。

      您也可以在群組預先輸入欄位中找到它，您可能想在「設定」區域中管理群組的設定。 這包括「首選項」、「事件通知」和「系統許可證」區域。

      例如，如果轉到「設定」>「項目首選項」>「項目」，並清除該選項上方的「預先鍵入」欄位，您仍可以找到非活動組並配置其項目首選項。

## 關於在非活動父組下重新激活子組 {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

停用組也會停用其下的所有子組。 如果您需要重新激活非活動組下的其中一個子組，可以執行下列兩項操作之一：

* 在活動組下移動子組。 然後為已移動的群組啟用「有效」選項，如 [停用或重新啟用群組](#View) 這篇文章。

   有關移動組的說明，請參閱 [移動組](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* 從其父組中刪除子組（這使子組成為頂級組）。 然後為已移動的群組啟用「有效」選項，如 [停用或重新啟用群組](#View) 這篇文章。

   有關從子組的父組中刪除子組的說明，請參閱 [從子組的父組中刪除子組，並使其成為頂級組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 在文章中 [管理子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
