---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文字模式語法概觀
description: 您可以使用文字模式介面在清單和報告中建立更複雜的檢視、篩選器、分組和自訂提示。 使用文字模式，您可以存取在標準模式介面中無法使用的欄位及其屬性。
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: dcbb55f57d189c715cc1111fde3c4bc597495851
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 0%

---

# 文字模式語法概觀

您可以使用文字模式介面在清單和報告中建立更複雜的檢視、篩選器、分組和自訂提示。 使用文字模式，您可以存取在標準模式介面中無法使用的欄位及其屬性。

有關開始前文字模式的資訊和考量事項，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

如需所有可報告欄位及其屬性的完整清單，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

如需使用文字模式建立報表的詳細資訊，包括類別、影片和教學課程，請造訪Adobe Experience League網站上的「學習」區段。

## 有關文字模式語法的考量事項

* 您必須先瞭解Adobe Workfront語法，才能開始以文字模式建立報表元素。 文字模式的Workfront語法是此應用程式所獨有的，並具有您必須熟悉的唯一特性。
* 在報表中開始使用文字模式之前，強烈建議您先參加進階報表課程，以更深入地瞭解我們的文字模式語言。 <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* 您可以使用標準模式介面自訂檢視、篩選器和群組。 不過，您只能使用文字模式來建置自訂提示。

## 以文字模式建立報表元素的通用准則

以文字模式建立任何報表或清單元素時，以下是常見的准則：

* 參考Workfront資料庫中的物件或屬性時，請一律使用駝峰式大小寫。
* 請記住Workfront中的物件階層。 檢視、篩選和群組之間有下列差異：

   * 您可以在檢視中顯示與報表或清單物件相距三個物件的物件。
   * 您不能在群組、篩選或自訂提示中參照遠離主物件2個以上的物件。

  **範例：** 您可以在任務檢視中顯示Portfolio擁有者的名稱或GUID：


  `valuefield=project:portfolio:ownerID`

  您不能在任務檢視中群組、篩選或提示Portfolio擁有者：

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  在這些範例中，Portfolio擁有者ID是三個物件，與清單的物件不同。

  如需Workfront中物件階層的相關資訊，請參閱：

   * [瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API總管](../../../wf-api/general/api-explorer.md)

* 儘可能使用萬用字元，讓您的報告和清單更動態，並避免針對不同使用者和類似時間表重複使用它們。

## 駝峰式大小寫概觀

在文字模式中參考Workfront欄位或其屬性時，Workfront會要求您以駝峰式大小寫輸入其名稱。 在這種情況下，單一名稱欄位會以小寫拼寫。 複合欄位的拼字方式如下：

`camelCaseSyntax`

>[!IMPORTANT]
>
>所有報表元素都遵循此大小寫模式。

駝峰式大小寫的特點是：

* 第一個字詞一律以小寫字母開頭。
* 下列字詞一律以大寫字母開頭。
* 字詞之間沒有空格。

**範例：** 若要參考專案的實際完成日期，您在建置文字模式報表元素時所使用的欄位名稱是

`actualCompletionDate`

## 各種報表元素的文字模式語法

使用文字模式建立下列報表元素集合時，其語法存在下列相似性：

