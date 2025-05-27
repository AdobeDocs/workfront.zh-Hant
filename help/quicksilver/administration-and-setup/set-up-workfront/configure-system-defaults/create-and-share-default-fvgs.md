---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立、編輯和共用系統範圍的篩選器、檢視和群組
description: 您可以建立預設的篩選器、檢視和群組，然後讓貴組織中的使用者可以使用它們。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 4fbf88c544cd56887e6f6f36d7aabfa0668a2a05
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# 建立、編輯和共用系統範圍的篩選器、檢視和群組

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

您可以建立篩選器、檢視和群組，並讓這些篩選器、檢視和群組在整個組織內可供使用者使用。

如本文所述，當您建立系統範圍內的篩選器、檢視和群組時，與您共用這些篩選器、檢視和群組的使用者可在檢視其清單時運用它們。 使用者可以根據您建立的篩選器、檢視和群組建立自己的篩選器、檢視和群組，但無法直接變更。

請注意，您建立的全系統篩選器、檢視和群組與Adobe Workfront自動為您在系統中建立的預設篩選器、檢視和群組不同。 無法編輯或刪除這些預設的篩選器、檢視和群組。

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
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p>
   </td> 
  </tr>
  <tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立篩選器、檢視或群組

{{step-1-to-setup}}


1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按一下下列其中一個專案： **[!UICONTROL 篩選器]**、**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 群組]**。

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


## 讓篩選器、檢視或群組可供所有使用者使用 {#make-filters-views-or-groupings-available-to-users}

您可以選擇顯示或隱藏系統中的篩選器、檢視或群組。 可見的篩選器可供系統範圍的所有使用者使用。 此設定就像整個系統的開啟/關閉開關，包括配置範本。

如果您想要對特定使用者隱藏篩選器、檢視或群組，建議使用版面範本，而不是在整個系統內將其關閉。

>[!NOTE]
>
>* 如果使用者主動使用篩選器、檢視或分組，然後管理員禁用它，則使用者仍然具有存取權，直到他們選擇新的篩選器、檢視或分組。 選擇新檔案後，他們將無法再恢復為隱藏檔案。
>* 如果所有篩選器、檢視和群組都透過「版面配置範本」受到限制，或是在系統範圍內停用，則使用者會看到預設選項，因為系統必須顯示一些內容。

若要顯示或隱藏篩選器、檢視或群組：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按一下下列其中一個專案： **[!UICONTROL 篩選器]**、**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 群組]**。

1. （視條件而定）選取您要讓使用者使用的篩選、檢視或群組，然後按一下[啟用系統範圍] ****。

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >如果要讓篩選器、檢視或分組對大部分使用者都可用，但對其他使用者卻隱藏它，您可以使用「版面配置範本」。 如需詳細資訊，請參閱[使用配置範本自訂篩選器、檢視和群組](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. （視條件而定）選取您要隱藏給使用者的篩選、檢視或群組，然後按一下&#x200B;**[!UICONTROL 停用系統範圍]**。 篩選器、檢視或分組現在對版面配置範本和整個系統的使用者都隱藏。


## 與特定使用者共用自訂篩選器、檢視或群組

這些步驟說明如何使用[!UICONTROL 設定]中[!UICONTROL 介面]區域中的共用對話方塊與特定使用者共用自訂篩選器、檢視和群組。 您可以授予檢視或管理您或其他人建立的篩選器、檢視和群組的存取權。 您無法與使用者共用系統預設值。


{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按一下下列其中一個專案： **[!UICONTROL 篩選器]**、**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 群組]**。

1. 選取您要共用的篩選、檢視或群組，然後按一下&#x200B;**[!UICONTROL 共用]**&#x200B;圖示![共用圖示](assets/share-icon.png)。
1. 開始輸入特定使用者、專案團隊、角色、群組或公司的名稱，以便共用篩選、檢視或分組，然後按一下該名稱（當其出現在下拉式清單中時）。

   如需關於共用的詳細資訊，請參閱[物件共用許可權總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. 選擇使用者、團隊、角色、群組或公司名稱旁的&#x200B;**檢視**&#x200B;或&#x200B;**管理**。 若要微調許可權，請按一下滑桿圖示並調整許可權。

   ![微調許可權](assets/fine-tune-permissions.png)

1. 按一下「**[!UICONTROL 儲存]**」。您指定的使用者現在可以在檢視與其關聯的物件型別時，與篩選、檢視或群組互動。


## 刪除篩選器、檢視和群組

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按一下下列其中一個專案： **[!UICONTROL 篩選器]**、**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 群組]**。

1. 在清單中選取一或多個專案，然後按一下&#x200B;**[!UICONTROL 刪除]**&#x200B;圖示![刪除圖示](assets/delete.png)。

1. 在出現的&#x200B;**刪除**&#x200B;對話方塊中，按一下&#x200B;**是，刪除**。
