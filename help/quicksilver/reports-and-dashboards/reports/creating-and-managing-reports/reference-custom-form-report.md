---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在報表中參考自訂表單
description: 您可以在該物件的報表檢視、篩選器和群組中參考物件的自訂表單。
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# 在報表中參考自訂表單

您可以在該物件的報表檢視、篩選器和群組中參考物件的自訂表單。

您可以參考要包含在報表中的自訂表單內容，也可以參考要包含在報表中的自訂表單本身相關資訊。

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

自訂表單必須存在，您才能在報表中參照。

如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 參考自訂表單的內容

您可以參考自訂表單中的欄位。 將自訂表單套用至物件後，與該自訂表單相關聯的所有欄位都可在報表中參照，如同物件上的任何其他欄位一樣。

>[!NOTE]
>
>對於具有多個選項的欄位，所有選項都可在報表的「篩選和提示」中使用，包括隱藏的選項。\
>如需在自訂欄位中隱藏選項的詳細資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

建立報表時，只需使用表單的物件類型作為欄位來源，並使用自訂欄位的名稱作為欄位名稱。

例如，您可能會將自訂表單套用至包含自訂欄位的所有專案 **顧問**. 若要建立列出Olivia Kim為顧問的所有專案的報表，請使用 **專案** 對象類型作為欄位源，並使用 **顧問** 作為欄位名稱。 將篩選限定符設定為 **等於**&#x200B;然後輸入奧莉維亞·金。

![](assets/qs-consultant-filter-example-350x126.png)

如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 自訂表單的參考資訊

您可以參考自訂表單的相關資訊，例如與物件相關聯的任何自訂表單的名稱。

根&#x200B;據元素（檢視、篩選或分組），您可以參照以下任一項：

* 套用至物件的主要自訂表單：

   這是首先顯示在對象的「詳細資訊」(Details)頁面上的表單。

* 所有自訂表單（如果一個物件套用了多個自訂表單）

您可以參考檢視、篩選和群組上的自訂表單：

* [在報表檢視（欄）中參考自訂表單](#reference-custom-forms-in-a-report-view-column)
* [在報表篩選器中參考自訂表單](#reference-custom-forms-in-a-report-filter)
* [在報表分組中參考自訂表單](#reference-custom-forms-in-a-report-grouping)

### 在報表檢視（欄）中參考自訂表單 {#reference-custom-forms-in-a-report-view-column}

要顯示與對象關聯的所有自定義表單：

1. 開始建立報表，如文章所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **欄** 頁簽，展開要引用的自定義表單所應用的對象類型，然後按一下 **類別名稱**.\
   例如，若要顯示與任務相關聯的所有自訂表單，請展開 **任務** 欄位來源，然後按一下 **類別名稱** 欄位名稱。\
   ![](assets/qs-category-name-column-350x267.png)

要僅顯示與對象關聯的主自定義表單，請執行以下操作：

1. 開始建立報表，如文章所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **欄** 頁簽，展開 **類別** 欄位來源，然後按一下 **名稱** 欄位名稱。\
   ![](assets/qs-category-name-column-2-350x248.png)

### 在報表篩選器中參考自訂表單 {#reference-custom-forms-in-a-report-filter}

要篩選與對象類型關聯的所有自定義表單，請執行以下操作：

1. 開始建立報表，如文章所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **篩選器** 標籤，展開 **類別**，然後按一下 **名稱**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. 選擇要使用的條件限定符：

   * 空白
   * 不為空白
   * 包含
   * 不包含
   * 等於 (區分大小寫)
   * 不等於

   有關每個限定符的詳細資訊，請參閱文章 [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >如果您要篩選的欄位有多個選項，則請使用 **不等於** 或 **不包含** 限定符，這將篩選僅包含您指定的選項的結果。 如果欄位包含其他選項，包括指定的選項，則不會從報表中篩選這些結果。 這包括篩選多個自訂Forms（如果它們附加至相同物件）。

1. 開始輸入要篩選的自訂表單名稱，然後在下拉式清單中出現時按一下名稱。
1. （選用）按一下 **新增其他篩選規則**，然後重複步驟2至4以建立其他篩選規則。
1. 按一下 **儲存並關閉**.

要僅篩選與對象類型關聯的主自定義表單，請執行以下操作：

1. 開始建立報表，如文章所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **篩選器** 頁簽，展開 **類別** 欄位來源，然後按一下 **名稱** 欄位名稱。\
   ![](assets/qs-category-name-filter-350x437.png)

1. 選擇要使用的條件限定符：

   * 空白
   * 不為空白
   * 包含
   * 不包含
   * 等於 (區分大小寫)
   * 不等於

   有關每個限定符的詳細資訊，請參閱文章 [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. 開始輸入要篩選的自訂表單名稱，然後在下拉式清單中出現時按一下名稱。
1. （選用）按一下 **新增其他篩選規則**，然後重複步驟2至4以建立其他篩選規則。
1. 按一下 **儲存並關閉**.

### 在報表分組中參考自訂表單 {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>您只能依與物件相關聯的主要自訂表單來分組項目；不能按與對象關聯的所有表單對項進行分組。

1. 開始建立報表，如文章所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **分組** 標籤，展開 **類別**，然後按一下 **名稱**.\
   ![](assets/qs-category-name-grouping-350x373.png)
