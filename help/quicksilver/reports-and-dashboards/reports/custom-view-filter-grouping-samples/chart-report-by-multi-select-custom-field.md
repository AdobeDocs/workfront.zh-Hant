---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 依據多選自訂欄位繪製報表圖表
description: 只有在您建立其他計算欄位(擷取多選自訂欄位中所選的選項後，才能根據多選自訂欄位繪製報表的圖表。
author: Jenny
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: ce986a912c2ee231b9dc2e1c7a3e9587b20aa0ba
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# 依多選自訂欄位繪製報表圖表

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

建議您不要使用多選自訂欄位來建置圖表，而是為多選自訂欄位的每個選項建立個別的欄位。

多選自訂欄位的範例包括：

* 核取方塊
* 多選下拉式功能表

如需有關使用文字模式的資訊，請參閱文章[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

不過，如果多選欄位的每個選項不可能有單獨的欄位，您可以使用計算出的自訂欄位，先將多選欄位的選擇分組，依多選自訂欄位繪製報表的圖表。 之後，您就可以依據計算欄位繪製報表圖表。

>[!NOTE]
>
>已選取任何選項的專案只會計算一次。
>
>例如，如果您有一個核取方塊自訂欄位，其中選項1和選項2為選項，並且您將表單附加至任務，則同時具有選項1和選項2的任務會顯示在單獨的圖表元素中，而不是只選取選項1或選項2的任務。
>
>已選取選項1的任務不會顯示在已選取選項1和選項2的任務所在的圖表元素中。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>修改篩選器的貢獻者或請求 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須建立一個計算自訂欄位，顯示從多選自訂欄位中選取的值。 如需相關資訊，請參閱本文中的[建立參照多重選取自訂欄位](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)區段的計算自訂欄位。

## 依多選自訂欄位繪製報表圖表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

您無法透過參考多選自訂欄位在報告中建置圖表。 相反地，您可以建立一個計算欄位，記錄指定物件上多選自訂欄位的值，並按計算欄位分組。 

* [建立參照多重選取自訂欄位的計算自訂欄位](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [建立參照計算自訂欄位的圖表](#build-a-chart-that-references-a-calculated-custom-field)

### 建立參照多選自訂欄位的計算自訂欄位 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

若要建置參照多選自訂欄位的計算欄位，您必須具備下列先決條件：

* 自訂表單中的多選自訂欄位。\
  如需有關建立自訂表單及新增自訂欄位的資訊，請參閱文章[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

* 具有附加到物件的多選自訂欄位的自訂表單。
* 每個物件的多選自訂欄位值。

若要建置參照多選自訂欄位的計算自訂欄位：

1. 建立自訂表單或編輯現有表單。

   如需建立自訂表單的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 選取您計畫與自訂表單搭配使用的一或多個物件。
1. 按一下&#x200B;**新增欄位**，然後按&#x200B;**計算**，將多重選取自訂欄位新增至表單。

1. 在&#x200B;**標籤**&#x200B;方塊中，將新的計算欄位命名以表示它參考多重選取自訂欄位。

   例如：「已計算的多重選取欄位」。

1. 在&#x200B;**計算**&#x200B;方塊中，輸入下列程式碼：

   `{DE:Multi-select Custom Field}`

   這會將多選自訂欄位中選取的選項新增至計算自訂欄位。 例如，如果表單已附加到任務並從多選自訂欄位中選擇了選項1，則計算自訂欄位將顯示值「選項1」。 如果為不同的任務選取了選擇1和選擇2，則計算的自訂欄位會顯示值「選擇1，選擇2」。

1. 將「多選自訂欄位」取代為您多選自訂欄位的實際名稱，如Workfront中所示。

   ![已計算的多重選取自訂欄位](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （選擇性）如果多重選取自訂欄位已在此表單上，而且此表單已附加至物件，請啟用&#x200B;**套用至現有計算**&#x200B;選項。

   這可確保新的計算欄位自動填入多選自訂欄位的值，因為該值會新增到已附加到物件的表單中。

1. 按一下&#x200B;**套用**。
1. 按一下&#x200B;**儲存並關閉**。

   計算出的自訂欄位會新增至自訂表單，如果表單目前已附加至物件，則會使用多選自訂欄位的資訊填入該欄位。

### 建立參照計算自訂欄位的圖表 {#build-a-chart-that-references-a-calculated-custom-field}

1. （選擇性）為確保您要用來製作圖表的所有計算欄位皆填入值，您必須重新計算報表中所有物件的自訂運算式。
如需重新計算運算式的資訊，請參閱[編輯自訂欄位中的資訊](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

   <!--from the Details tab of the report select all the objects that contain the custom form with both the multi-select custom field and the calculated custom field, then click **Edit**. 
   1. (Optional and conditional) Select the **Recalculate Custom Expressions** field, then click **Save Changes**.  
   ![Recalculate custom expressions](assets/recalculate-custom-expressions-350x259.png) 
   >[!NOTE]
   >
   >This option has been eliminated from editing projects in bulk.  You can still recalculate expressions for projects in bulk by clicking the **More** icon ![More icon](assets/more-icon-45x33.png) at the top of a project list, then **Recalculate Expressions**. -->

1. 移至您要為參照多選自訂欄位的計算欄位新增圖表的報表。
1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**編輯**。

1. 選取<strong>群組</strong>索引標籤，然後按一下<strong>新增群組</strong>。
1. 新增您建立的<strong>計算多重選取欄位</strong>作為您的群組。
1. 選取<strong>圖表</strong>索引標籤，然後將圖表新增至您的報表。

   例如，選擇&#x200B;**資料行**&#x200B;圖表。
   <br>如需有關將圖表新增至報表的資訊，請參閱文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">建立自訂報表</a>中的<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">將圖表新增至報表</a>小節。
1. 在&#x200B;**底部(X)軸**&#x200B;欄位中，選取要在圖表中顯示的<strong>計算多重選取欄位</strong>。
1. 按一下「<strong>儲存並關閉</strong>」。

   報表會以圖表顯示按「已計算的多重選取欄位」分組的結果。

   ![圖表中的多重選取欄位](assets/chart-multi-select-field-column-chart-example.png)
