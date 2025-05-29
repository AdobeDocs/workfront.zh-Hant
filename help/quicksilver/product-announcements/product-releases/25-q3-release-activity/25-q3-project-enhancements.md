---
title: 2025年第三季度專案增強功能
description: 2025年第三季度專案增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: a5a61045bad5a97fb1413fac4a5a2666b753fa83
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 2025年第三季度專案增強功能

本頁說明2025年第三季度版本中針對預覽環境所進行的專案增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2025年第三季度發行週期中目前可用的所有變更清單，請參閱[2025年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

## 變更API呼叫實際時數在資料庫中儲存的方式

>[!NOTE]
>
>* 預覽： 2025年5月27日
>* 生產快速發行： 2025年5月27日
>* 適用於所有客戶的生產： 2025年5月27日

此更新引進了專案、任務和問題實際時數儲存在資料庫中的方式變更。 從此更新開始，實際時數將使用`actualWorkRequiredDouble`的valuefield （具有以小時為單位的值）。

在此更新之前，實際時數儲存於`actualWorkRequired`的valuefield （值以分鐘為單位）。 此更新將確保在使用API呼叫計算實際時數時更準確地計算實際時數。

由於此變更，您可能需要更新任何參考原始值欄位的API呼叫。 如果您在API呼叫中使用`actualWorkRequiredExpression`的valuefield，則不應進行任何變更。

此更新不會變更計算自訂欄位欄中專案、任務和問題的實際時數的計算。

## 使用任務或問題標題中的完成百分比滑桿在中更新

>[!NOTE]
>
>* 預覽： 2025年5月27日
>* 生產快速發行： 2025年5月27日
>* 適用於所有客戶的生產： 2025年5月27日

我們更新了完成百分比滑桿處理任務和問題的方式。

下列功能現已可用：

* 當您在任務或問題的標題中滑動完成百分比藍色泡泡時，任務或問題的完成百分比現在將以五點增量更新。 在此更新之前，滑動藍色完成百分比泡泡以一點為增量更新任務或問題。

* 您可以連按兩下藍色泡泡，並手動更新為任何需要的數字，而不使用滑桿。 此功能未變更。

更新Workfront其他區域中任務和問題的完成百分比時，沒有引入其他變更。

如需詳細資訊，請參閱[檢視和更新任務的完成百分比](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md)。

## 在專案、任務和問題中使用AI助理時提高透明度

>[!NOTE]
>
>* 預覽： 2025年5月19日
>* 生產快速發行： 2025年5月19日
>* 適用於所有客戶的生產： 2025年5月19日

為了更清楚說明AI助理如何找到有關Workfront專案、任務和問題的解答，我們將此資訊新增至問題回應。 現在，AI助理在輸出中包含其搜尋資訊。 您可以使用此資訊來檢查AI助理是否正確識別您提出的問題，並了解答案的內容。

以前，AI助理的回應中不會提供此資訊。

如需有關使用AI助理取得Workfront專案相關資訊的資訊，請參閱[使用AI助理處理專案、任務和問題](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md)。
