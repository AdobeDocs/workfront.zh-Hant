---
title: 在報表畫布中新增或編輯表格區塊
description: 在報表畫布中新增或編輯表格區塊
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: d706659c-457f-4da0-a6e7-03ea29cab700
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# 在報表畫布中新增或編輯表格區塊

表格會在欄中顯示欄位資訊，這些欄可以進行篩選、分組和排序。

## 必要條件

開始之前，您必須註冊「報表畫布測試版」。 如需詳細資訊，請參閱 [報表畫布測試版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 添加或編輯表塊

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.
1. 按一下 **新報表**.

   或

   前往現有報表，按一下 **更多** 圖示 ![](assets/more-icon-27x15.png) 在報表標題中，按一下 **編輯**.

1. 在畫面的右側，位於 **新增區塊**，其中之一：

   拖曳 **表格** 圖示 ![](assets/table-icon.png) 直接放到畫布上您想要的位置。

   或

   按兩下 **表格** 圖示 ![](assets/table-icon.png) 將表格新增至畫布頂端。

   >[!TIP]
   >
   >通過拖動塊的拐角控點，可以在放置塊後更改塊的大小。

1. 按一下 **無標題表** 在表格標題中，輸入表格的標題。

   ![](assets/table-name-350x142.png)

1. 按一下 **編輯** 在表格區塊的中央以設定表格。

   >[!NOTE]
   >
   >如果表格已是畫布的一部分（例如編輯現有報表時），則 **編輯** 按鈕不會顯示在區塊的中央。 若要編輯表格，請按一下 **編輯** 圖示 ![](assets/edit-icon.png) 填入表格標題。
   >![](assets/edit-icon-table-header-350x71.png)

1. 在 **欄位** 在右側的「 」面板中，找出要作為列添加到表中的欄位，然後將其拖動到所需的表中，或按兩下該欄位以將其添加為表中的最後一列。

   您可以在 **搜尋** 框，按名稱查找特定欄位。 您也可以使用此方塊下的兩個下拉式功能表，將顯示欄位清單縮小為下列其中一個或兩個欄位：

   * 與所需欄位相關聯的對象類型，如「項目」或「任務」
   * 您想要的欄位類型，例如日期或貨幣

   對要新增為欄的每個欄位重複此步驟。

   >[!TIP]
   >
   >通過將選定列拖到新位置，可以更改表中列的順序。

1. 執行下列任一操作以進一步配置表：

   * **新增公式欄位**:按一下 **新增+** 在 **欄位** 清單。 有關建立公式欄位的更多說明，請參閱 [在報表畫布中建立公式欄位](../../../reports-and-dashboards/reporting-canvas/table-blocks/create-formula-field.md).
   * **新增篩選**:將您要表格篩選依據的欄位拖曳至 **篩選** 一節。 如需設定篩選規則的詳細資訊，請參閱 [在報表畫布中篩選表格](../../../reports-and-dashboards/reporting-canvas/table-blocks/configure-filter-rules-for-table.md).
   * **按特定屬性分組行**：將您要表格依分組的欄位拖曳至 **群組** 一節。 如需建立列群組的詳細資訊，請參閱 [在報表畫布中將表格列分組](../../../reports-and-dashboards/reporting-canvas/table-blocks/group-rows-in-table.md).
