---
title: 2026年第四季報表增強功能
description: 2026年第四季報表增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 3%

---

# 2026年第四季報表增強功能

本頁說明2026年第四季版本針對預覽環境所進行的報告增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第四季版本週期目前可用的所有變更清單，請參閱[2026年第四季版本概觀](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

<!--

## Duplicate dashboards in Canvas Dashboards

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now duplicate a Canvas Dashboard using the new **Duplicate dashboard** action. This action is available to any user whose access level grants edit or create rights to Dashboards, even if they only have view access to the specific dashboard being copied. Users without edit or create rights to Dashboards do not see this action.

When you duplicate a dashboard, you can rename it, update its description and currency, and choose which widgets, dashboard filters, and dashboard prompts to carry over to the copy.

Run as user configurations on widgets are only preserved if you are the designated user or a system administrator. Sharing preferences are not copied to the new dashboard, and a confirmation message with a link to the new dashboard displays once the copy is complete.

Previously, there was no way to duplicate a dashboard; users had to rebuild dashboards from scratch to create audience-specific variations.

For more information, see 

-->

## 畫布儀表板中的核准型別欄位

>[!NOTE]
>
>適用於所有人的生產： 2026年8月28日
>[!BADGE 不在排程]{type=Neutral}內

核准實體現在包含&#x200B;**核准型別**&#x200B;欄位，可讓使用者區分校訂核准、檔案版本核准、接收核准和其他核准型別。

## 畫布儀表板中的核准術語更新

>[!NOTE]
>
>適用於所有人的生產： 2026年8月28日
>[!BADGE 不在排程]{type=Neutral}內

為了清楚起見，已重新命名下列在畫布儀表板中用於檔案和工作核准的欄位名稱：

| 前一個名稱 | 新名稱 |
| --- | --- |
| 文件核准 | 核准 |
| 文件核准階段 | 核准階段 |
| 文件核准階段參與者 | 核准階段參與者 |
| 核准流程 | 工作核准流程 |
| 核准階段 | 工作核准階段 |
| 核准者狀態 | 工作核准者狀態 |
| 等待核准 | 等待工作核准 |

此變更不會影響目前報表的運作方式。

## 畫布儀表板中的樞紐分析表報表

>[!NOTE]
>
>預覽： 2026年8月27日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

「畫布控制面板」中的新樞紐分析表報表型別，會以準確、完整的統計來彙總資料。 您可以直接在儀表板上建立計數、總和和平均等量度，然後深入研究任何總計背後的基礎記錄。

如需詳細資訊，請參閱[在畫布儀表板中建立樞紐分析表](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md)。

## 強制排程報表的結束日期

>[!NOTE]
>
>預覽： 2026年8月13日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

排程報告現在需要結束日期，以防止無限期傳送。 超過其結束日期的排程會自動停用。

現有排程已更新為結束日期，以提高可靠性並減少不必要的系統使用。 Workfront也提供可見度和警告，協助您在報表排程生命週期接近結束日期時加以管理。

如需詳細資訊，請參閱[排程自動報告傳遞](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。

## 清單和報告有原生參考欄位可用

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

您現在可以在Workfront中，將原生參考欄位新增至清單和報表。

原生參考欄位是自訂欄位。 當欄位位於附加到物件的自訂表單上時，會從物件資料填入欄位。 例如，如果欄位參考說明欄位，並且它位於附加到專案的自訂表單上，則會提取專案說明。 （如果沒有可用資料，欄位可能會顯示「N/A」。）

如需有關建立原生參考欄位的資訊，包括支援原生欄位的清單，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
如需有關新增欄位至報表的資訊，請參閱[建立自訂報表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 舊版清單和報告的多重選取欄位值順序一致

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

您現在可以在舊版清單和報告上，以一致且可預測的順序，檢視多選自訂欄位的所選選項。 欄位順序取決於欄位在自訂表單中的排列方式。

![自訂表單欄位順序符合清單或報告中選取值的順序](assets/new-field-order-multi-select.png)

以前，選取的選項會以您選取它們的順序顯示，或是以不一致的順序顯示，這會使列更難以掃描和比較。

備註：如果欄位使用文字模式，則不會套用新排序。
