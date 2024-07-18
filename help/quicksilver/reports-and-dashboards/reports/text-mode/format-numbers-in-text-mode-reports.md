---
product-area: reporting
navigation-topic: text-mode-reporting
title: 格式化文字模式報表中的數字、貨幣和百分比值
description: 包括貨幣在內的數值可設定為以各種格式顯示在Adobe Workfront的報表和清單中。
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# 格式化文字模式報表中的數字、貨幣和百分比值

<!-- Audited: 2/2024 -->

包括貨幣在內的數值可設定為以各種格式顯示在Adobe Workfront的報表和清單中。

若要修改數值的格式，您必須編輯欄的&#x200B;**valueformat**&#x200B;行。

例如，如果您想要將「預算」欄顯示為$1000，則值格式行會如下所示：

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

如需使用文字模式在Workfront報表和清單中套用條件式格式的詳細資訊，請參閱[在文字模式中使用條件式格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)。

您可以使用下列欄的`valueformat`行值來格式化數字：

| 範例 | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>或<br><pre>整數</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

