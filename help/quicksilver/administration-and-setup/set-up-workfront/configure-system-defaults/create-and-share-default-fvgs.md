---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立、編輯和共用預設篩選器、檢視和群組
description: 您可以建立預設的篩選器、檢視和群組，然後讓組織中的使用者能使用。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# 建立、編輯和共用預設篩選器、檢視和群組

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以建立預設的篩選器、檢視和群組，然後讓組織中的使用者能使用。

當您建立本文所述的預設篩選器、檢視和群組時，您與其共用的使用者可以在檢視其清單時運用這些篩選器、檢視和群組。 使用者可以根據您建立的篩選器、檢視和群組建立自己的篩選器、檢視和群組，但無法直接變更您建立的篩選器、檢視和群組。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立預設篩選器、視圖或群組

{{step-1-to-setup}}

1. 根據您要建立或編輯篩選器、檢視或分組，執行下列任一操作：

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 篩選器]**.

   * 按一下 **[!UICONTROL 介面] >** **[!UICONTROL 檢視]**.

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 分組]**.

1. 如果您要建立篩選、檢視或分組，請按一下 **[!UICONTROL 新增篩選]**, **[!UICONTROL 添加視圖]**，或 **[!UICONTROL 添加分組]**，然後選擇要關聯新篩選器、視圖或分組的對象類型。

   或

   如果您要編輯現有的篩選器、檢視或分組，請選取該篩選器，然後按一下 **[!UICONTROL 編輯]** 圖示 ![編輯圖示](assets/edit-icon.png).

1. 設定篩選、檢視或分組。

   如需可用選項的相關資訊，請參閱下列其中一篇文章：

   * [篩選器概觀，於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [檢視概觀，於 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [群組概觀(於 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 按一下 **[!UICONTROL 儲存]** 靠近左下角。

您可以讓系統中的使用者能使用篩選、檢視或分組。 如需與其他使用者共用篩選器、檢視或群組的詳細資訊，請參閱區段 [讓使用者可使用篩選器、檢視或群組](#make-filters-views-or-groupings-available-to-users) 這篇文章。


## 顯示或隱藏「佈局模板」中可用的篩選器、視圖或分組

您可以選擇在「配置範本」中顯示或隱藏篩選器、視圖或分組。 可見篩選器適用於全系統的所有使用者。 您可以使用「版面範本」來隱藏特定使用者或群組的可見篩選器。

>[!NOTE]
>
>如果使用者目前使用篩選、檢視或分組，然後管理員停用該篩選、檢視或分組，則使用者仍有存取權，直到他們選擇新的篩選、檢視或分組為止。 選擇新篩選器、檢視或分組後，他們將無法再回復到隱藏的篩選器、檢視或分組。

要顯示或隱藏「佈局模板」中可用的篩選器、視圖或分組：

1. 按一下 **[!UICONTROL 介面]**，然後按一下下列其中一項： **[!UICONTROL 篩選器]**, **[!UICONTROL 檢視]**，或 **[!UICONTROL 分組]**.

1. （條件性）選取您要讓使用者可用的篩選、檢視或分組，然後按一下 **[!UICONTROL 啟用全系統]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >如果您想要讓大部分使用者都能使用篩選、檢視或分組，但不讓其他使用者看到，則可使用「配置範本」。 如需詳細資訊，請參閱 [使用版面範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. （條件性）選取您要對使用者進行隱藏的篩選、檢視或分組，然後按一下 **[!UICONTROL 禁用全系統]**. 停用後，配置範本以及整個系統的使用者會隱藏篩選、檢視或分組。


## 讓所有使用者都能使用篩選器、檢視或群組 {#make-filters-views-or-groupings-available-to-users}

這些步驟說明如何讓篩選器、檢視和群組可從 [!UICONTROL 共用] 對話框 [!UICONTROL 介面] 區域 [!UICONTROL 設定]. 此設定就像對整個系統（包括佈局模板）的開/關開關。

{{step-1-to-setup}}

1. 按一下 **[!UICONTROL 介面]**，然後按一下下列其中一項： **[!UICONTROL 篩選器]**, **[!UICONTROL 檢視]**，或 **[!UICONTROL 分組]**.

1. 選取您要讓使用者可用的篩選、檢視或分組，然後按一下 **[!UICONTROL 共用]** 圖示 ![共用圖示](assets/share-icon.png) 開啟 [!UICONTROL 篩選存取], [!UICONTROL 檢視存取]，或 [!UICONTROL 分組訪問] 表單。
1. （條件性）若要讓系統中的所有使用者都能使用篩選、檢視或分組，請按一下 **[!UICONTROL 齒輪]** 下拉式功能表 ![](assets/gear-menu-for-sharing-items.png)，然後按一下 **[!UICONTROL 使此可見系統範圍]**. 系統中的所有使用者現在都能看到篩選、檢視或分組。

   或

   開始輸入要與共用篩選、檢視或分組的特定使用者、團隊、角色、群組或公司的名稱，然後在下拉式清單中出現時按一下名稱。

   如需共用的詳細資訊，請參閱 [對象共用權限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   您指定的使用者現在可以在檢視您關聯的物件類型時，看到預設的篩選、檢視或分組。

## 刪除篩選器、檢視和群組

{{step-1-to-setup}}

1. 視您要刪除篩選器、檢視或分組而定，執行下列任一操作：

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 篩選器]**

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 檢視]**

   * 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 分組]**

1. 在清單中選取一或多個項目，然後按一下 **[!UICONTROL 刪除]** 圖示 ![刪除圖示](assets/delete.png).
1. 如需設定篩選器、檢視或分組的詳細資訊，請參閱下列其中一篇文章。

   * [篩選器概觀，於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [檢視概觀，於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [群組概觀(於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
