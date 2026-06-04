---
product-area: reporting
navigation-topic: text-mode-reporting
title: 格式化文字模式報表中的數字、貨幣和百分比值
description: 包括貨幣在內的數值可設定為以各種格式顯示在Adobe Workfront的報表和清單中。
author: Courtney
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/z96Rvp54iQcZxVWJ4Evoe1Qasl-VrEZ-IrVy11n9cDc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 145
ht-degree: 6%

---

# 格式化文字模式報表中的數字、貨幣和百分比值

<!-- Audited: 1/2025 -->

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
| 1234 | `doubleAsString`<br>或<br>`int` |
| 1,234 | `doubleAsInt` |
| $1,234 | `currencyStringCurrencyRounded` |
| 1234.56 | `doubleAsDouble` |
| $1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12.34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

