---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 使用展示板控制面板
description: 此 [!UICONTROL 展示板] 控制面板顯示您有權存取的展示板清單，包括您建立的展示板和您已新增的展示板。
author: Lisa
feature: Agile
exl-id: bb275f4f-efaf-4dcc-b184-40e015f089b6
source-git-commit: 553e3dd6c903f0ba2f95019b2824cf944745bf09
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# 使用展示板控制面板

{{highlighted-preview}}

展示板控制面板顯示展示板清單 <span class="preview">和集合</span> 您有權存取的展示板，包括您建立的展示板和您新增的展示板。 <span class="preview">您有權存取但不屬於集合的個別展示板會先顯示。</span>

>[!NOTE]
>
>集合只能透過 [!DNL Workfront] [!UICONTROL 展示板].

在控制面板上，您可以對展示板和 <span class="preview">集合</span>:

* 封存展示板（無法封存集合）
* 篩選展示板清單
* 按展示板名稱或修改日期排序展示板清單
* 搜尋展示板或集合
* 刪除展示板或集合

有關建立新展示板或編輯現有展示板的資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md). <span class="preview">如需建立新集合的相關資訊，請參閱 [管理集合](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).</span>

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 篩選板 {#filter-boards}

您可以篩選展示板控制面板，以顯示作用中的展示板、已封存的展示板或所有展示板。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 按一下 [!UICONTROL **篩選**] 選取 **[!UICONTROL 全部]**, **[!UICONTROL 作用中展示板]**，或 **[!UICONTROL 封存的展示板]**.

   在控制面板上套用預設值以外的篩選時，篩選器圖示上會顯示指標 ![[!UICONTROL 套用至的篩選器] 儀表板](assets/boards-filterapplied-30x30.png).

## 排序展示板

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 若要排序展示板清單，請按一下 [!UICONTROL **排序**]. 頁面的預設排序選項為 **[!UICONTROL 修改日期]**. 您也可以依展示板排序頁面 **[!UICONTROL 名稱]**.

   選擇 **[!UICONTROL 反向順序]** 按修改日期或名稱的反向順序排序展示板。 排序圖示上的箭頭指向上時，會套用反向順序。 當箭頭向下時，會套用標準順序。

   在控制面板上套用預設值以外的排序時，排序圖示上會顯示指標 ![已應用排序](assets/sort-applied-boards.png).

## 搜尋展示板 <span class="preview">或集合</span>

<span class="preview">您可以在「展示板」區域中搜尋特定展示板，或在「集合」區域中搜尋特定集合。</span>

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 按一下 [!UICONTROL **搜尋**] 並輸入搜尋詞。 然後，按Enter鍵。

   標題中包含搜尋詞的所有展示板都會隨即顯示。

   按一下X以清除搜尋。

   ![在控制面板上搜尋展示板](assets/boards-searchbox.png)

## 封存展示板

歸檔展示板會將其發送到歸檔檔案，您稍後可以恢復它。

>[!NOTE]
>
>當您存檔展示板時，會為所有展示板成員存檔。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多功能表](assets/more-icon-spectrum.png) 在展示板上，選取 **[!UICONTROL 封存]**.

   安 [!UICONTROL 封存] 圖示 ![封存](assets/archive-icon-spectrum-25x20.png) 出現在展示板上。 您無法編輯已封存的展示板。

   封存的展示板會隱藏在展示板控制面板上，除非您套用篩選器來顯示。 如需詳細資訊，請參閱 [[!UICONTROL 篩選板]](#filter-boards) 一節。

1. 若要還原已封存的展示板，請按一下 **[!UICONTROL 更多]** 功能表 ![「更多」菜單表徵圖](assets/more-icon-spectrum.png) 在展示板上選取 **[!UICONTROL 還原]**.

## 刪除展示板 <span class="preview">或集合</span>

當您刪除展示板時，會從 [!DNL Workfront] 無法恢復。 展示板上的任何資訊卡也會隨展示板一起刪除。

<span class="preview">刪除集合會刪除集合中的所有展示板。</span>

>[!NOTE]
>
>您只能刪除您建立的展示板和集合，不能刪除您新增至的展示板和集合。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 按一下 **[!UICONTROL 更多]** 功能表 ![[!UICONTROL 更多功能表]](assets/more-icon-spectrum.png) 在展示板或集合上，然後選取 **[!UICONTROL 刪除]**.

   <span class="preview">在集合中，功能表位於右側，位於 [!UICONTROL **檢視集合**] 按鈕。</span>

1. 按一下 **[!UICONTROL 刪除展示板]** 或 [!UICONTROL **刪除集合**] 在確認訊息上。

<div class="preview">

## 將展示板移至集合

您可以將獨立展示板移入系列，或將展示板從一個系列移至另一個系列。

>[!NOTE]
>
>您只能移動您建立的展示板，不能移動您新增的展示板。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 按一下 **[!UICONTROL 更多]** 功能表 ![[!UICONTROL 更多功能表]](assets/more-icon-spectrum.png) 在展示板上，選取 [!UICONTROL **移至集合**].
1. 選取要新增展示板的集合，然後按一下 [!UICONTROL **移動**].

   展示板會移入集合中，且不再顯示於 [!UICONTROL 展示板] 的上界。
如果您尚未建立集合，系統會提示您建立集合，以將展示板移入。

</div>
