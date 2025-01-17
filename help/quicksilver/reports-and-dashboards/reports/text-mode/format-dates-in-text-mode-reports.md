---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文字模式報表中的日期格式
description: 日期可以設定為在Adobe Workfront的報表和清單中以各種格式顯示。 若要建立日期格式，您必須修改欄中文字模式程式碼的valueformat行。
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 文字模式報表中的日期格式

<!-- Audited: 1/2025 -->

日期可以設定為在Adobe Workfront的報表和清單中以各種格式顯示。 若要建立日期格式，您必須修改欄中文字模式程式碼的`valueformat`行。

`valueformat= [new date format]`例如，如果您希望預計完成日期顯示為MM/DD/YY，則程式碼會如下所示：

```
valueformat=atDate
valuefield=projectedCompletionDate
```

如果您想要將計畫完成日期顯示為&#x200B;*Mth， DD， Year*，則程式碼會如下所示：

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

如需使用文字模式在Workfront報表和清單中套用條件式格式的詳細資訊，請參閱[在文字模式中使用條件式格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)。

您可以使用下列`valueformat`個文字模式值來格式化日期：

| **格式** | 範例  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY時間 | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 月、日、年 | 2018年10月11日 | `mediumAtDate` |
| DW、月、日、年 | 2018年10月11日，星期一 | `partialAtDate` |
| DW、月、日、年時間 | 2018年10月11日，星期一下午12:00 | `fullAtDate` |
