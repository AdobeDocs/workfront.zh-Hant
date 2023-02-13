---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式報告中的數字、貨幣和百分比值的格式
description: 在Adobe Workfront中，數值（包括貨幣）可設定為以多種格式顯示在報表和清單中。
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---

# 文本模式報告中的數字、貨幣和百分比值的格式

在Adobe Workfront中，數值（包括貨幣）可設定為以多種格式顯示在報表和清單中。

若要修改數值格式，您必須編輯 **valueformat** 行。

例如，如果您想將「預算」欄顯示為$1000，則值格式行如下所示：

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

如需使用文字模式在Workfront報表和清單中套用條件式格式的詳細資訊，請參閱 [在文字模式中使用條件式格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

您可以使用下列值來格式化數字 `valueformat` 行：

| 範例 | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>或 <br><pre>int</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |
