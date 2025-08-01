---
title: 2025年第三季度專案增強功能
description: 2025年第三季度專案增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: d950346c549d22c7a8db82ce032caa24202f9126
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 0%

---

# 2025年第三季度專案增強功能

本頁說明2025年第三季度版本中針對預覽環境所進行的專案增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2025年第三季度發行週期中目前可用的所有變更清單，請參閱[2025年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

## 提出請求時的體驗更新

>[!NOTE]
>
>* 預覽： 2025年7月9日
>* 生產快速發行： 2025年7月17日
>* 適用於所有客戶的生產： 2025年7月17日

我們已更新在新的請求體驗中提出請求時的體驗。

* 可用的請求表單和路徑會出現在清單中，而不是卡片上。 最近一次出現在頂端附近的區段中。
* 所有請求表單(包括Workfront和Workfront Planning請求表單)都會顯示在清單中。 之前，只顯示前50個。
* 請求路徑和請求表單會列在個別的區段中，包括最近使用的區域及下方較大型的清單中。
* 當您搜尋請求佇列時，清單會篩選以僅顯示包含搜尋字詞的表單和路徑。 每個顯示的請求表單或路徑都會反白顯示搜尋字詞。

如需提出要求的資訊，請參閱[建立及提交要求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

## 以舊版實際時數取代現有實際時數欄位，並建立新的實際時數欄位

>[!NOTE]
>
> 預覽和生產： 2025年6月24日 

我們新增了實際時數欄位，該欄位以時數為單位儲存專案、任務和問題的記錄時間，精確到小數。 欄位以`actualWorkRequiredDouble`形式儲存在Workfront資料庫中。

現有的實際時數欄位已重新命名為舊版實際時數。 欄位會儲存專案、任務和問題的記錄時間（以分鐘為單位），並以`actualWorkRequired`形式儲存在Workfront資料庫中。

實際時數和舊版實際時數欄位都顯示在專案、任務和問題檢視與報告中。

專案、任務和問題詳細資訊區段中顯示的實際時數欄位代表新的實際時數。

>[!IMPORTANT]
>
>根據記錄時數的時間，專案、任務或問題的實際時數與舊版實際時數之間可能會出現差異。<br>
>&#x200B;>存在下列情況：
>
>* 實際時數代表自2021年5月起為專案、任務和問題記錄的時數。
>* 舊版實際時數代表專案、任務或問題存留期內的專案、任務或問題記錄時數。 這包括在2021年5月之前記錄到目前時間的小時數。
>  &#x200B;><br>您可能需要更新報告以反映新欄位及其值。
>  &#x200B;><br>Workfront使用舊版實際時數來計算實際勞力成本。

如需詳細資訊，請參閱[檢視實際時數](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)。


## 變更API呼叫實際時數在資料庫中儲存的方式

>[!NOTE]
>
>* 預覽：下一版API預計於2025年下半年推出
>* 生產環境快速發行：下一版API預計於2025年下半年推出
>* 適用於所有客戶的生產：下一版API預計於2025年下半年推出

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


