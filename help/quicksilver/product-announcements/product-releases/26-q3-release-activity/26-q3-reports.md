---
title: 2026年第三季度報告增強功能
description: 2026年第三季度報告增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 0c7265c477030137d14e95f42eaf67580589d70b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# 2026年第三季度報告增強功能

本頁說明2026年第三季度版本中針對預覽環境進行的報告增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第三季度發行週期中目前可用的所有變更清單，請參閱[2026年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## Snowflake中Workfront Planning的自動化存取控制

>[!NOTE]
>
>所有客戶的預覽和生產： 2026年7月16日不在排程&rbrack;{type=Neutral}內

此發行版本引入了Snowflake中Workfront Planning資料的自動化、權益導向式存取管理，作為Workfront Data Connect的一部分。
首先，將安全檢視的產生延伸至Planning表格，建立下游存取控制的必要基礎，並使基於權利的授權成為可能。以此為基礎，讀取器帳戶布建現在會在建立時檢查TMS權益，並自動套用或保留Planning資料庫的授權，以確保正確無誤。
在此增強功能之前，這僅適用於Workfront。
此更新包含下列功能： 

* 自動的每日工作會偵測現有客戶的權益變更
* 新工作會根據許可權授予、撤銷或保留存取權
* 提供完整的生命週期涵蓋範圍，涵蓋布建、建立帳戶及進行中的權益變更。

[Workfront Data Connect資料字典](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)文章將在發行日期後更新。

## 新增新物件的自訂資料支援

>[!NOTE]
>
>所有客戶的預覽和生產： 2026年7月7日不在排程&rbrack;{type=Neutral}內

在2026年第二季，我們新增物件以支援Workfront的企業作業增強功能。在目前版本中，我們也會在「畫布控制面板」中新增多個新物件的自訂資料支援。

如需詳細資訊，請參閱[畫布儀表板總覽](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md)。

## 畫布控制面板提示預設和使用者偏好設定持續性

>[!NOTE]
>
>預覽： 2026年6月25日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

為了透過保留使用者的工作篩選狀態來提高使用者在控制面板和記錄之間移動的效率，控制面板管理員現在可以定義Canvas控制面板的預設提示值。 這些預設值會自動套用至所有儀表板檢視器。

當使用者更新提示時，他們的選擇會在重新整理、重新開啟或導覽到記錄並返回後儲存和還原。

管理員可隨時重設儀表板的預設狀態。 使用者也可以透過三點選單快速還原為預設值。

在此增強功能之前，儀表板提示不具有提示狀態的可配置預設或已儲存的使用者偏好設定。

如需詳細資訊，請參閱[篩選畫布控制面板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md)。

## 一次新增多個Power BI IP位址範圍至資料連線允許清單

>[!NOTE]
>
>預覽：不適用生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

Workfront管理員將Microsoft Power BI連線至Workfront Data Connect後，現在只需一個步驟，即可將整個區域的Azure IP位址範圍新增至允許清單。 在&#x200B;**Data Connect**&#x200B;的&#x200B;**IP允許清單**&#x200B;索引標籤中，**新IP位址**&#x200B;按鈕現在包含&#x200B;**新增Power BI IP位址區塊**&#x200B;選項，該選項會開啟一個對話方塊，您可以在此處貼上Microsoft已發佈的Azure IP範圍和服務標籤JSON檔案中的Power BI服務標籤專案。

這取代了先前一次新增一個Power BI CIDR區塊的工作流程，而針對發佈數十個位址首碼的地區，此工作流程相當耗時。

如需詳細資訊，請參閱[建立與Workfront Data Connect的連線](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)。


## 排序畫布儀表板清單

>[!NOTE]
>
>預覽： 2026年6月11日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日
>
>畫布儀表板目前是測試版。

您現在可以依下列任一欄來排序畫布儀表板清單： **名稱**、**描述**、**建立者**&#x200B;或&#x200B;**建立日期**。 按一下欄標題依該欄排序清單，然後再次按一下相同標題以反轉排序方向。 依預設，清單會依&#x200B;**名稱**&#x200B;從A到Z排序。當您在「畫布控制面板」清單中的標籤之間切換時，排序順序會保留。

如需詳細資訊，請參閱[使用畫布儀表板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)。

## 自訂公式中實際時數的變更

>[!NOTE]
>
>預覽： 2026年6月1日生產環境快速發行： 2026年6月1日每個人都要生產： 2026年6月1日

2025年，新的「實際時數」欄位已新增至Workfront資料庫，做為`actualWorkRequiredDouble`，而現有的「實際時數」欄位（資料庫中的`actualWorkRequired`）已重新命名為「舊版實際時數」。 如需詳細資訊，請參閱[發行說明](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md)。

在2026年6月，使用`actualWorkRequired` （舊版實際時數）的現有自訂公式已移轉為使用`actualWorkRequiredDouble` （實際時數）。 `actualWorkRequired`無法再用於計算和公式中。

此外，強烈建議在所有報表中使用`actualWorkRequiredDouble`。

取代欄位時，請注意`actualWorkRequired`以分鐘儲存值，而`actualWorkRequiredDouble`以小數精確度以小時儲存值。

如需實際時數的詳細資訊，請參閱[檢視實際時數](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)。

## 畫布控制面板報表中的自訂貨幣資料欄位

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

畫布控制面板報表現在支援自訂貨幣資料欄位做為欄、篩選器、群組和彙總，包括當在系統設定中設定多個匯率時。 當自訂貨幣資料欄位顯示為欄或彙總時，除非欄位在報表層級鎖定，否則值會轉換為在控制面板的匯率切換中選取的貨幣。

先前在新增第二個匯率貨幣後失敗並顯示「受限欄位」訊息的報表，現在會呈現。 定義多重匯率時，規劃貨幣欄位仍受限制。

如需詳細資訊，請參閱[在畫布儀表板中使用貨幣欄位](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md)。

## 改善「畫布」控制面板報表中的資料準確度

>[!NOTE]
>
>預覽： 2026年5月14日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日
>
>畫布儀表板目前是測試版。

畫布儀表板現在會建構報表查詢，以防止篩選器或欄位交叉相關記錄時產生重複列，因此計數、總和和其他彙總會傳回精確值。

以前，相關記錄之間的聯結可能會針對每個相關記錄重複一次父記錄。 例如，在篩選成指派給特定使用者之任務的專案報告中，每個專案都會針對每個相符任務重複一次。 彙總專案預算的KPI可能會顯示$6,000，而不是正確的$1,250。

「畫布」控制面板介面沒有變更。 在此版本之後，現有報表會自動傳回精確資料。

