---
title: 在增強型分析中套用篩選器
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Adobe Workfront增強型分析區域中的篩選器可幫助您專注於特定專案或特定型別的資料。
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 4ade799ff735183f83f045e7eaa876961d266208
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 0%

---

# 在增強型分析中套用篩選器

Adobe Workfront增強型分析區域中的篩選器可幫助您專注於特定專案或特定型別的資料。 您使用的篩選器型別可讓您深入分析：

* 您擁有的專案
* 特定投資組合或計畫檢視
* 特定時間範圍（周、季、會計年度）的關鍵績效指標

您可以視需要新增和移除篩選器，即使您登出，Workfront仍會保留您套用的篩選器。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>
      <p>新計畫：任何</p>
      <p>或</p>
      <p>目前計畫：商務或以上</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>
      <p>新計畫：淺色或更高</p>
      <p>或</p>
      <p>目前計畫：複查或更新</p>
   </td> 
  </tr>
  <tr> 
   <td><b>存取層級*</b> </td> 
   <td> <p>檢視專案的存取權</p> <p>您也必須擁有「任務」、「Portfolio」和「使用者」的「檢視」存取權，才能檢視特定專案欄位篩選選項。</p> <p>注意：如果在「編輯存取層級」對話方塊的「設定其他限制」區段中選取限制，則套用篩選後，您可能無法在篩選或「增強分析」頁面上看到所有資訊。 如需有關Workfront管理員如何變更您的存取層級的資訊，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>物件許可權</b> </p> </td> 
   <td> <p>檢視</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

