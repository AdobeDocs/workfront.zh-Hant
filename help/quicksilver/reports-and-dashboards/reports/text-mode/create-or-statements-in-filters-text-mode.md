---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在文字模式篩選器中建立「OR」陳述式
description: 在清單和報表中建立篩選器時，可以包含多個陳述式。
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 在文字模式篩選器中建立「OR」陳述式

在清單和報表中建立篩選器時，可以包含多個陳述式。

如需建立篩選器的相關資訊，請參閱下列文章：

* [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## 文本模式篩選器運算子

如需標準篩選介面中Adobe Workfront篩選運算子的相關資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront有2個篩選器運算子，可連結每個篩選器陳述式：

* **和**:使用AND運算子連接2個篩選語句時，您表示希望同時滿足兩個篩選語句。

   依預設，篩選器中的陳述式會以AND運算子連結。

   在文字模式介面中建立AND篩選器時，您不需要使用AND運算子。 這是假設的。

   **範例：** 要篩選「計畫完成日期」為「今天」且「完成百分比」低於100%的任務，請使用以下文本模式代碼：

   <pre>planedCompletionDate=$$TODAY</pre><pre>planededCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **或**:當使用OR運算子連接2個篩選語句時，表示希望滿足任一語句。

   >[!TIP]
   >
   >將AND陳述式變更為OR陳述式時，報表中的項目數應會增加。

   使用文字模式介面建立OR篩選器時，您必須使用OR運算子。

   **範例：** 要篩選「計畫完成日期」為「今天」或「完成百分比」低於100%的任務，請使用以下文本模式代碼：

   <pre>planedCompletionDate=$$TODAY</pre><pre>planededCompletionDate_Mod=eq</pre><pre>或:1:percentComplete=100</pre><pre>或:1:percentComplete_Mod=lt</pre>

## OR篩選器的文字模式語法

OR篩選器的文字模式語法必須包含下列項目：

* OR運算子，在每個篩選行的開頭，後面接著一個冒號、一個數字和另一個冒號，引用OR陳述式中的物件。 這包括引用篩選欄位或屬性的行，以及引用篩選修飾符的行。

   建置OR篩選器時，請遵循此模式：

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_修改=<modifier value></pre><pre>或:1:<field name in camel case>=<value></pre><pre>或:1:<field name in camel case>_修改=<modifier value></pre>

   >[!TIP]
   >
   >OR運算子區分大小寫，且一律為大寫。

   篩選器中可能有多個OR陳述式。 在此情況下，每個OR語句都會按照要應用語句的順序接收數字。

   **範例：**  要篩選「計畫完成日期」為「今天」或「完成百分比」低於100%或「新狀態」為「新狀態」的任務，請使用以下文本模式代碼：

   <pre>planedCompletionDate=$$TODAY</pre><pre>planededCompletionDate_Mod=eq</pre><pre>或:1:status=NEW</pre><pre>或:1:status_Mod=in</pre><pre>或:2:percentComplete=100</pre><pre>或:2:percentComplete_Mod=lt</pre>

* 欄位名稱或您在篩選器中參考的屬性必須以駝峰式寫入。 如需駝峰式大小寫的詳細資訊，請參閱 [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* 當您參考OR篩選器中的自訂欄位時，必須插入DE:或修飾詞語法與自訂欄位名稱之間。 您必須拼寫自訂欄位在Workfront介面中顯示的名稱。

   **範例：** 要篩選狀態為「新」或「完成百分比」低於100%的任務，或篩選名為「帳戶類型」且值為「等於」的自定義欄位，請使用以下文本模式代碼：

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>或:1:percentComplete=100</pre><pre>或:1:percentComplete_Mod=lt</pre><pre>或:2:DE：帳戶類型=資本</pre><pre>或:2:DE:Account Type_Mod=in</pre>
