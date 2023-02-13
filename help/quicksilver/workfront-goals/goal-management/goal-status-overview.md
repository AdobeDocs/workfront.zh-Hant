---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目標中的目標狀態概觀
description: 目標狀態指示目標是處於活動狀態且當前記錄進度，還是處於非活動狀態、已起草或已實現狀態。
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Adobe Workfront目標中的目標狀態概觀

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>貴組織必須具備下列條件才能使用本文所述的功能：
>
>* Pro或更高版本 [Adobe Workfront計畫](https://www.workfront.com/plans).
>* 除了Adobe Workfront授權，還有Workfront授權。
>
>請連絡您的Workfront客戶經理，以了解Workfront Target授權。

如需存取Workfront目標的詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


目標狀態指示目標是處於活動狀態且當前記錄進度，還是處於非活動狀態、已起草或已實現狀態。

## 更新Workfront目標中的目標狀態時的考量事項

* 您無法手動更新已建立或已共用給您之目標的狀態。 目標的狀態會根據您對目標採取的動作而更新。 例如，啟動目標會將草稿狀態變更為「作用中」。
* 存在某些限制，有時您無法根據下列規則將目標的狀態更改為其他狀態：

   | 從/到 | 草稿 | 使用中 | 非使用中 | 已關閉 |
   |---|---|---|---|---|
   | 草稿 | - | 是 | 否 | 否 |
   | 使用中 | 否 | - | 是 | 是 |
   | 非使用中 | 否 | 是 | - | 否 |
   | 已關閉 | 否 | 是 | 否 | - |

* 開啟已結束的目標也會更新目標的進度。
* 您在目標上執行的某些動作也會更新其狀態。 如需如何更新目標狀態的詳細資訊，請參閱下列文章：

   * [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)
   * [啟用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/activate-goals.md)
   * [刪除和停用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [在Adobe Workfront目標中關閉和重新開啟目標](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront目標中的目標狀態概觀

如需建立Workfront目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).

如需啟用目標的相關資訊，請參閱 [啟用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/activate-goals.md).

Workfront Target中的目標可以具有下列其中一種狀態：

* [草稿](#draft)
* [使用中](#active)
* [非使用中](#inactive)
* [已關閉](#closed)

### 草稿 {#draft}

* 這是新建立目標的預設狀態。 如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).
* Workfront目標沒有記錄起草目標的進展。
* 無法更新已起草目標的進度。
* 您無法關閉或停用起草的目標，因為它們缺少進度資訊。
* 起草的目標對其他目標的進度計算沒有幫助，圖表也沒有考慮這些目標。
* 起草的目標在Workfront目標的以下方面顯示：

   * 目標清單
   * 「目標對齊」部分（僅作為對齊的目標）


>[!IMPORTANT]
>
>將目標的狀態變更為其他任何狀態後，就無法再將目標置於草稿狀態。

### 使用中 {#active}

* 僅當將擬定目標與結果、活動關聯或與其協調另一個目標時，才可激活該目標。 啟用目標會將其狀態變更為「作用中」。 如需啟用目標的相關資訊，請參閱 [啟用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/activate-goals.md).
* Workfront目標籤錄了在積極目標方面的進展。
* 積極目標有助於對其他目標的進度計算，並在圖表中加以考慮。
* 作用中目標會顯示在Workfront目標的下列區域：

   * 目標清單
   * 「目標對齊」部分
   * 活動目標的進度會顯示在圖表中

* 您可以重新啟用關閉或非使用中目標。

### 非使用中 {#inactive}

* 當擁有者暫時或永久停止使用作用中目標時，您可以停用該目標。 您可以保留它以取得歷史資訊。 這會將目標的狀態更新為非作用中。

   如需停用目標的相關資訊，請參閱文章中的「停用目標」一節 [刪除和停用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* 不能停用起草的目標或關閉的目標。
* 您可以重新啟用非作用中目標，並繼續處理。
* Workfront目標不會計算非作用中目標的進度。
* 無法更新非活動目標的進度。
* 非活動目標對其他目標的進度計算沒有貢獻，圖表中沒有考慮這些目標。
* 不活動的目標有進展歷史，因為它們曾經是活動的，與起草的目標不同。
* 非作用中目標會顯示在Workfront目標的下列區域：

   * 目標清單
   * 「目標對齊」部分（僅作為對齊的目標）

### 已關閉 {#closed}

* 當您想要指出您已實現目標，或您不再致力於目標時，您可以結束目標，而您將來也不會這麼做。 如需關於結束目標的資訊，請參閱 [在Adobe Workfront目標中關閉和重新開啟目標](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >如果您打算稍後著手達成尚未達成的目標，建議您將狀態變更為「非使用中」，而非「已關閉」。

* 你無法像起草的目標那樣關閉從未啟動的目標。
* 您可以重新開啟已關閉的目標並繼續處理該目標。
* Workfront目標不再記錄已關閉目標的進展。
* 無法更新已關閉目標的進度。
* 已結束的目標會顯示在Workfront目標的下列區域：

   * 目標清單
   * 「目標對齊」部分（僅作為對齊的目標）
   * 圖表部分也考慮來自已結束目標的資訊。
