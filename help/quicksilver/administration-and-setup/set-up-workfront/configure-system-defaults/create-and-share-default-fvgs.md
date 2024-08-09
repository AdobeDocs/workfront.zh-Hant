---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立、編輯和共用預設篩選器、檢視和群組
description: 您可以建立預設的篩選器、檢視和群組，然後讓貴組織中的使用者可以使用它們。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 1%

---

# 建立、編輯和共用預設篩選器、檢視和分組

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以建立預設的篩選器、檢視和群組，然後讓貴組織中的使用者可以使用它們。

當您依照本文所述建立預設篩選器、檢視和群組時，與您共用這些篩選器和群組的使用者可在檢視其清單時運用它們。 使用者可以根據您建立的篩選器、檢視和群組建立自己的篩選器、檢視和群組，但他們無法直接變更您建立的篩選器、檢視和群組。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>您必須是[!DNL Workfront]管理員。</p> <p><b>注意</b>：如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 建立預設篩選器、檢視或群組

{{step-1-to-setup}}

1. 根據您是要建立或編輯篩選、檢視或群組，執行下列任一項作業：

   * 按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 篩選器]**。

   * 按一下&#x200B;**[!UICONTROL 介面] >** **[!UICONTROL 檢視]**。

   * 按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 群組]**。

1. 如果您正在建立篩選器、檢視或群組，請按一下&#x200B;**[!UICONTROL 新增篩選器]**、**[!UICONTROL 新增檢視]**&#x200B;或&#x200B;**[!UICONTROL 新增群組]**，然後選取您要與新篩選器、檢視或群組關聯的物件型別。

   或

   如果您正在編輯現有的篩選器、檢視或群組，請選取該篩選器，然後按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

1. 設定篩選、檢視或群組。

   如需可用選項的相關資訊，請參閱下列文章之一：

   * [篩選器總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * 在[!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)中的[檢視總覽
   * [[!UICONTROL Adobe Workfront]中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 按一下左下角附近的&#x200B;**[!UICONTROL 儲存]**。

您可以讓系統中的使用者可以使用篩選、檢視或分組。 如需與其他使用者共用篩選器、檢視或群組的詳細資訊，請參閱本文中的[讓使用者可以使用篩選器、檢視或群組](#make-filters-views-or-groupings-available-to-users)小節。


## 顯示或隱藏版面配置範本中可用的篩選器、檢視或群組

您可以選擇從版面配置範本顯示或隱藏篩選器、檢視或群組。 可見的篩選器可供系統範圍的所有使用者使用。 您可以使用版面配置範本來隱藏特定使用者或群組的可見篩選器。

>[!NOTE]
>
>如果使用者主動使用篩選器、檢視或分組，然後管理員禁用它，則使用者仍然具有存取權，直到他們選擇新的篩選器、檢視或分組。 選擇新的篩選器、檢視或分組後，他們將無法再恢復為隱藏的篩選器、檢視或分組。

若要顯示或隱藏「版面配置範本」中可用的篩選器、檢視或群組：

1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按一下下列其中一個專案： **[!UICONTROL 篩選器]**、**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 群組]**。

1. （視條件而定）選取您要讓使用者使用的篩選、檢視或群組，然後按一下[啟用系統範圍] ****。

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >如果要讓篩選器、檢視或分組對大部分使用者都可用，但對其他使用者隱藏它，您可以使用「版面配置範本」。 如需詳細資訊，請參閱[使用配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. （視條件而定）選取您要隱藏的篩選器、檢視或群組，然後按一下&#x200B;**[!UICONTROL 停用系統範圍]**。 在停用後，篩選器、檢視或分組將從版面配置範本中隱藏，在整個系統中也將隱藏使用者。


## 讓篩選器、檢視或群組可供所有使用者使用 {#make-filters-views-or-groupings-available-to-users}

這些步驟說明如何從[!UICONTROL 設定]中[!UICONTROL 介面]區域的[!UICONTROL 共用]對話方塊提供篩選器、檢視和群組。 此設定就像整個系統的開啟/關閉開關，包括配置範本。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按一下下列其中一個專案： **[!UICONTROL 篩選器]**、**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 群組]**。

1. 選取您要讓使用者使用的篩選、檢視或群組，然後按一下&#x200B;**[!UICONTROL 共用]**&#x200B;圖示![共用圖示](assets/share-icon.png)以開啟[!UICONTROL 篩選存取權]、[!UICONTROL 檢視存取權]或[!UICONTROL 群組存取權]表單。
1. （視條件而定）若要讓系統內的所有使用者都可以使用篩選、檢視或群組，請按一下&#x200B;**[!UICONTROL 齒輪]**&#x200B;下拉式功能表![](assets/gear-menu-for-sharing-items.png)，然後按一下&#x200B;**[!UICONTROL 讓此在整個系統內可見]**。 系統中的所有使用者現在都可以檢視篩選、檢視或分組。

   或

   開始輸入特定使用者、專案團隊、角色、群組或公司的名稱，以便共用篩選、檢視或分組，然後按一下該名稱（當其出現在下拉式清單中時）。

   如需關於共用的詳細資訊，請參閱[物件共用許可權總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. 按一下「**[!UICONTROL 儲存]**」。

   您指定的使用者現在可以在檢視與其關聯的物件型別時看到預設的篩選、檢視或群組。

## 刪除篩選器、檢視和群組

{{step-1-to-setup}}

1. 根據您要刪除篩選、檢視或群組，執行下列任一動作：

   * 按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 篩選器]**

   * 按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 檢視]**

   * 按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 群組]**

1. 在清單中選取一或多個專案，然後按一下&#x200B;**[!UICONTROL 刪除]**&#x200B;圖示![刪除圖示](assets/delete.png)。
1. 請參閱下列文章之一，以取得有關設定篩選、檢視或分組的詳細資訊。

   * [篩選器總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [在 [!DNL Adobe Workfront]中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [ [!DNL Adobe Workfront]中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