如需使用增強型分析的先決條件，請參閱 [必要條件](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) 在 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 變更日期範圍篩選 {#change-the-date-range-filter}

依預設，增強型分析區域中的視覺效果會顯示過去60天和未來15天的資料。 您可以選取新的日期範圍，並將其套用至增強型分析區域中的所有視覺效果。 如果您離開頁面，會在您下次回導時套用預設日期範圍。

>[!TIP]
>
>您也可以使用鍵盤上的鍵，導覽至、開啟及選取行事曆Widget的日期範圍。\
>如需詳細資訊，請參閱 [鍵盤快速鍵](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) 文章中的區段 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

若要選取新的日期範圍：

{{step1-to-analytics}}

1. 在右上方，按一下日期範圍欄位以開啟行事曆檢視。
1. 使用日曆上方的箭頭來找出開始日期的月份，然後選取開始日期。

   ![選取日期範圍](assets/filters-select-date-range-350x344.png)

1. 使用日曆上方的箭頭來找出結束日期的月份，然後選取結束日期。
1. （可選）若要放大顯示較短的日期範圍，請在其中一個視覺效果上，將滑鼠從一個特定日期拖曳至另一個特定日期。

   熒幕上的所有視覺效果都會更新以符合所選的時間範圍，而時間範圍篩選器會出現在任何現有篩選器的旁邊。 如果您登出或離開增強型分析區域，則不會保留此篩選器。

   ![時間範圍篩選器](assets/timeframe-filter-350x220.png)

## 新增篩選器

您可以根據預設專案欄位、自訂表單欄位和指派給專案的首頁團隊來新增篩選器。

>[!TIP]
>
>您也可以使用鍵盤上的按鍵，導覽至並新增篩選器。\
>如需詳細資訊，請參閱 [鍵盤快速鍵](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 文章中的區段 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

* [新增專案欄位篩選器](#add-a-project-field-filter)
* [新增專案自訂表單篩選器](#add-a-project-custom-form-filter)
* [新增團隊篩選器](#add-a-team-filter)

### 新增專案欄位篩選器 {#add-a-project-field-filter}

專案欄位篩選可讓您根據預設包含在專案中的欄位中輸入的值，篩選專案和任務的資料。

下列專案欄位篩選型別可供使用：

| 欄位 | 顯示的資料 |
|---|---|
| **專案** | 僅顯示選定專案的資料 |
| **計畫** | 僅顯示選定方案中專案的資料 |
| **Portfolio** | 僅顯示選定投資組合中專案的資料 |
| **條件** | 僅顯示最近具有選定狀態（符合目標、有風險或有問題）之專案的資料 |
| **狀態** | 僅顯示最近具有選定狀態（完成、目前、保留、取消等）的專案資料 |
| **贊助者** | 僅顯示具有所選贊助者的專案的資料 |
| **專案所有者** | 僅顯示具有所選專案所有者的專案的資料 |

自訂表單篩選器的運作方式不同。 如需詳細資訊，請參閱 [新增專案自訂表單篩選器](#add-a-project-custom-form-filter).

若要新增專案欄位篩選：

{{step1-to-analytics}}

1. 在左上方，按一下 **新增篩選器**，然後選取所需的篩選器型別。

   >[!NOTE]
   >
   >不同的篩選器型別會顯示不同的資料。 在一個篩選中只能使用一個篩選型別。 選取篩選器型別後，即無法在其他專案欄位篩選中使用。

1. 請至少輸入三個文字字元，找出您要檢視其資料的值 **搜尋** 欄位，然後選取要納入篩選的每個值。

   若要選取所有目前值，請按一下 **全選**.

   ![選取篩選器值](assets/select-filter-value-350x251.png)

1. 選取所有所需值後，按一下 **套用篩選器**.

   右上角的專案計數會更新，以反映您套用的篩選器。

1. 對每個要新增的篩選器重複這些步驟。

   當您新增篩選器時，資料會顯示在下方的視覺效果中，最多50個專案。

   >[!TIP]
   >
   >若要檢視預設顯示的50個以上專案的資料，您可以：
   >
   >   * 使用左下方的箭頭，在該視覺效果中顯示接下來的50個專案。\
   >     ![分頁箭頭](assets/pagination-350x118.png)
   >   
   >   * 使用 **排序依據：** 視覺效果上的下拉式功能表，以不同順序檢視專案。\
   >     ![依功能表排序](assets/sort-by-menu-350x247.png)

   若要調整日期範圍，請參閱 [變更日期範圍篩選](#change-the-date-range-filter).

### 新增專案自訂表單篩選器

自訂表單篩選型別可讓您根據在專案的自訂表單欄位中輸入的值，篩選專案和任務的資料。 與其他增強型分析篩選器型別不同，您可以新增多個自訂表單篩選器。 每個自訂表單篩選器僅包含在特定自訂表單上選定欄位內輸入的值。

若要新增自訂表單篩選器：

{{step1-to-analytics}}

1. 在熒幕的左上角，按一下 **新增篩選器**，然後選取 **自訂表格**.

   ![選取自訂表單篩選器](assets/select-custom-form-filter-350x271.png)

1. 請至少輸入三個字元的文字，找出您想要的自訂表格 **搜尋** 欄位，然後選取自訂表格。
1. 選取您想要的欄位，然後根據要新增至篩選的欄位型別完成下列動作之一：

   >[!NOTE]
   >
   >並非所有自訂corm欄位型別都可以新增到篩選器中。 目前，增強型分析僅支援下列欄位型別。

   * **核取方塊**， **下拉式清單**，或 **選項按鈕**：選取欄位中要納入篩選的每個值，或按一下 **全選** 核取方塊。\
     ![核取方塊值](assets/custom-form-filter-checkbox-350x255.png)

   * **日期**：使用箭頭來導覽至特定月份，然後在欄位中選取您要納入篩選的日期。\
     ![日期值](assets/custom-form-filter-date-350x348.png)

   * **文字**：在欄位中輸入您要納入篩選的文字。\
     ![文字值](assets/custom-form-filter-text-350x90.png)

   * **數字**：在欄位中輸入您要納入篩選器的數字。\
     ![數值](assets/custom-form-filter-number-350x93.png)

1. 輸入或選取要篩選的值後，按一下 **套用篩選器**.

   右上角的專案計數會更新，以反映您套用的篩選器。

1. 對每個要新增的篩選器重複這些步驟。

   當您新增篩選器時，資料會顯示在下方的視覺效果中，最多50個專案。

   >[!TIP]
   >
   >若要檢視預設顯示的50個以上專案的資料，您可以：
   >  
   >   * 使用左下方的箭頭，在該視覺效果中顯示接下來的50個專案。\
   >     ![分頁箭頭](assets/pagination-350x118.png)
   >   
   >   * 使用 **排序依據：** 視覺效果上的下拉式功能表，以不同順序檢視專案。\
   >     ![依功能表排序](assets/sort-by-menu-350x247.png)

   若要調整日期範圍，請參閱 [變更日期範圍篩選](#change-the-date-range-filter).

### 新增團隊篩選器 {#add-a-team-filter}

{{step1-to-analytics}}

1. 在左側面板中，按一下 **人員**.

   ![選取人員](assets/people-area-cropped-qs-350x276.png)

1. 在畫面左上方，按一下 **新增篩選器**，然後選取 **團隊** 篩選。
1. 請至少輸入三個字元的文字，以找出您要檢視其資料的團隊 **搜尋** 欄位，然後選取要納入篩選的每個團隊。 若要選取所有專案團隊，請按一下 **全選**.

   ![選取團隊](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >無論您的存取層級為何，所有團隊都會納入為篩選器選項。

1. 選取所有所需團隊後，按一下 **套用篩選器**.

   當您新增篩選器時，資料會顯示在以下視覺效果中。

   若要調整日期範圍，請參閱 [變更日期範圍篩選](#change-the-date-range-filter).

## 移除篩選器

您可以隨時移除篩選器。 如果您移除篩選器，該篩選器在您下次造訪增強型分析區域時不會顯示。

>[!TIP]
>
>您也可以使用鍵盤上的按鍵，導覽至並移除現有的篩選器。\
>如需詳細資訊，請參閱 [鍵盤快速鍵](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) 文章中的區段 [增強型分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

若要移除篩選器：

{{step1-to-analytics}}

1. 如果要移除專案欄位或自訂表單篩選器，請保留在 **工作** 區域。

   或

   如果要移除團隊篩選器，請選取 **人員** 在左側面板中。

1. 找到所需的篩選器，然後按一下 **X** 以移除它。

   ![移除](assets/remove-filter-350x213.png)

   篩選器不再啟用，除非您再次新增，否則不會顯示。
