---
title: 2025年第三季度報告增強功能
description: 2025年第三季度專案增強功能
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 2025年第三季度報告增強功能

本頁說明2025年第三季度版本對「預覽」環境所做的所有報告增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2025年第三季度發行週期中目前可用的所有變更清單，請參閱[2025年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

## 增強報告傳送安全性

* 預覽： 2025年6月26日
* 生產：自2025年6月26日至2025年7月9日分階段推出

我們已增強排程報告傳送，以確保Workfront通知僅傳送至允許清單中核准的電子郵件網域。

先前，如果您的組織已定義哪些電子郵件網域Workfront通知的限制，我們會在新增電子郵件時對照允許清單執行檢查。

現在，我們也會在傳送電子郵件時執行檢查，以確保輸入的電子郵件地址符合電子郵件允許清單。 這項改善的檢查會套用至與使用者相關聯的電子郵件地址，以及新增至報告收件者清單的臨時電子郵件。

如需詳細資訊，請參閱[排程自動報告傳遞](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。


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
