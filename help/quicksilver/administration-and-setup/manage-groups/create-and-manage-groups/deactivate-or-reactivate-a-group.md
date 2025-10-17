---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 停用或重新啟用群組
description: 您可以停用您不再使用的管理群組。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 0%

---

# 停用或重新啟用群組

您可以停用您不再使用的管理群組。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr>
  <tr> 
   <td>存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 停用或重新啟用群組

>[!IMPORTANT]
>
>當您停用群組時，其下方的任何子群組也會停用。
>
>如果您需要重新啟用其中一個，可以執行下列任一項作業之後再啟用：
>
>* 將其從父群組中移除。 如需詳細資訊，請參閱[管理子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make)一文中的[從父群組中移除子群組，並將其設為最上層群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)一節。
>
>* 將其移至使用中群組的下方。 如需詳細資訊，請參閱文章[管理子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create)中的[建立、移動、檢視、編輯、複製、重新命名、匯出或刪除子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)一節。

{{step-1-to-setup}}

1. 在左側面板中，選取&#x200B;**群組**。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下群組的名稱以開啟其頁面。

1. 按一下群組名稱旁的[更多]功能表![更多圖示](assets/more-icon.png)，然後按一下[停用] **或[重新啟用]**&#x200B;**。**

   >[!NOTE]
   >
   >如果群組是已停用群組的子群組，則無法使用作用中選項（預覽中的重新啟用選項）。 您必須先將其從父群組中移除，或將其移動到作用中群組的下方，才能重新啟用它，如上方的重要備註所述。

1. （視條件而定）如果您正在停用群組，請在顯示的&#x200B;**停用群組**&#x200B;方塊中按一下&#x200B;**停用**。

## 非作用中群組的考量事項

請考量下列有關您透過停用[停用或重新啟用本文中群組](#View)一節中說明的[作用中]選項來停用的群組。

* 停用群組也會停用其下方的所有子群組。 這包括您停用子群組後新增的子群組。

  如需在此情況下重新啟用子群組的相關資訊，請參閱本文中的[關於重新啟用非作用中父群組](#about-reactivating-a-subgroup-below-an-inactive-parent-group)下的子群組。

* 當您前往「設定」中的「群組」區域時，您只能在清單中看到作用中的群組，因為「作用中」是預設的篩選器![篩選器圖示](assets/filter-nwepng.png)。 如果您想要檢視您管理的所有群組，包括非作用中的群組，可以使用「全部」篩選器。 或者，使用非使用中篩選器以僅列出非使用中篩選器。

  如需清單中篩選器的詳細資訊，請參閱[篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

* 停用群組不會變更下列專案：

   * 群組與物件的關聯。 關聯的物件會繼續像之前一樣運作，不會有任何變更。

     例如，如果專案與您停用的群組相關聯，專案會繼續使用群組的偏好設定和狀態，而不會有任何變更。

   * 您從設定的群組頁面中建立新物件（例如核准、團隊或公司）的能力。 依預設，新物件與非使用中群組相關聯。
   * 管理員可讓您在篩選器和報表中尋找群組。

     您也可以在群組預先輸入欄位中找到它，您可能想要在其中管理設定區域中的群組設定。 這包括「偏好設定」、「事件通知」和「系統授權」區域。

     例如，如果您前往「設定>專案偏好設定>專案」，並清除那裡選項上方的預先輸入欄位，您仍然可以找到非作用中群組並設定其專案偏好設定。

## 關於重新啟用非作用中父群組下方的子群組 {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

停用群組也會停用其下方的所有子群組。 如果您需要重新啟用非使用中群組下的其中一個子群組，可以執行下列其中一項作業：

* 將子群組移至使用中群組的下方。 然後啟用已移動群組的[作用中]選項，如本文中[停用或重新啟用群組](#View)一節所述。

  如需移動群組的指示，請參閱[移動群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md)。

* 從子群組的父群組中移除子群組（使子群組成為最上層群組）。 然後啟用已移動群組的[作用中]選項，如本文中[停用或重新啟用群組](#View)一節所述。

  如需從父群組移除子群組的說明，請參閱[管理子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make)一文中的[從父群組移除子群組，並使其成為最上層群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)一節。
