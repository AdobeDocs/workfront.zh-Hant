---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 建立矩陣報表
description: 矩陣報表以匯總的表格格式呈現摘要資訊，比如傳統報表中的清單顯示更容易檢視。
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# 建立矩陣報表

矩陣報表以匯總的表格格式呈現摘要資訊，比如傳統報表中的清單顯示更容易檢視。

## 矩陣報表的使用時機

您可以為任何包含2個或多個群組的報表建立矩陣報表。 傳統報表最多可包含3個群組，而矩陣報表最多可包含4個群組。

例如，您想要建立一個「小時」報表，顯示3個月期間記錄的小時數，而且您想要根據輸入小時的人員以及按月和周來組織報表。

![](assets/report-matrix-overview-350x123.png)

## 資料在矩陣報表中的顯示方式

矩陣報表中的資訊一律顯示為數值。 在大多數情況下，包含數值的欄最適合在矩陣報表中顯示（例如記錄時數和實際成本）。

不過，其他欄（例如狀態）仍可顯示在矩陣報表中，如下圖所示：\
![](assets/report-matrix-status-350x73.png)

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 設定矩陣報表

1. 建立報表輸出中包含數值資料的傳統報表。\
   如需如何建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 前往您在步驟1建立的報表，按一下 **報表動作**，然後選取 **編輯**.

1. （條件性）如果您已建立檢視，且想要將其套用至此報表，請按一下 **應用現有視圖**，然後從下拉式清單中選取「檢視」 。
1. （條件性）如果要為報表建立新的檢視，請完成下列步驟：

   1. 按一下 **欄（檢視）** ，然後選取要匯總到矩陣報表的欄。
   1. 在 **欄設定** ，按一下 **匯總此欄，依** 下拉式清單中，然後選取用於匯總資訊的可用選項之一。

      >[!IMPORTANT]
      >
      >如果未選取此選項，則列中的資訊無法正確顯示在矩陣報表中。

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. 在「欄（檢視）」標籤中對每一欄重複此程式，然後按一下 **完成**.

1. 按一下 **分組** 標籤。
1. （條件性）如果您已建立分組且想要將其套用至此報表，請按一下 **應用現有分組**，然後從下拉式清單中選取分組。
1. （條件性）如果要為報表建立新的矩陣分組，請完成下列步驟：

   1. 選擇 **切換到矩陣分組** 位於產生器介面的右上角。
   1. 在 **列分組** 節，確定行分組，該分組建立表的水準分組。
   1. （可選）若要新增其他列分組，請按一下 **添加輔助行分組**.
   1. 在 **欄分組** 節，確定列分組，以建立表的垂直分組。
   1. （可選）若要新增其他欄分組，請按一下 **添加輔助列分組**.
   1. （條件性）如果您依日期新增分組，也可指定結果是否依日、周、月、季或年分組。\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. （條件性）如果您選擇按日期分組並按季度顯示結果，例如，通過選擇 **顯示無結果的季度** 核取方塊。\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >此 **顯示無結果的季度** 欄位僅適用於矩陣分組，不適用於標準分組。\
      >只有沒有資料的季度在具有有效資料的兩個季度之間，則矩陣頁簽中的資料值才會顯示為零。 沒有位於篩選器所選時間範圍開始和結束的資料的季度完全不會出現在矩陣分組中。 沒有結果的季度不會顯示在報告的「詳細資訊」頁簽上的分組中。

1. （選用和條件式）按一下 **矩陣設定**，然後從下列選項中選取：\
   **顯示記錄計數：** 選擇此選項可顯示指定欄位條目總數的行。\
   **顯示值列：** 選取此選項，在矩陣中顯示下列資訊：

   * 記錄計數
   * 值欄

      >[!NOTE]
      >
      >此欄包含說明每列資料代表什麼的資訊。\
      >在按分組方式聚合以下欄位的值時，父對象（例如父任務）適用以下例外：
      >
      >   
      >   
      >   * 除「實際小時數」（例如，「計畫/實際人工成本」、「計畫/實際費用成本」、「計畫/實際成本」、「計畫小時數」）之外，所有數字和幣種欄位僅匯總子任務和獨立任務的值。 它們不會匯總父任務或父項的父項的值。
      >   * 「實際小時數」匯總主要父任務和獨立任務的值；它們不會匯總父任務或子任務的父任務的數量。
      >   * 數字和貨幣值的自訂資料欄位會匯總所有任務：父母、子女、父母和獨立任務。 如果建立矩陣報表，以在 **值** 列，請注意，任何父對象（如父任務）的小時數或成本資訊不會顯示在矩陣報表中。 要查看父對象的小時數，必須查看 **詳細資料** 標籤。

   **條件規則：** 為匯總的值設定任何格式規則。\
   新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 按一下 **新增規則** 定義完規則後， **完成** 來儲存規則。

1. 按一下 **篩選器** 標籤來定義要在報表中顯示的資訊。
1. （條件性）如果您已建立篩選器且想要將其套用至此報表，請按一下 **套用現有篩選**，然後從下拉式清單中選取「篩選」 。
1. （條件性）如果您想要為此報表建立新篩選器，請參閱 [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   ，以了解在構建篩選器時可以使用的各種限定符。

1. 按一下 **儲存並關閉** 儲存並檢視矩陣報表。
