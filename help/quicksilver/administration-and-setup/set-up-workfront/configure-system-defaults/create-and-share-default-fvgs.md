---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立、編輯和共用預設的篩選器、檢視和群組
description: 您可以建立預設的篩選器、檢視和群組，然後讓貴組織中的使用者可以使用它們。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# 建立、編輯和共用預設的篩選器、檢視和群組

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以建立預設的篩選器、檢視和群組，然後讓貴組織中的使用者可以使用它們。

當您依照本文所述建立預設篩選器、檢視和群組時，與您共用這些篩選器和群組的使用者可在檢視其清單時運用它們。 使用者可以根據您建立的篩選器、檢視和群組建立自己的篩選器、檢視和群組，但他們無法直接變更您建立的篩選器、檢視和群組。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立預設篩選器、檢視或群組

{{step-1-to-setup}}

1. 根據您是要建立或編輯篩選、檢視或群組，執行下列任一項作業：

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 篩選器]**.

   * 按一下 **[!UICONTROL 介面] >** **[!UICONTROL 檢視]**.

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 群組]**.

1. 如果您要建立篩選、檢視或群組，請按一下 **[!UICONTROL 新增篩選器]**， **[!UICONTROL 新增檢視]**，或 **[!UICONTROL 新增群組]**，然後選取您要與新篩選器、檢視或分組相關聯的物件型別。

   或

   如果您正在編輯現有的篩選器、檢視或群組，請選取該篩選器，然後按一下 **[!UICONTROL 編輯]** 圖示 ![編輯圖示](assets/edit-icon.png).

1. 設定篩選、檢視或群組。

   如需可用選項的相關資訊，請參閱下列文章之一：

   * [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [中的檢視總覽 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [中的群組概述 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 按一下 **[!UICONTROL 儲存]** 左下角附近。

您可以讓系統中的使用者可以使用篩選、檢視或分組。 如需與其他使用者共用篩選器、檢視或群組的詳細資訊，請參閱區段 [讓使用者可以使用篩選器、檢視或群組](#make-filters-views-or-groupings-available-to-users) 本文章內容。


## 顯示或隱藏版面配置範本中可用的篩選器、檢視或群組

您可以選擇從版面配置範本顯示或隱藏篩選器、檢視或群組。 可見的篩選器可供系統範圍的所有使用者使用。 您可以使用版面配置範本來隱藏特定使用者或群組的可見篩選器。

>[!NOTE]
>
>如果使用者主動使用篩選器、檢視或分組，然後管理員禁用它，則使用者仍然具有存取權，直到他們選擇新的篩選器、檢視或分組。 選擇新的篩選器、檢視或分組後，他們將無法再恢復為隱藏的篩選器、檢視或分組。

若要顯示或隱藏「版面配置範本」中可用的篩選器、檢視或群組：

1. 按一下 **[!UICONTROL 介面]**，然後按一下下列其中一項： **[!UICONTROL 篩選器]**， **[!UICONTROL 檢視]**，或 **[!UICONTROL 群組]**.

1. （視條件而定）選取您要讓使用者使用的篩選、檢視或群組，然後按一下 **[!UICONTROL 在整個系統內啟用]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >如果要讓篩選器、檢視或分組對大部分使用者都可用，但對其他使用者隱藏它，您可以使用「版面配置範本」。 如需詳細資訊，請參閱 [使用版面配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. （視條件而定）選取您要對使用者隱藏的篩選、檢視或群組，然後按一下 **[!UICONTROL 在整個系統內停用]**. 在停用後，篩選器、檢視或分組將從版面配置範本中隱藏，在整個系統中也將隱藏使用者。


## 讓篩選器、檢視或群組可供所有使用者使用 {#make-filters-views-or-groupings-available-to-users}

以下步驟說明如何讓篩選器、檢視和群組可在以下位置使用： [!UICONTROL 共用] 對話方塊 [!UICONTROL 介面] 區域於 [!UICONTROL 設定]. 此設定就像整個系統的開啟/關閉開關，包括配置範本。

{{step-1-to-setup}}

1. 按一下 **[!UICONTROL 介面]**，然後按一下下列其中一項： **[!UICONTROL 篩選器]**， **[!UICONTROL 檢視]**，或 **[!UICONTROL 群組]**.

1. 選取您要讓使用者使用的篩選、檢視或群組，然後按一下 **[!UICONTROL 共用]** 圖示 ![「共用」圖示](assets/share-icon.png) 以開啟 [!UICONTROL 篩選器存取權]， [!UICONTROL 檢視存取權]，或 [!UICONTROL 群組存取權] 表單。
1. （視條件而定）若要讓系統內的所有使用者都可以使用篩選、檢視或分組，請按一下 **[!UICONTROL 齒輪]** 下拉式功能表 ![](assets/gear-menu-for-sharing-items.png)，然後按一下 **[!UICONTROL 使其在整個系統內可見]**. 系統中的所有使用者現在都可以檢視篩選、檢視或分組。

   或

   開始輸入特定使用者、專案團隊、角色、群組或公司的名稱，以便共用篩選、檢視或分組，然後按一下該名稱（當其出現在下拉式清單中時）。

   如需共用的詳細資訊，請參閱 [物件許可權共用概觀](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 按一下「**[!UICONTROL 儲存]**」。

   您指定的使用者現在可以在檢視與其關聯的物件型別時看到預設的篩選、檢視或群組。

## 刪除篩選器、檢視和群組

{{step-1-to-setup}}

1. 根據您要刪除篩選、檢視或群組，執行下列任一動作：

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 篩選器]**

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 檢視]**

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 群組]**

1. 在清單中選取一或多個專案，然後按一下 **[!UICONTROL 刪除]** 圖示 ![「刪除」圖示](assets/delete.png).
1. 請參閱下列文章之一，以取得有關設定篩選、檢視或分組的詳細資訊。

   * [篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [中的檢視總覽 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [中的群組概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
