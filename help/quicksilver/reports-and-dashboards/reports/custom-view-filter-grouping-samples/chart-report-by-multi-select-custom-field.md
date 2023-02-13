---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 按多選自訂欄點陣圖表報表
description: 無法按多選自訂欄位來繪製報表圖表。 您需要建立參照多選自訂欄位的其他計算欄位，以便依多選自訂欄位的值來繪製報表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 按多選自訂欄點陣圖表報表

無法按多選自訂欄位來繪製報表圖表。 您需要建立參照多選自訂欄位的其他計算欄位，以便依多選自訂欄位的值來繪製報表。

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

## 必要條件

開始之前，您必須建立計算的自訂欄位，以顯示從多選自訂欄位中選取的值。 如需詳細資訊，請參閱 [建立參考多選自訂欄位的計算自訂欄位](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 一節。

## 按多選自訂欄點陣圖表報表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

您無法參考多選自訂欄位，以在報表中建立圖表。 相反地，您可以建立計算欄位，根據計算欄位在指定對象和組上記錄多選自定義欄位的值。 

* [建立參考多選自訂欄位的計算自訂欄位](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [建立參考計算自訂欄位的圖表](#build-a-chart-that-references-a-calculated-custom-field)

### 建立參考多選自訂欄位的計算自訂欄位 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

若要建立參考多選自訂欄位的計算欄位，您必須具備下列必要條件：

* 以自訂表單建立多選自訂欄位。\
   如需建立自訂表單及為表單新增自訂欄位的相關資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* 將自定義表單附加到對象。
* 在多選自訂欄位中，為每個物件填入值。

若要建立參考多選自訂欄位的計算自訂欄位：

1. 建立自訂表單或編輯現有表單。\
   如需建立自訂表單的相關資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 選取您打算用於自訂表單的物件。
1. 按一下&#x200B;**新增欄位**，然後 **計算** 將多選自定義欄位添加到窗體中。

1. 在 **標籤** 框中，為新計算欄位命名，以指示它引用了多選自定義欄位。\
   例如：&quot;計算的多選欄位。&quot;

1. 在 **計算** 框中，輸入以下代碼：

   ```
   {DE:Multi-select Custom Field}
   ```

1. 將「多選自訂欄位」取代為多選自訂欄位的實際名稱，如Workfront中所示。

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （可選）如果此表單上已有多選自定義欄位，並且此表單已附加到對象，請啟用 **更新先前的計算** 選項。\
   這可確保新欄位自動填入多選自定義欄位中的值，因為它已添加到附加到對象的表單中。

1. 按一下 **完成**.
1. 按一下 **保存+關閉**.

### 建立參考計算自訂欄位的圖表 {#build-a-chart-that-references-a-calculated-custom-field}

1. （可選）若要確保要繪製圖表的所有計算欄位都已填入值，請選取報表中包含自訂表單的所有對象，其中同時包含多選自訂欄位和計算自訂欄位，然後按一下 **編輯**.
1. （選用和條件式）啟用 **重新計算自定義運算式** 欄位，然後按一下 **儲存變更**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

1. 移至報表，以新增參考多選自訂欄位之計算欄位的圖表。
1. 按一下 **報表動作**，然後 **編輯**.

1. 選取 <strong>分組</strong> ，然後按一下 <strong>添加分組</strong>.
1. 新增<strong>計算的多選欄位</strong> 您已建立為群組。
1. 選取 <strong>圖表</strong> ，並新增圖表至報表。<br>如需將圖表新增至報表的相關資訊，請參閱區段 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">新增圖表至報表</a> 在文章中 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.
1. 選取 <strong>計算的多選欄位</strong> 作為圖表中顯示的其中一個欄位。
1. 按一下 <strong>儲存+關閉</strong>.<br>報表顯示圖表中按「計算多選欄位」分組的結果。
