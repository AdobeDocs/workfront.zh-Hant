---
content-type: release-notes
title: Adobe Workfront Planning 2027年第一季度發行活動
description: 這是Adobe Workfront Planning產品2027年第一季的發行活動。
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 65b1e818b321dd396720fb791e49e8ae9eb7af92
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%
---
# Adobe Workfront Planning 2027年第一季度發行活動

本文介紹2027年第一季度發行的Workfront Planning功能。

如需針對Adobe Workfront Planning發行之所有功能的清單，請參閱[Adobe Workfront Planning發行活動：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## 在表格檢視中更清楚顯示快速搜尋結果

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

當您在表格檢視中使用快速搜尋來尋找專案時，該檢視會排除所有不符合搜尋的記錄，並僅顯示符合的專案。

在此增強功能之前，所有記錄都會顯示與反白顯示之搜尋結果相符的記錄。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## 當跨工作區連線關閉時，允許在次要工作區中連線全域記錄型別的記錄

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

將兩種連線的全域記錄型別新增至次要工作區時，您可以關閉跨工作區連線，同時仍在本機連結記錄。

每個次要記錄型別只會針對這兩種記錄型別顯示其自己的記錄，並且可以將它們相互連線。 不再顯示全域工作區和其他次要工作區的記錄。

在此增強功能之前，如果針對連線的全域記錄型別關閉跨工作區連線，次要工作區就無法將其自己的記錄相互連結。 如果已開啟，使用者可以從全域工作區和所有其他次要工作區檢視並連結記錄。

如需詳細資訊，請參閱[跨工作區記錄型別概觀](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)。

## 在表格、時間軸和清單檢視中檢視記錄總數

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

現在，當您套用篩選器、搜尋或變更檢視時，表格、時間軸和清單檢視會自動顯示記錄總數和計數更新。 記錄計數一律會反映完整的篩選結果，並尊重您的許可權。

記錄計數會顯示在快速搜尋方塊的左側，位於表格、時間軸或清單檢視的右上角。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## 查詢欄位數字限制

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

我們將限制您可以新增到記錄型別的查閱欄位數：

* 每個記錄型別最多40個查閱欄位
* 每個記錄型別最多5個長文字查閱欄位。 連線的查閱欄位將計入其原始欄位的限制中。
* 單一長文字查閱儲存格的值最多可達50,000個字元。 如果查閱值的組合內容超過此值，則會以連線順序顯示值，直到達到限製為止。 超過它的第一個值及其後的所有值都會被忽略。 原始的連線物件欄位不會變更。

當您嘗試建立或編輯前兩個限制以外的查閱欄位時，會收到錯誤。 已超過這些限制的記錄型別不會受此變更影響。 您可以編輯欄位，但您必須未超過限制，才能新增更多查閱欄位或值。

如需詳細資訊，請參閱[Adobe Workfront Planning物件限制總覽](/help/quicksilver/planning/general/limitations-overview.md)。

## 新欄位現在只出現在您建立它們的檢視中

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

當您新增欄位到記錄型別時，它現在只顯示在您正在處理的檢視中，並隱藏在所有其他現有的檢視中。 其他檢視會維持設定狀態，如有需要，您可以取消隱藏檢視中的新欄位。

在此增強功能之前，新欄位會取消隱藏地新增到每個檢視，有時會導致不熟悉新欄位的使用者感到困惑。

如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

## 從任何檢視匯出記錄詳細資料

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

您現在可以從任何詳細資料檢視匯出記錄的詳細資訊，而無需切換到「所有欄位」檢視。

以前，只有在選取了所有欄位檢視時，才能使用匯出選項。

如需詳細資訊，請參閱[匯出記錄的詳細資料](/help/quicksilver/planning/records/export-the-record-page.md)。

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## 透過在表格和時間表檢視中載入增量資料來提高效能

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

為了改善大量記錄的效能，我們已對表格和時間表檢視進行下列改進：

* 現在，表格檢視一開始會載入前500筆記錄，當您以500筆批次捲動時，會自動載入其他記錄。
* 時間軸檢視有類似行為，但一次載入1000筆記錄，並在捲動時載入下一個1000筆。
* 快速搜尋適用於所有記錄，而不只是顯示在目前檢視中的記錄。 當您同時捲動時間軸和表格檢視時，會載入更多記錄。
* 在時間軸檢視中套用快速搜尋，且找到超過1000個專案時，您可以按一下時間軸底部的「載入更多」 ，以顯示更多符合搜尋的記錄。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)和[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## 在時間表檢視中手動群組重新排序

>[!NOTE]
>
>預覽： 2026年10月29日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

您現在可以拖放群組、子群組和記錄，以在時間軸檢視中建立自訂順序。 您的手動排列會保留在工作階段中，而且隨著規劃需求的變更，您可以在手動排序和依欄位排序之間無縫切換。

拖放功能適用於泳道和棧疊版本的時間軸檢視。

如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 全域記錄型別的商業規則

>[!NOTE]
>
>預覽： 2026年10月28日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

Workspace管理員現在可以在主要和次要工作區中，針對全域記錄型別設定商業規則。 規則會套用至新增規則的所有工作區中，相同型別的所有記錄。

全域工作區中新增的商業規則在記錄型別匯入的次要工作區中顯示為唯讀。 在次要工作區中新增的商業規則，在原始建立記錄型別的主要工作區中顯示為唯讀。 規則只有在建立時所在的工作區中才可編輯。

如需詳細資訊，請參閱[設定記錄型別商業規則](/help/quicksilver/planning/architecture/configure-business-rules.md)。

## 為Planning請求中的填寫表單功能設定預設提示設定

>[!NOTE]
>
>預覽： 2026年10月21日
>生產快速發行： 2026年11月12日
>適用於所有人的生產： 2027年1月21日

您現在可以自訂使用者在提交Planning請求時使用AI支援的填寫表單功能時看到的提示。

建立Planning請求的請求表單時，您可以建立預設提示。

如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。
