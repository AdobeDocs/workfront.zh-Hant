---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文字模式篩選器中建立「OR」陳述式
description: 當您在清單和報告中建立篩選器時，可以包含多個陳述式。
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# 在文字模式篩選器中建立「OR」陳述式

當您在清單和報告中建立篩選器時，可以包含多個陳述式。

如需建立篩選的詳細資訊，請參閱下列文章：

* [篩選器總覽](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [使用文字模式編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## 文字模式篩選器運運算元

如需有關標準篩選器介面中Adobe Workfront篩選器運運算元的資訊，請參閱[篩選器概觀](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

Workfront有2個篩選器運運算元，用來連線每個篩選器陳述式：

* **AND**：當您使用AND運運算元聯結2個篩選陳述式時，表示您要同時符合兩個篩選陳述式。

  依預設，篩選器中的陳述式會由AND運運算元連線。

  在文字模式介面中建立AND篩選器時，您不需要使用AND運運算元。 假設成立。

  **範例：**&#x200B;若要篩選計畫完成日期為今天且完成百分比低於100%的任務，請使用下列文字模式代碼：

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OR**：當您使用OR運運算元聯結2個篩選陳述式時，表示您想要滿足任一陳述式。

  >[!TIP]
  >
  >將AND陳述式變更為OR陳述式時，報表中的專案數應會增加。

  使用文字模式介面建立OR篩選器時，您必須使用OR運運算元。

  **範例：**&#x200B;若要篩選計畫完成日期為今天或完成百分比低於100%的任務，請使用下列文字模式代碼：

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## OR篩選器的文字模式語法

OR篩選器的文字模式語法必須包含下列專案：

* OR運運算元，後面接著冒號、數字，以及每個篩選器行開頭參照OR陳述式中物件的另一個冒號。 這包括參考篩選欄位或屬性的明細行，以及參考篩選修飾元的明細行。

  建立OR篩選器時，請遵循此模式：

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >OR運運算元區分大小寫，且一律大寫。

  篩選器內可有多個OR陳述式。 在這種情況下，每個OR陳述式都會依照您想要套用陳述式的順序收到一個數字。

  **範例：**&#x200B;若要篩選計畫完成日期為今天、完成百分比低於100%或狀態為新的任務，請使用下列文字模式程式碼：

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* 您在篩選中參考的欄位或屬性名稱必須以駝峰式大小寫撰寫。 如需有關駝峰式大小寫的資訊，請參閱[文字模式語法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)。
* 當您在OR篩選器中參考自訂欄位時，必須在OR修飾詞語法和自訂欄位名稱之間插入DE： 。 您必須拼字自訂欄位在Workfront介面中顯示的名稱。

  **範例：**&#x200B;若要篩選狀態為「新增」或「完成百分比」低於100%的任務，或是值為「等於」且名為「帳戶型別」的自訂欄位，請使用下列文字模式代碼：

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
