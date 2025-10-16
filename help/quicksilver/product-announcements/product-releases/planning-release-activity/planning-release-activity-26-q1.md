---
content-type: release-notes
title: Adobe Workfront Planning 2026年第一季度發行活動
description: 這是Adobe Workfront Planning產品2026年第一季的發行活動。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: ac079ad7cb4b696cb54ff5ad8ff34940d0d62913
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第一季度發行活動

本文介紹2026年第一季度發行的Workfront Planning功能。

<!--keep the sentence below for all future quarterly release pages-->

如需針對Adobe Workfront Planning發行之所有功能的清單，請參閱[Adobe Workfront Planning發行活動：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。


## 全域記錄型別，以及將全域記錄型別新增為其他工作區現有記錄型別的能力

>[!NOTE]
>
>預覽： 2025年10月16日
>>生產快速發行： 2025年11月13日
>>適用於所有人的生產： 2026年1月15日

針對具有通用工作流程的多團隊組織實作Workfront Planning時，您可能需要為關鍵記錄型別（例如行銷活動或交付專案）定義一致結構和中繼資料，這些記錄型別可以新增到每個團隊的工作區，以擷取和管理其工作。

此外，您可能需要每個團隊的工作彙總到中央層級。

在此類工作流程中，您可以確保團隊在解鎖跨團隊可見度的同時一致地擷取其工作，而無需將組織中的每個人新增到每個工作區。 您可以使用全域記錄型別來達成此目的。

您現在可以將記錄型別指定為全域，並跨多個工作區使用它。 使用者可以使用已在中央工作區中設定的相同欄位結構和連線。

如需詳細資訊，請參閱下列文章：

* [跨工作區記錄型別概觀](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [設定記錄型別跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [從另一個工作區新增現有記錄型別](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## 單一記錄型別的連線欄位新限制

>[!NOTE]
>
>預覽： 2025年10月16日
>>生產快速發行： 2025年11月13日
>>適用於所有人的生產： 2026年1月15日

我們引進了每個記錄型別30個連線欄位的限制。

注意：如果貴組織目前有一個記錄型別的連線欄位超過30個，您可以保留超過30個限制的其他欄位。 但是，您無法向超過限制的記錄型別新增更多連線欄位。 日後，將強制執行30個連線欄位的新限制。

如需詳細資訊，請參閱[連線記錄型別總覽](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

## 為選取型別的欄位選擇設定好記的值

>[!NOTE]
>
>預覽： 2025年10月16日
>>生產快速發行： 2025年11月13日
>>適用於所有人的生產： 2026年1月15日

將欄位選擇新增至單選或多選欄位時，Workfront現在會為每個選擇指派不重複的使用者友善值。 在此改善之前，Workfront產生的英數字元ID難以瞭解及用於API呼叫和其他整合。

改良時應考量下列事項：

* 新值將新增到新的欄位選擇中。 現有欄位選擇將保留其英數字元ID。

* 一個欄位的選擇值是唯一的，但可在不同欄位之間重複。

* 重新命名選擇不會更新其原始值。

* 選擇值會以小寫顯示，若為多字選擇，則會以底線分隔。 如果您使用已用作相同欄位另一個選擇名稱的標籤，Workfront會將連續數字新增至值。

如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。