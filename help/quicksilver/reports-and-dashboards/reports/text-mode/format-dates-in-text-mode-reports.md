---
product-area: reporting
navigation-topic: text-mode-reporting
title: 以文字模式報表格式化日期
description: 在Adobe Workfront中，日期可設定為以多種格式顯示在報表和清單中。 要建立日期格式，必須修改列中文本模式代碼的值格式行。
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# 以文字模式報表格式化日期

在Adobe Workfront中，日期可設定為以多種格式顯示在報表和清單中。 若要建立日期格式，您必須修改 `valueformat` 行。

`valueformat= [new date format]` 例如，如果希望「預計完成日期」顯示為「MM/DD/YY」，則代碼如下所示：

```
valueformat=atDate
valuefield=projectedCompletionDate
```

如果要將計畫完成日期顯示為 *Mth, DD，年*，程式碼看起來會像這樣：

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

如需使用文字模式在Workfront報表和清單中套用條件式格式的詳細資訊，請參閱 [在文字模式中使用條件式格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

您可以使用下列項目來設定日期格式

```
valueformat
```

 文本模式值：

| **格式** | 範例  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY時間 | 10/11/18中午12:00 | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 馬斯，dd,yr | 2018年10月11日 | `mediumAtDate` |
| DW, Mth，日， YR | 2018年10月11日星期一 | `partialAtDate` |
| DW, Mth，日， YR時間 | 2018年10月11日，星期一中午12:00 | `fullAtDate` |
