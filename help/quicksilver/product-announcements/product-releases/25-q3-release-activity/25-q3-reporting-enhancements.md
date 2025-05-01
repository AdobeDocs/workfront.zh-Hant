---
title: 2025年第三季度報告增強功能
description: 2025年第三季度專案增強功能
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 2025年第三季度報告增強功能

本頁說明2025年第三季度版本對「預覽」環境所做的所有報告增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2025年第三季度發行週期中目前可用的所有變更清單，請參閱[2025年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

## 篩選時，使用者萬用字元不再傳回帶有null值的結果

>[!NOTE]
>
>* 預覽： 2025年4月30日
>* 生產快速發行： 2025年5月15日
>* 適用於所有客戶的生產： 2025年7月17日

我們已更新在篩選報告時排除null值的使用者萬用字元行為。 此變更可協助篩選器產生更準確的結果，而非傳回未正確設定使用者的結果（空結果）。

先前，當使用者萬用字元產生null值時，報告會顯示所有也有null值的記錄。

此變更套用至下列萬用字元篩選器：

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

