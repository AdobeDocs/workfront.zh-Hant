---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 依多選自訂欄位繪製報表圖表
description: 只有在您建立其他計算欄位(擷取多選自訂欄位中所選的選項後，才能根據多選自訂欄位繪製報表的圖表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: a2f0ef565b0f0dbcfec7f3f5b5fece4c7b4b1ec6
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# 依多選自訂欄位繪製報表圖表

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

建議您不要使用多選自訂欄位來建置圖表，而是為多選自訂欄位的每個選項建立個別的欄位。

多選自訂欄位的範例包括：

* 核取方塊
* 多選下拉式功能表

如需有關使用文字模式的資訊，請參閱文章 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

不過，如果多選欄位的每個選項不可能有單獨的欄位，您可以使用計算出的自訂欄位，先將多選欄位的選擇分組，依多選自訂欄位繪製報表的圖表。 之後，您就可以依據計算欄位繪製報表圖表。

>[!NOTE]
>
>已選取任何選項的專案只會計算一次。
>
>例如，如果您有一個核取方塊自訂欄位，其中選項1和選項2為選項，並且您將表單附加至任務，則同時具有選項1和選項2的任務會顯示在單獨的圖表元素中，而不是只選取選項1或選項2的任務。
>
>已選取選項1的任務不會顯示在已選取選項1和選項2的任務所在的圖表元素中。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須建立一個計算自訂欄位，顯示從多選自訂欄位中選取的值。 如需詳細資訊，請參閱 [建立參照多選自訂欄位的計算自訂欄位](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 一節。

## 依多選自訂欄位繪製報表圖表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

您無法透過參考多選自訂欄位在報告中建置圖表。 相反地，您可以建立一個計算欄位，記錄指定物件上多選自訂欄位的值，並按計算欄位分組。 

* [建立參照多選自訂欄位的計算自訂欄位](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [建立參照計算自訂欄位的圖表](#build-a-chart-that-references-a-calculated-custom-field)

### 建立參照多選自訂欄位的計算自訂欄位 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

若要建置參照多選自訂欄位的計算欄位，您必須具備下列先決條件：

* 自訂表單中的多選自訂欄位。\
  如需有關建立自訂表單及新增自訂欄位的資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* 具有附加到物件的多選自訂欄位的自訂表單。
* 每個物件的多選自訂欄位值。

若要建置參照多選自訂欄位的計算自訂欄位：

1. 建立自訂表單或編輯現有表單。

   如需建立自訂表單的相關資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 選取您計畫與自訂表單搭配使用的一或多個物件。
1. 按一下 **新增欄位**，然後 **已計算** 將多選自訂欄位新增至表單。

1. 在 **標籤** 方塊中，將新的計算欄位命名以表示它參考了多選自訂欄位。

   例如：「計算的多選欄位」。

1. 在 **計算** 方塊中，輸入下列程式碼：

   `{DE:Multi-select Custom Field}`

   這會將多選自訂欄位中選取的選項新增至計算自訂欄位。 例如，如果表單已附加到任務並從多選自訂欄位中選擇了選項1，則計算自訂欄位將顯示值「選項1」。 如果為不同的任務選取了選擇1和選擇2，則計算的自訂欄位會顯示值「選擇1，選擇2」。

1. 將「多選自訂欄位」取代為您多選自訂欄位的實際名稱，如Workfront中所示。

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （選擇性）如果多選自訂欄位已在此表單上，而且此表單已附加到物件，請啟用 **更新先前的計算（在背景中）** 選項。

   這可確保新的計算欄位自動填入多選自訂欄位的值，因為該值會新增到已附加到物件的表單中。

1. 按一下 **完成**.
1. 按一下 **儲存+關閉**.

   計算出的自訂欄位會新增至自訂表單，如果表單目前已附加至物件，則會使用多選自訂欄位的資訊填入該欄位。

### 建立參照計算自訂欄位的圖表 {#build-a-chart-that-references-a-calculated-custom-field}

1. （選擇性）為確保您要繪製圖表的所有計算欄位皆填入值，請從報表的「詳細資訊」標籤中，選取包含自訂表單的所有物件（包含多選自訂欄位和計算自訂欄位），然後按一下 **編輯**.
1. （選擇性和條件性）選取 **重新計算自訂運算式** 欄位，然後按一下 **儲存變更**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >此選項已從大量編輯專案中移除。  您仍然可以按一下「 」，大量重新計算專案的運算式 **更多** 圖示 ![](assets/more-icon-45x33.png) 在專案清單頂端，然後 **重新計算運算式**.

1. 移至您要為參照多選自訂欄位的計算欄位新增圖表的報表。
1. 按一下 **報表動作**，然後 **編輯**.

1. 選取 <strong>群組</strong> 標籤，然後按一下 <strong>新增群組</strong>.
1. 新增 <strong>計算的多重選取欄位</strong> 您已建立為您的群組。
1. 選取 <strong>圖表</strong> 標籤，然後新增圖表至您的報表。

   例如，選擇 **欄** 圖表。
   <br>如需將圖表新增至報表的詳細資訊，請參閱區段 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">新增圖表至報表</a> 在文章中 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.
1. 在 **底部(X)軸** 欄位，選取 <strong>計算的多重選取欄位</strong> 以顯示在圖表中。
1. 按一下 <strong>儲存+關閉</strong>.

   報表會以圖表顯示按計算的多重選取欄位分組的結果。

   ![](assets/chart-multi-select-field-column-chart-example.png)