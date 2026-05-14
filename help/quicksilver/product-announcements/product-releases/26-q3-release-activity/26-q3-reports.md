---
title: 2026年第三季度報告增強功能
description: 2026年第三季度報告增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9a86968cf8fff2c7c930aa6c8408ab8566905cb8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# 2026年第三季度報告增強功能

本頁說明2026年第三季度版本中針對預覽環境進行的報告增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第三季度發行週期中目前可用的所有變更清單，請參閱[2026年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## 改善「畫布」控制面板報表中的資料準確度

>[!NOTE]
>
>預覽： 2026年5月14日>生產環境快速發行： 2026年6月11日>適用於所有人的生產： 2026年7月16日
>
>畫布儀表板目前是測試版。

畫布儀表板現在會建構報表查詢，以防止篩選器或欄位交叉相關記錄時產生重複列，因此計數、總和和其他彙總會傳回精確值。

以前，相關記錄之間的聯結可能會針對每個相關記錄重複一次父記錄。 例如，在篩選成指派給特定使用者之任務的專案報告中，每個專案都會針對每個相符任務重複一次。 彙總專案預算的KPI可能會顯示$6,000，而不是正確的$1,250。

「畫布」控制面板介面沒有變更。 在此版本之後，現有報表會自動傳回精確資料。
