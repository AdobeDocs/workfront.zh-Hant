---
title: Workfront Fusion發行活動：&amp；nbsp；2021年8月30日當週
description: Workfront Fusion發行活動：&amp；nbsp；2021年8月30日當週
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Workfront Fusion發行活動： 2021年8月30日起一週

本頁說明2021年8月30日當週在Adobe Workfront Fusion中所做的所有增強功能。

如需所有最近變更的清單，請參閱[Adobe Workfront Fusion發行活動](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)。

如需Workfront Fusion中最近的錯誤修正清單，請參閱[Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)頁面，並檢查任何標示為Workfront Fusion維護更新的更新。

## 篩選觸發「Workfront >關注事件」模組的事件

1. 設定觸發「Workfront >觀看事件」模組之事件的自訂篩選器

   為了減少不必要的案例執行次數，我們已更新Workfront >觀看記錄模組以啟用事件篩選。 現在，您可以在建立webhook時設定篩選器。 這允許案例只在事件符合特定條件時觸發。

   事件篩選器目前提供下列操作：

   * 等於：只有在事件符合篩選器的條件時，才會觸發案例。 例如，您可以設定只有在特定專案中發生事件時才會觸發情境的篩選器。
   * 不等於：只有在事件不符合篩選器的條件時，才會觸發案例。 例如，您可以建立篩選器，只有在中發生的問題之事件的狀態不是「已關閉」時，才會觸發案例。

   先前，「監看記錄」模組會擷取所有記錄。 使用者只能在情境中稍後設定篩選條件來進行篩選。

   若要利用活動篩選功能，請在您的「監看活動」模組中建立新的webhook。 目前無法編輯現有的Webhook以包含此功能。 我們強烈建議您針對現有情境使用事件篩選器來建立新的Webhook。

1. 篩選掉目前連線所觸發的事件。

   為了讓您更輕鬆地設定Webhook以用於「Workfront >觀看活動」模組，我們納入最常用的活動篩選條件。 現在，webhook可選擇使用為「觀看事件」模組指定的連線，來篩選掉模組所做的任何變更。 換言之，啟用此篩選器後，與該連線相關聯的Workfront使用者所做的任何變更都無法觸發該案例。

   之前，此篩選器無法使用。 因此，Workfront模組中所做的變更更容易觸發包含這些模組的情境，這可能會導致情境在無限回圈中觸發自己。

如需「Workfront >觀看活動模組」中活動篩選器的詳細資訊，請參閱[Adobe Workfront模組](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md)。