* 檢視和分組的程式碼行和語法類似。

  如需以文字模式建立檢視和群組時，其程式碼關鍵行的相關資訊，請參閱：

   * [使用文字模式編輯檢視](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [編輯群組中的文字模式](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 篩選和自訂提示的程式碼行和語法類似。

  如需詳細資訊，請參閱：

   * [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 檢視和群組的語法

建置檢視和分組時的程式碼行類似。

如需建立檢視和群組的相關資訊，請參閱下列文章：

* [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

檢視或分組最重要的程式碼行是用來識別檢視欄或分組中參考的物件的行。 這行程式碼的開頭可能為 `valuefield` 或 `valueexpression` 根據此欄位是Workfront資料庫欄位的直接參照，還是數個欄位之間的計算。

下表列出檢視或群組中最常見的程式碼行：

| 代碼行 | 說明 |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | 識別檢視欄或分組中參照的物件。 這是參照物件的直接參照。 |
| `valueexpression` | 識別檢視欄或分組中參照的物件。 這是在數個欄位之間的計算。 |
| `valueformat` | 識別Workfront傳回valuefield或valueexpression行中所指定值的格式。 |
| `width` | 識別欄的寬度（畫素）。 |
| `stretch` | 識別哪些欄佔用檢視不需要的額外空間。 |

>[!TIP]
>
>* 雖然下列範例中的程式碼行在檢視和分組之間類似，請永遠記住，分組的每行程式碼都以分組編號開頭。
>
>  若要依專案清單或報表中的專案名稱分組，請使用下列第一層分組行：
>
>  `group.0.valuefield=name`
>  
>* 如果您在同一欄的檢視中編輯多個欄（與共用欄的情況相同），請記住，每個欄的每一行程式碼都以欄編號開頭。
>
>  使用下列格式來識別檢視的第一欄：
>
>  `column.0.valuefield=name`
>  
>  如需共用欄的詳細資訊，請參閱 [檢視：合併一個共用欄中多個欄的資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` 檢視和群組的語法概觀

`Valuefield=` 是檢視和群組中的關鍵程式碼行，可識別您直接參照的物件。

分組和檢視的直接參考欄位語法相同。

使用參照Workfront物件時，適用下列規則 `valuefield` 行：

* 使用駝峰式大小寫直接參考欄位。

  **範例：** 若要在作業檢視中參考「作業實際完成日期」，請使用下列明細行：

  `valuefield=actualCompletionDate`

* 使用駝峰式大小寫和冒號來分隔相同物件彼此相關的欄位。

  **範例：** 若要在任務檢視中參考「專案計畫完成日期」，請使用下列明細行：

  `valuefield=project:plannedCompletionDate`

  如需物件在Workfront資料庫中如何相互參照的詳細資訊，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

* 參考自訂欄位時，請使用與介面中顯示的欄位完全相同的名稱。

  **範例：** 若要在任務檢視中參照標示為「其他詳細資訊」的專案自訂欄位，請使用以下行：

  `valuefield=project:Additional Details`

#### `Valueexpression` 檢視和群組的語法概觀

您可以取代 `valuefield=` 程式碼行 `valueexpression=` 當您想要在2個或更多欄位之間參考計算時，在文字模式中建立檢視和群組時。

>[!TIP]
>
>雖然您可以建立可在報表中顯示的計算欄位，但計算檢視和分組更動態。 每次執行報表或顯示清單時，計算的檢視和群組都會以新資訊重新整理。
>
>如需有關在檢視中建立計算欄的資訊，請參閱 [計算自訂欄位與計算欄的比較](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

建立計算群組類似於在檢視中建立計算欄。

使用參照Workfront物件時，適用下列規則 `valueexpression` 行：

* 使用駝峰式大小寫直接參照欄位，並以大括弧括住每個欄位。

  **範例：** 若要使用在工作列中顯示任務名稱欄位 `valueexpression`，使用下列行：

  `valueexpression={name}`


* 使用駝峰式大小寫和句號來分隔彼此相關的欄位。

  **範例：** 若要在任務報告中顯示與任務名稱串連的專案名稱，請使用下列行：

   * 在檢視中：

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * 在群組中：

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  如需物件在Workfront資料庫中如何相互參照的詳細資訊，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

* 參照自訂欄位時，請使用下列規則：

   * 使用與介面中顯示的欄位完全相同的名稱。
   * 在欄位名稱前面加上「DE：」。
   * 以大括弧將欄位括住。
   * 以句點分隔與物件相關的欄位。

  **範例：** 若要在值運算式行的任務檢視中顯示「其他詳細資訊」專案自訂欄位，請使用下列行：

  `valueexpression={project}.{DE:Additional Details}`

* 您可在中使用萬用字元 `valueexpression` 但不在 `valuefield` 行。

  如需萬用字元的詳細資訊，請參閱 [萬用字元篩選器變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` 檢視和群組的概觀

檢視或分組中第二重要的一行程式碼為 `valueformat=` 行。 這會告訴Workfront要以哪種格式傳回您在 `valuefield` 或 `valueexpression` 行。 雖然您可以使用各種格式來 `valueformat` 行數，我們建議您在使用時 `valueexpression`：

`valueformat=HTML`

其他 `valueformat` 值，另請參閱下列文章：

* [文字模式報表中的日期格式](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [格式化文字模式報表中的數字、貨幣和百分比值](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` 檢視概觀

`width=` 是一行程式碼，您可以在其中指定每欄的寬度（畫素）。 Workfront會提供每個欄位的建議寬度，不過根據欄位型別和格式，您可能想要進行調整。

您必須使用 `usewidths=true` 用於強制實施為欄指定的寬度的程式碼行。

**範例：** 若要顯示寬度為80畫素的欄，請使用下列線條：

`width=80`

`usewidths=true`

#### `stretch` 檢視概觀

此 `stretch` 用於識別哪些欄佔用檢視不需要的額外空間。 一般使用者的工作區使用者介面寬度約為850畫素。 也就是說，如果您有一個檢視包含四欄（每欄150畫素），則您的檢視會佔用600 / 850畫素。 UI中有250個額外的畫素，將會新增至提供延伸百分比的欄。

當您使用其他程式碼行時，會強制使用欄的延伸： `usewidths=true` 檢視中至少其中一欄。

**範例：** 若要指示欄可以在檢視中使用70%的空白空間，請使用下列行：

`stretch=70`

`usewidths=true`

### 篩選和自訂提示的語法

建立篩選的語法與建立自訂提示的語法類似。

>[!TIP]
>
>您可以先為要包含在提示中的陳述式建立篩選器，以建立自訂提示。 使用「&amp;」連線篩選器中的所有程式碼行，且各行之間不留任何空格，這會成為您的自訂提示。

如需有關建立篩選和自訂提示的資訊，請參閱：

* [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

如需有關在文字模式中建立篩選的資訊，請參閱 [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

您可以使用以下元素在文字模式中建立篩選和自訂提示：

* 參考篩選陳述式物件的程式碼行。 濾鏡物件使用駝峰式大小寫。
* 一行程式碼，參考濾鏡物件及濾鏡物件值的修飾元。 此行中的濾鏡物件使用駝峰式大小寫。

  >[!TIP]
  >
  >參考範圍時，這需要2個修正因子明細行。

* 連線多個篩選陳述式的陳述式聯結器：

   * 且

     這是篩選器陳述式之間的預設聯結器。

   * 或

     >[!TIP]
     >
     >陳述式聯結器會區分大小寫，且一律大寫。 文字模式中可省略「AND」。

* 萬用字元，讓篩選器更動態，並針對目前時間或登入的使用者自訂篩選器。 如需萬用字元的詳細資訊，請參閱 [萬用字元篩選器變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
