---
title: Workfront Fusion發行活動：(&N)2021年8月30日當周
description: Workfront Fusion發行活動：(&N)2021年8月30日當周
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Workfront Fusion發行活動： 2021年8月30日起第一週

本頁說明2021年8月30日當周在Adobe Workfront Fusion中所做的所有增強功能。

如需所有最近變更的清單，請參閱 [Adobe Workfront Fusion發行活動](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

如需Workfront Fusion最近錯誤修正的清單，請參閱 [Workfront維護更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) 並檢查任何標示為「Workfront Fusion維護更新」的更新。

## 篩選觸發Workfront >監看事件模組的事件

1. 為觸發Workfront >監看事件模組的事件設定自訂篩選

   為了減少不必要的情境執行次數，我們已更新Workfront >監看記錄模組以啟用事件篩選。 現在，您可以在建立網頁連結時設定篩選器。 這可讓情境僅在事件符合特定條件時觸發。

   事件篩選器目前提供下列操作：

   * 等於：只有在事件符合篩選條件時才觸發案例。 例如，您可以設定篩選器，只在特定專案中發生事件時觸發案例。
   * 不等於：只有在事件不符合篩選條件時才觸發案例。 例如，您可以建立篩選器，只有在中發生的問題沒有「已關閉」狀態時，才會觸發案例。

   以前，Watch記錄模組將檢索所有記錄。 使用者只能在案例中稍後設定篩選，才能進行篩選。

   若要善用事件篩選功能，請在Watch事件模組中建立新的Webhook。 目前無法編輯現有的Webhook以包含此功能。 我們強烈建議您針對現有案例使用事件篩選器來建立新的Webhook。

1. 篩選掉目前連線所觸發的事件。

   為了讓您更輕鬆地為Workfront >監看事件模組設定WebHook，我們加入了最常見的事件篩選器。 現在，Webhook可選擇使用為Watch事件模組指定的連接來過濾模組所做的任何更改。 換言之，啟用此篩選器後，與該連線相關聯的Workfront使用者所做的任何變更都無法觸發案例。

   此篩選器之前無法使用。 因此，在Workfront模組中所做的變更較容易觸發包含這些模組的案例，而可能導致案例在無限回圈中觸發。

如需Workfront >監看事件模組中事件篩選器的詳細資訊，請參閱 [Adobe Workfront模組](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

