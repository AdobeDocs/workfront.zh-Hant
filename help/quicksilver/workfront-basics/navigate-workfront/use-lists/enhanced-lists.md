---
navigation-topic: get-started-with-workfront
title: Use Enhanced Lists
description: Enhanced lists use a table format for displaying the list items, and they have a different look and feel than the standard lists
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '2931'
ht-degree: 1%

---

# 使用增強型清單

Enhanced lists are available in some areas of Adobe Workfront. These lists use a table format for displaying the list items, and they have a different look and feel than the standard lists. The management of views is also enhanced, including filtering, grouping, managing columns, and searching.

For information about the standard lists, see [Get started with lists in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

>[!NOTE]
>
>Each enhanced list may be configured differently to help you display the data that you need. Every list will not use every feature described in this article, and some lists may have specialized features that only apply to that list.

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>投稿人或以上</p>
   <p>要求或更高版本</p></td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Objects that use enhanced lists

Below are some types of Workfront object lists that use the enhanced list format and some of the areas where they display by default when you have rights to view the object.

>[!NOTE]
>
>This list is not comprehensive. Each of these object lists can also appear on a report or a dashboard. For example, a Request report or a dashboard that contains a Request report also displays a list of requests.

| Workfront list | Location of object list |
| --- | --- |
| 優先順序 | <ul><li>Home > select the Priorities icon in the left menu</li><li>Main Menu > Priorities</li></ul> |
| List of requests | <ul><li>Requests (new experience only)</li><li>My Requests widget on Home</li></ul> |
| 設定中的狀態、優先順序、嚴重程度和匯率清單 | <ul><li>設定>專案偏好設定>狀態</li><li>設定>專案偏好設定>優先順序</li><li>設定>專案偏好設定>嚴重程度</li><li>設定>專案偏好設定>匯率</li></ul> |
| 報告清單 | 報告（**使用可共用的資料夾**&#x200B;必須開啟） |
| 費率卡上的職務角色和費率清單 | 設定>費率卡>選取費率卡>職務角色與費率 |
| 翻譯清單 | 設定>本地化 |
| 快照清單 | 專案>快照 |
| 計費的資源清單 | 專案>計費資源 |
| 在任務中新增進階指派 | 任務>工作總攬>進階 |
| Adobe企業儲存空間上的檔案 | 專案、任務、問題、投資組合、計畫範本>檔案 |

## 將專案新增至增強型清單

請根據您檢視的增強型清單，執行下列任一項作業：

1. 按一下清單右上方的藍色按鈕。 此選項會開啟對話方塊，您可以在其中輸入資訊。 資料會儲存為表格中的新列。

   或

1. 按一下清單底部的&#x200B;**新列**。 此選項會將新的一列新增至表格。 在儲存格中連按兩下以輸入資訊。 每個儲存格代表清單專案的欄位。 欄位必須先存在，您才能在清單中看到它們。

   增強型清單支援這些欄位型別：

   * 文字
   * 數字
   * 貨幣
   * 日期
   * 日期與時間
   * 單一/多選下拉式清單
   * 自動提示
   * 段落
   * 被指定者（一或多個）
   * 檢色器

   >[!NOTE]
   >
   >每個欄位型別都有自己的編輯選項。 有些欄位可能是唯讀的。

![增強型清單範例](assets/glist-exchange-rates.png)

## 使用動作列編輯專案

您可以使用增強型清單中的動作列來編輯清單中的專案。 並非所有動作列都包含相同的選項。 此外，有些清單可能不允許您選取專案，而且動作列無法使用。

1. 選取增強型清單中專案旁的核取方塊。

   動作列會顯示在畫面底部。

   >[!NOTE]
   >
   >根據您編輯的清單，您可以選取一個或多個專案來使用動作列。

1. 按一下列上的動作以編輯專案。 您可以選擇的動作範例包括：

   * 檢視
   * 編輯
   * 刪除
   * 複製
   * 移至資料夾
   * 共用

   如果選取的專案沒有可用的動作，動作列會顯示「沒有可用的動作」。

   ![動作列範例](assets/glist-action-bar-statuses.png)

1. 暫留在清單專案的主要欄位上，然後按一下&#x200B;**更多**&#x200B;功能表![更多功能表圖示](assets/more-icon.png)以檢視其他動作。 有些動作可能特定於該清單。

   >[!TIP]
   >
   >主要欄位會顯示在清單的第一欄。

   ![更多功能表範例](assets/glist-more-menu-priorities.png)

## 自訂欄

根據您在增強型清單中檢視的物件，您可以隱藏、顯示或重新排序清單中的欄。

1. 按一下清單上方的&#x200B;**欄**。

   ![顯示資料行範例](assets/glist-display-move-columns.png)

1. 使用切換來顯示或隱藏清單中的欄。
1. 若要重新排序欄，請按一下&#x200B;**拖曳**&#x200B;圖示![拖曳圖示](assets/drag-icon.png)並將欄移至您想要的位置。 移動欄會自動變更清單。

   >[!NOTE]
   >
   >主要欄位是清單中的第一欄。 它在第一個位置是固定的，您無法變更其欄。 如果欄數很大，則主要欄位會凍結在左側，當您水準捲動時，您永遠可以看到它。
   >
   >欄位名稱旁的圖示會顯示欄位型別，例如文字或日期欄位。

   當欄隱藏時，**欄**&#x200B;按鈕上會出現指示器。 當您重新排序欄時，指示器未出現。

   隱藏資料行的![指標](assets/glist-columns-hidden-indicator.png)

### 重新命名欄

有些欄可讓您儲存欄標題的自訂名稱。

1. 將游標停留在欄上，然後按向下箭頭並選取&#x200B;**重新命名**。

   ![選取重新命名資料行](assets/glist-rename-or-sort-column.png)

1. 在&#x200B;**重新命名**&#x200B;對話方塊中，在&#x200B;**自訂標籤**&#x200B;欄位中輸入資料行的名稱，然後按一下&#x200B;**儲存**。

   新欄名稱會出現在清單中。

### 使用欄管理員新增和移除欄

您可以在某些增強型清單中使用&#x200B;**資料行管理員**，以輕鬆地新增及移除清單上的資料行。 您可以將已存在於Workfront中作為欄的系統欄位和自訂欄位新增或移除至增強型清單。

若要新增和移除欄：

1. 按一下表格右上角的+圖示以開啟&#x200B;**欄管理員**&#x200B;方塊。
1. 搜尋&#x200B;**可用**&#x200B;欄位中的現有物件欄位，然後按一下欄位名稱右側的+ ，以將其新增至&#x200B;**已選取**&#x200B;欄。
1. Click - to the right of a field in the **Selected** column to remove it from the list.

   >[!NOTE]
   >
   >Some fields might be fixed and cannot be removed.

   <!-- Add info about Properties and KPIs when something gets released with those options -->

1. 按一下「**儲存**」。

   ![Column manager](assets/glist-column-manager.png)

   The list updates the columns according to the choices you made.

### Change the row height in a view

>[!NOTE]
>
>Not all enhanced lists have all the elements described in this section.

1. Click the **Row height** icon ![Row height icon](assets/row-height-icon.png) in an enhanced list.

   This updates the vertical length of a row. 從下列選項中選擇:
   * 短
   * Standard. This is the default choice.
   * 媒體
   * 高

## Update enhanced list elements

The following elements are components of an enhanced list:

* **View**: Defines the columns, filters, and groupings in the list with preset settings
* **Filters**: Limits the amount of information displayed in the list
* **Groupings**: Organize the list items according to common fields
* **Sort**: Arranges the items in a list according to the order you identify for a given field
* **Search**: Quickly finds an item using a search keyword

### Apply and create views

>[!NOTE]
>
>Not all enhanced lists have all the elements described in this section.

To apply or create a view:

1. Click the **Views** dropdown and select an existing view to apply it to the list

   或

   Click **New view** to create one.

1. (Conditional) For adding a new view, enter a name for the view, then click **Create**.
1. (Optional) Hide, show, or rearrange the columns. For more information, see [Customize columns in an enhanced list](#customize-columns-in-an-enhanced-list).
1. （選用）篩選清單。 如需詳細資訊，請參閱[篩選增強型清單](#filter-items-in-an-enhanced-list)中的專案。
1. （選用）將清單中的專案分組。 如需詳細資訊，請參閱增強型清單](#group-items-in-an-enhanced-list)中的[群組專案。

   檢視的變更會自動儲存。 下次套用此檢視時，欄和篩選設定仍會保留您設定的方式。

### 共用檢視

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

在&#x200B;**檢視**&#x200B;下拉式清單中，您可能會看到三種檢視類別：

* **系統檢視**：系統管理員指派給您的檢視。 您無法共用系統檢視。
* **共用的檢視**：其他使用者與您共用的檢視。
* **我的檢視**：您建立且可與其他人共用的檢視。 您可以與其他使用者、團隊或群組共用檢視。

當您共用檢視時，會包含所有檢視元素（欄、篩選器和群組）。

共用檢視：

1. 在&#x200B;**檢視**&#x200B;下拉式清單中，將滑鼠停留在您要共用的&#x200B;**我的檢視**&#x200B;中的檢視上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-icon.png)，然後按一下&#x200B;**共用**。
1. 在「共用」對話方塊中，輸入您要共用檢視的使用者、專案團隊、群組、公司或工作角色的名稱，然後在它們出現時從清單中選取它們。

   您可以授予收件者下列許可權：

   * **檢視**：使用者可以將檢視套用至清單，但不能共用它。

     當檢視存取權使用者更新檢視時，這些變更會儲存到使用者的個人偏好設定中。 檢視名稱（在使用者的&#x200B;**共用檢視**&#x200B;中）上的藍點顯示個人更新已套用至檢視。

   * **管理**：使用者可以重新命名、共用或刪除檢視，以及編輯檢視的元素。

     當「管理存取權」使用者變更檢視時，所有擁有共用檢視的使用者都會在檢視套用至清單時看到這些更新。

1. 按一下「**儲存**」。

   如果您與某個使用者共用一個檢視，然後移除該存取權，則該檢視會從使用者的&#x200B;**共用檢視**&#x200B;中移除。 如果移除使用者存取權時，已將共用檢視套用至清單，則會套用系統預設檢視。

### 複製檢視

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

當您共用一個檢視且您沒有許可權編輯時，您可以複製該檢視並以新名稱儲存它。 您必須先對檢視進行變更，才能進行複製。

1. 在「檢視」下拉式清單中，將滑鼠停留在您修改設定且想要複製的&#x200B;**共用檢視**&#x200B;中的檢視，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-icon.png)，然後按一下&#x200B;**使用偏好設定複製**。

   系統會自動建立新檢視。 所複製檢視的名稱遵循下列模式： `Original view name (copy)`它顯示在檢視的&#x200B;**我的檢視**&#x200B;區段中。

   您是此檢視的所有者，且可以重新命名、編輯、共用或刪除此檢視。 如果原始檢視的擁有者移除您對該檢視的共用存取許可權，您仍可透過複製共用原始檢視來存取您建立的檢視。

   >[!NOTE]
   >
   >**使用偏好設定複製**&#x200B;選項只有在您變更與您共用的檢視時才可用。

### 重設檢視

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

當您共用的檢視沒有編輯許可權，而您更新該檢視時，您可以將其重設為原始檢視。

1. 在&#x200B;**檢視**&#x200B;下拉式清單中，將滑鼠游標停留在您要重設的&#x200B;**共用檢視**&#x200B;中的檢視上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-icon.png)，然後按一下&#x200B;**重設為預設值**。

   檢視元素（欄、篩選器和群組）會重設為與您共用的原始設定。

   >[!NOTE]
   >
   >**重設為預設值**&#x200B;選項只有在您變更與您共用的檢視時才可用。

   ![複製和重設檢視選項](assets/glist-copy-view-shared-with-you.png)

### 在檢視中套用條件式格式

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

條件式格式可協助您根據通用准則，在檢視中反白顯示重要資訊。

1. 按一下&#x200B;**格式化儲存格**&#x200B;圖示![格式化儲存格圖示](assets/format-cells-icon.png)。 **格式**&#x200B;方塊開啟。

1. 按一下&#x200B;**新增條件**。
1. 在&#x200B;**If**&#x200B;行中，選取欄位並選擇欄位值並新增修飾元。 修正因子會根據您選擇的欄位型別而變更。

   >[!TIP]
   >
   >只有增強型清單中的可見欄位才適用於條件式格式。

1. （選擇性）按一下&#x200B;**與另一個欄位比較**&#x200B;圖示![與另一個欄位比較](assets/compare-to-another-field-icon.png)並選擇您要與所選欄位值進行比較的欄位，而不新增欄位值。 例如，您可以比較請求專案的主旨和說明欄位。

   >[!TIP]
   >
   >只有清單檢視中顯示的欄位才適用於條件式格式。 您比較的欄位必須屬於相同型別。

1. （選擇性）按一下&#x200B;**If**&#x200B;行中的「**新增條件**」，將更多條件新增至相同規則。

   >[!TIP]
   >
   >您可以在條件規則中新增最多10個條件，而且一個欄位最多可以有20個規則。

1. 按一下條件之間的&#x200B;**Or**&#x200B;聯結器，變更為&#x200B;**和**，並指示必須同時符合多個條件。 **或**&#x200B;是預設聯結器。
1. 在&#x200B;**格式**&#x200B;行中，選取欄位以指示要格式化的欄。
1. （選擇性）按一下所選欄位旁的&#x200B;**顏色圓形**&#x200B;圖示![顏色格式圖示](assets/color-format-icon.png)，展開該欄位並在&#x200B;**儲存格填滿**&#x200B;區域中選擇另一種顏色，以變更儲存格中的背景顏色，或是從&#x200B;**文字顏色**&#x200B;區域挑選一種顏色，以變更儲存格中的文字顏色。
1. 按一下&#x200B;**文字格式**&#x200B;圖示![文字格式圖示](assets/text-format-icon.png)並從下列選項中選取，以格式化儲存格中的文字：
   * 粗體
   * 斜體

1. 開啟&#x200B;**套用至列**&#x200B;設定，將格式套用至符合條件的欄位整列。

1. （選擇性）在&#x200B;**格式**&#x200B;方塊中按一下&#x200B;**新增條件**，為其他欄位新增另一個規則，並重複上述步驟。
1. （選擇性）按一下「全部清除&#x200B;**」**&#x200B;以移除所有格式設定。
1. 按一下&#x200B;**格式**&#x200B;方塊外部以關閉它。

   這會將您帶回清單檢視。
格式會立即套用至清單檢視。
**格式化儲存格**&#x200B;圖示旁有一個藍點，表示檢視已套用特殊格式。

### 篩選增強型清單中的專案

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

篩選器可協助您減少在清單中顯示的資訊量。

1. 按一下清單上方的&#x200B;**篩選器**。
1. 在[篩選]方塊中，按一下[**新增條件**]。
1. Select a field to filter by.
1. Select a filter modifier, such as &quot;Has any of,&quot; &quot;Has none of,&quot; &quot;Is before,&quot; or &quot;Is after.&quot; The modifier options are different depending on the type of field you are filtering by.
1. Select the field value or values. Depending on the field type you are filtering by, you might be prompted to select the item from a list, search for it, or use a calendar to select a date range.

   ![Filter in enhanced lists](assets/glist-filter-with-options.png)

   The filter is applied to the list automatically.

   >[!TIP]
   >
   >To apply a personalized filter, select one of the following options for a field value:
   >
   >* **Me (logged in user)** to refer to the logged in user in fields referring to users.
   >
   >* **My teams** or **My home team** to refer to your teams in fields referring to teams.
   >
   >* **My groups** or **My home group** to refer to your groups in fields referring to groups.
   >
   >* **My company** to refer to your company in fields referring to companies.
   > 
   >* **My roles** or **My primary role** to refer to your job roles in fields referring to roles.

1. Click **Add condition** to add another condition to the filter.

   You can join multiple filters by an AND or an OR connector.

1. When the filter is applied, you can open the **Filter** options again to change the filter options or clear all of the filters.

   An indicator appears on the **Filter** button when a filter is applied to the list.

   ![Filter applied indicator](assets/glist-filter-applied-indicator.png)

### Group items in an enhanced list

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

Groupings separate the objects on the list into areas based on specific criteria.

Workfront provides a limited number of predefined groupings and you cannot modify them.

1. Click **Grouping** above the list.
1. Select a grouping to organize your list.

   ![Select a grouping](assets/glist-grouping-choose-a-group-by.png)

1. Click **Collapse all** to display the list with all the groupings collapsed. The default option is to display the list with all groupings expanded.
1. When the grouping is applied, you can open the Group options again to collapse or expand all of the groupings at once, change the grouping to group by a different field, or clear all of the groupings.

   ![Grouping in enhanced lists](assets/glist-group-by-due-date-priorities.png)

   An indicator appears on the **Grouping** button when a grouping is applied to the list.

   ![Grouping applied indicator](assets/glist-grouping-applied-indicator.png)

### Sort in an enhanced list

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

To sort individual columns:

1. Hover over the column, then click the down arrow and select **Sort**.

   An icon next to a column name indicates that the list is sorted by the values in that column, and the direction of the sort.

   >[!NOTE]
   >
   >Some columns might not be sortable, depending on the list.

   ![Sort by a column](assets/glist-sort-by-column.png)

1. (Optional) To sort your work within a grouping, click **Grouping**, go to the line of the applied grouping, click on the sorter dropdown, and select an ascending or descending order.

   ![Sort in a grouping](assets/sort-in-groups.png)

   >[!TIP]
   >
   >The sorting order differs based on the field type you sort by.

### Search in an enhanced list

>[!NOTE]
>
>並非所有增強型清單都具有本節所述的所有元素。

1. Type a keyword you want search by in the Search box in the upper-right corner of the list. The results are highlighted in the list as you type.

   ![Search term highlighted](assets/glist-search-highlighted.png)

   >[!NOTE]
   >
   >The search looks at all columns in all list items. If the list is long, the search includes items that you may need to scroll to see. When the list is filtered, the search only looks at what is currently displayed.


