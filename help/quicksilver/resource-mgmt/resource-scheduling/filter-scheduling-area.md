---
product-area: resource-management
navigation-topic: resource-scheduling
title: 篩選「排程」區域中的資訊
description: 在「資源計畫」區域中使用篩選器，可以確定在計畫時間表上顯示哪些工作項。 這包括「未指派」區域中顯示哪些任務和問題，以及顯示哪些用戶。
author: Alina
feature: Resource Management
exl-id: 974b2515-ed10-459d-a317-36e62c52afc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2452'
ht-degree: 0%

---

# 篩選「排程」區域中的資訊

>[!IMPORTANT]
>  
><span class="preview">自2023年1月的23.1版開始，本文所述的排程功能已遭取代，並已從Adobe Workfront中移除。   </span>
>  
> <span class="preview"> 2023年初，23.1版發行後不久，也將移除本文。 此時，建議您據以更新任何書籤。 </span>
> 
><span class="preview"> 您現在可以使用工作負載平衡器來調度資源的工作。 </span>
>  
> <span class="preview">有關使用工作負載平衡器調度資源的資訊，請參見一節 [工作負載平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<p>(SEVERAL SECTIONS BELOW LINKED TO THE PRODUCT. SEE NOTES</p>
-->

在「資源計畫」區域中使用篩選器，可以確定在計畫時間表上顯示哪些工作項。 這包括「未指派」區域中顯示哪些任務和問題，以及顯示哪些用戶。

開始依本節所述篩選內容之前，請先熟悉資源排程在Adobe Workfront中的運作方式。\
如需Workfront中資源排程的相關資訊，請參閱文章 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).\
如需排程時間軸的詳細資訊，請參閱文章 [開始使用資源計畫](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

您可以為您是資源管理員的任何項目，計畫資源或您是其成員或成員的單個團隊。

## 存取需求

您必須具備下列條件：

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
   <td role="rowheader">存取層級*</td> 
   <td> <p>查看對項目、任務和問題的訪問權限或更高權限</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案、工作和問題的權限或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

<!--
<p>(NOTE: sections below - LINKED TO THE ui. DO NOT RENAME/ DELETE)</p>
-->

## 在「排程」區段中建立篩選器（適用於團隊）

您在篩選器中定義的專案、使用者和角色中的任務和問題會顯示在「工作中」標籤的排程時間軸上。 使用篩選器中的選項，可決定在排程時間軸上代表哪些專案、使用者和角色。

>[!NOTE]
>
>您無法在「工作於」索引標籤中儲存篩選器（適用於團隊）。 重新整理頁面或離開頁面時，篩選器會回復為預設設定。

要在團隊的「工作時間」頁簽上為計畫時間線建立篩選器，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **團隊**，選取團隊，按一下 **工作負載平衡器** 在左側面板中，選取 **排程** 從左上角的下拉式功能表。
1. 按一下 **篩選**.
1. 通過指定以下資訊確定在「未分配」區域中表示的項目：

   <!--
   <p>(NOTE: Alina: there was a note that [This step is linked to from the context-sensitive help] but I could not find from where in the UI it is linked.)&nbsp;</p>
   -->

   * **項目優先順序：** 選擇要在計畫時間表上表示的項目的優先順序。 排程時間軸上會顯示包含您選取之優先順序之專案的任務和問題。\
      只有指派給團隊的任務或問題的項目的優先順序才能從此菜單中選擇。
   * **項目狀態：** 選擇要在計畫時間表上表示的項目的狀態。 排程時間軸上會顯示您選取狀態之專案的任務和問題。\
      只有指派給團隊的任務或問題的項目狀態，才能從此菜單中選擇。
   * **專案：** 選擇要在計畫時間表上表示的任何項目。 您選取的專案中的任務和問題會顯示在排程時間表上。\
      您在先前欄位中的選取項目會決定可供選取的專案。\
      只有包含指派給團隊的任務或問題的專案才能從此功能表中選擇。

1. 指定下列資訊，以決定要在排程時間軸上顯示的使用者。 預設情況下，將顯示所有團隊成員。

   <!--
   <p>(NOTE: this step is linked in the UI.)</p>
   -->

   * **角色：** 選擇要在計畫時間表上表示的角色。\
      只有分配給該角色的任務才會顯示在「未分配」區域中。 僅顯示具有您所選角色的用戶，這些用戶可以被分配這些任務。\
      用戶顯示在計畫時間表上，按作業角色組織。
   * **用戶：** 選取要在排程時間表上呈現的個別使用者。\
      系統僅顯示您選擇的用戶，而不管他們是否具有與「未分配」區域中任務的角色分配匹配的角色分配。\
      此選項不會影響「未分配」區域中顯示的任務和問題。

      <!--   
     <p>(NOTE: Alina: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])</p>   
     -->

1. （可選）若要進一步修改排程時間表（例如變更日期範圍），並修改使用者指派，請參閱文章 [在「計畫」區域中手動分配未分配的任務和問題](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p>(NOTE: below - LINKED TO THE UI, DO NOT RENAME/ DELETE/ CHANGE)</p>
-->

## 在「排程」區段中建立和修改篩選器（適用於多個專案）

您可以建立新篩選器、套用您先前建立的篩選器、修改您先前建立的篩選器，或刪除篩選器。 您無法與其他使用者共用您建立的篩選器。

* [在排程區段中建立篩選器（適用於專案）](#create-a-filter-in-the-scheduling-section-for-projects)
* [套用儲存的篩選](#apply-a-saved-filter)
* [修改儲存的篩選](#modify-a-saved-filter)
* [刪除儲存的篩選器](#delete-a-saved-filter)

### 在排程區段中建立篩選器（適用於專案） {#create-a-filter-in-the-scheduling-section-for-projects}

<!--
<p>(NOTE: *****LINKED TO THE PRODUCT FROM THE GLOBAL SCHEDULER >> BOTH THE FIRST AND THE SECOND AREAS) </p>
-->

您在篩選器中定義的專案、使用者和角色中的任務和問題會顯示在「排程」索引標籤的排程時間軸上。 使用篩選器中的選項，可決定在排程時間軸上代表哪些專案、使用者和角色。

要在「計畫」頁簽上為多個項目的計畫時間線建立篩選器，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
1. 按一下 **篩選**.\
   ![](assets/scheduling-filter-350x351.png)

1. 保留 **儲存的篩選** 欄位空白。
1. 通過指定以下資訊確定在「未分配」區域中表示的項目：

   <!--
   <p>(NOTE: Alina: this step is linked in the UI.) </p>
   -->

   * **Portfolio:** 選取任何包含您要在排程時間表上呈現的方案和專案的產品組合。

      只有您所選產品組合內的方案才可在 **方案** 欄位。

   * **計畫：** 選擇要在計畫時間表上表示的包括項目的任何方案。\
      您在 **Portfolio** 欄位決定可供選取的方案。\
      只有您選取的方案內的專案才可在 **專案** 欄位。

   * **項目優先順序：** 選擇要在計畫時間表上表示的項目的優先順序。\
      系統只會顯示具有您選取之優先順序的專案。

   * **項目狀態：** 選擇要在計畫時間表上表示的項目的狀態。\
      系統只會顯示您選取的狀態。

   * **項目公司：** 只有當任務和問題屬於與所選公司匹配的項目時，它們才會顯示在計畫時間軸上。

   * **項目組：** 只有當任務和問題屬於與您選擇的組匹配的項目時，它們才會顯示在計畫時間軸上。

   * **專案：** 選擇要在計畫時間表上表示的任何項目。 您選取的專案中的任務和問題會顯示在排程時間表上。\
      您在先前欄位中的選取項目會決定可供選取的專案。\
      您選取的專案中的任務和問題會顯示在排程時間表上。 只有包含指派給團隊的任務或問題的專案才能從此功能表中選擇。

1. 指定下列資訊，以決定要在排程時間軸上顯示的使用者：(預設情況下，只顯示有資格從「未分配」區域分配任務或問題的用戶。 當您選擇單個用戶時，無論用戶是否有資格從「未分配」區域分配任務或問題，這些用戶都將顯示在計畫時間表上。) 

   <!--
   <p>(NOTE: Alina: this step had a note that it is linked in the UI but I could not find from where.) </p>
   -->

   * **使用者公司：** 此欄位可讓您限制其他公司的使用者顯示在排程時間表上。\
      如果您想要新增任何公司的使用者，請將此欄位留空。 如果您指定個別公司，則只能將這些公司的使用者新增至排程時間軸。 指定公司不會自動將該公司的使用者新增至排程時間軸。 請改為使用下列欄位來新增特定使用者。\
      此選項不會影響「未分配」區域中顯示的任務和問題。****

   * **使用者群組：** 來自您指定之任何使用者群組的所有使用者都會顯示在排程時間表上。

   * **團隊：** 您指定的任何團隊的所有使用者都會顯示在排程時間表上。\
      此選項不會影響「未分配」區域中顯示的任務和問題。

   * **角色：** 選擇要在計畫時間表上表示的角色。\
      只有分配給該角色的任務才會顯示在「未分配」區域中。 僅顯示具有您所選角色的用戶，這些用戶可以被分配這些任務。\
      用戶顯示在計畫時間表上，按作業角色組織。

   * **用戶：** 選取要在排程時間表上呈現的個別使用者。\
      系統僅顯示您選擇的用戶，而不管他們是否具有與「未分配」區域中任務的角色分配匹配的角色分配。\
      此選項不會影響「未分配」區域中顯示的任務和問題。
   <!--
   <p>NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->

1. 按一下 **儲存新篩選器**.\
   您的資料會顯示在排程時間軸上。

1. （可選）若要進一步修改排程時間表（例如變更日期範圍），並修改使用者指派，請參閱文章 [在「計畫」區域中手動分配未分配的任務和問題](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 套用儲存的篩選 {#apply-a-saved-filter}

>[!NOTE]
>
>只有在為多個專案排程資源時（從「排程」索引標籤），才適用此選項；在為團隊計畫資源時（從「工作在」頁簽），或在為單個項目計畫資源時（從「人員配置」頁簽），不能應用保存的篩選器。

您可以套用先前建立的篩選。

若要對多個專案套用儲存的篩選：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
1. 按一下 **篩選**.
1. 在 **儲存的篩選** 欄位，選擇要套用的篩選器。\
   您的資料會顯示在排程時間軸上。

1. （可選）若要進一步修改排程時間表（例如變更日期範圍），並修改使用者指派，請參閱文章 [在「計畫」區域中手動分配未分配的任務和問題](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 修改儲存的篩選 {#modify-a-saved-filter}

>[!NOTE]
>
>只有在為多個專案排程資源時（從「排程」索引標籤），才適用此選項；在計畫團隊資源時（從「工作在」頁簽），或在計畫單個項目的資源時（從「人員配置」頁簽），您無法修改保存的篩選器。

您可以修改先前建立的篩選。

要修改多個項目的已保存篩選器，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
1. 按一下 **篩選**.
1. 在 **儲存的篩選** 欄位中，從下拉式清單中選取您要修改的篩選器。
1. 指定要在排程時間軸上顯示的資料。
1. 按一下&#x200B;**儲存**。\
   您的資料會顯示在排程時間軸上。

1. （可選）若要進一步修改排程時間表（例如變更日期範圍），並修改使用者指派，請參閱文章 [在「計畫」區域中手動分配未分配的任務和問題](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 刪除儲存的篩選器 {#delete-a-saved-filter}

>[!NOTE]
只有在為多個專案排程資源時（從「排程」索引標籤），才適用此選項；在計畫團隊的資源時（從「工作中」頁簽），或在計畫單個項目的資源時（從「人員配置」頁簽），您無法刪除保存的篩選器。

您可以刪除先前建立的篩選器。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，按一下 **資源配置>工作負載平衡器**，然後選取 **排程** 的下拉式功能表。
1. 按一下 **篩選**.
1. 在 **儲存的篩選** 欄位中，在下拉式清單中，按一下您要刪除之篩選器旁的(x)。 

## 在「排程」區段中建立和修改篩選器（適用於單一專案）

<!--
<p>(NOTE: **** LINKED FROM THE PRODUCT FROM THE PROJECT> STAFFING> SCHEDULING AREA) </p>
-->

您在篩選器中定義的使用者、團隊和角色的任務和問題會顯示在「人員配備」標籤的排程時間表上。 使用篩選器中的選項，可決定在排程時間軸上代表哪些使用者、團隊和角色。

>[!NOTE]
您無法在「人員配備」標籤中儲存篩選器（適用於單一專案）。 重新整理頁面或離開頁面時，篩選器會回復為預設設定。

要在「人員配備」頁簽上為單個項目的計畫時間表建立篩選器，請執行以下操作：

1. 前往專案，按一下 **工作負載平衡器** 區段，然後選取 **排程** 從左上角的下拉式功能表。
1. 指定下列資訊，以決定要在排程時間軸上顯示的使用者：(預設情況下，只顯示有資格從「未分配」區域分配任務或問題的用戶。 當您選擇單個用戶時，無論用戶是否有資格從「未分配」區域分配任務或問題，這些用戶都將顯示在計畫時間表上。) 

   <!--
   <p><span>(NOTE: Alina: [This step is linked to from the context-sensitive help]) </span> </p>
   -->

   * **使用者公司：** 此欄位可讓您限制其他公司的使用者顯示在排程時間表上。\
      如果您想要新增任何公司的使用者，請將此欄位留空。 如果您指定個別公司，則只能將這些公司的使用者新增至排程時間軸。 指定公司不會自動將該公司的使用者新增至排程時間軸。 請改為使用下列欄位來新增特定使用者。\
      此選項不會影響「未分配」區域中顯示的任務和問題。

   * **使用者群組：** 來自您指定之任何使用者群組的所有使用者都會顯示在排程時間表上。

   * **團隊：** 您指定的任何團隊的所有使用者都會顯示在排程時間表上。\
      此選項不會影響「未分配」區域中顯示的任務和問題。

   * **角色：** 選擇要在計畫時間表上表示的角色。\
      只有分配給該角色的任務才會顯示在「未分配」區域中。 僅顯示具有您所選角色的用戶，這些用戶可以被分配這些任務。\
      用戶顯示在計畫時間表上，按作業角色組織。

   * **用戶：** 選取要在排程時間表上呈現的個別使用者。\
      系統僅顯示您選擇的用戶，而不管他們是否具有與「未分配」區域中任務的角色分配匹配的角色分配。\
      此選項不會影響「未分配」區域中顯示的任務和問題。
   <!--
   <p>(NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->
