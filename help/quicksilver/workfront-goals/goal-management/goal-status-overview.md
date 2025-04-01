---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront目標中的目標狀態概觀
description: 目標狀態會指出目標是否作用中且目前正在記錄進度，或是非作用中、草擬或已經達成。
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 4%

---

# Adobe Workfront目標中的目標狀態概觀

<!--Audited: 4/2025-->

>[!IMPORTANT]
>
>您的組織必須具備下列專案，才能使用本文所述的功能：
>
>* 對於新計畫和授權結構：
>
>   * Ultimate Workfront計畫
>    
>* 對於目前的計畫與授權結構：
>
>   * Pro或更高版本Workfront計畫
>   * 除了Adobe Workfront授權之外，還有Workfront目標授權。
>
>請連絡您的Workfront客戶經理，以瞭解Workfront Goals授權。
> 
>如需存取Workfront目標的詳細資訊，請參閱[使用Workfront目標的需求](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md)。

## 更新Workfront目標中的目標狀態時的考量

* 您無法手動更新您建立的目標或與您共用的目標的狀態。 目標的狀態會根據您對目標採取的動作而更新。 例如，啟動目標會將草稿狀態變更為作用中。
* 根據下列規則，有些限制存在，而且您有時無法將目標的狀態變更為其他狀態：

  | 從/到 | 草稿 | 作用中 | 非使用中 | 已關閉 |
  |---|---|---|---|---|
  | 草稿 | - | 是 | 否 | 否 |
  | 作用中 | 否 | - | 是 | 是 |
  | 非使用中 | 否 | 是 | - | 否 |
  | 已關閉 | 否 | 是 | 否 | - |

* 開啟已關閉的目標也會更新目標的進度。
* 您在目標上執行的特定動作也會更新其狀態。 如需有關如何更新目標狀態的資訊，請參閱下列文章：

   * [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)
   * [在Adobe Workfront目標中啟用目標](../../workfront-goals/goal-management/activate-goals.md)
   * [刪除和停用Adobe Workfront目標中的目標](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [在Adobe Workfront目標中關閉並重新開啟目標](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Workfront目標中的目標狀態概觀

如需建立Workfront目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。

如需啟用目標的相關資訊，請參閱[在Adobe Workfront目標中啟用目標](../../workfront-goals/goal-management/activate-goals.md)。

在Workfront目標中，目標可以有下列其中一種狀態：

* [草稿](#draft)
* [作用中](#active)
* [非使用中](#inactive)
* [已關閉](#closed)

### 草稿 {#draft}

* 這是新建立目標的預設狀態。 如需建立目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。
* Workfront目標不會記錄草擬目標的進度。
* 您無法更新草擬目標的進度。
* 草稿目標缺乏進度資訊，因此無法關閉或停用。
* 草擬的目標不會有助於其他目標的進度計算，並且圖表不會考慮這些目標。
* 草擬的目標會顯示在Workfront目標的下列領域：

   * 目標清單
   * 目標校準區段（僅作為校準的目標）


>[!IMPORTANT]
>
>將目標的狀態變更為任何其他狀態後，該目標就不能再置於草稿狀態。

### 作用中 {#active}

* 您只能在草擬目標與結果、活動相關聯或將另一個目標與其對齊時，啟用草擬目標。 啟用目標會將其狀態變更為作用中。 如需啟用目標的相關資訊，請參閱[在Adobe Workfront目標中啟用目標](../../workfront-goals/goal-management/activate-goals.md)。
* Workfront目標會記錄作用中目標的進度。
* 作用中目標有助於其他目標的進度計算，並在圖形中加以考慮。
* 作用中目標會顯示在Workfront目標的下列區域中：

   * 目標清單
   * 目標對齊區段
   * 作用中目標的進度會以圖形顯示

* 您可以重新啟用「已關閉」或「非作用中」目標。

### 非使用中 {#inactive}

* 當擁有者暫時或永久停止處理作用中目標時，您可以停用該目標。 您可以保留它以取得歷史資訊。 這會將目標的狀態更新為非作用中。

  如需有關停用目標的資訊，請參閱文章[在Adobe Workfront目標中刪除及停用目標](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)中的「停用目標」一節。

* 您無法停用草擬或已關閉的目標。
* 您可以重新啟用非作用中目標並繼續處理它。
* Workfront目標不會計算非作用中目標的進度。
* 您無法更新非作用中目標的進度。
* 非作用中目標不會影響其他目標的進度計算，且圖表不會考慮這些目標。
* 非作用中的目標具有進度歷史，因為它們曾經是作用中的目標，不同於草擬的目標。
* 非作用中目標會顯示在Workfront目標的下列區域中：

   * 目標清單
   * 目標對齊區段（僅對齊的目標）

### 已關閉 {#closed}

* 當您想要指出您已達成目標，或您不再處理目標，且將來也不會進行時，可以關閉目標。 如需關閉目標的相關資訊，請參閱[在Adobe Workfront目標中關閉及重新開啟目標](../../workfront-goals/goal-management/close-and-reopen-goals.md)。

  >[!TIP]
  >
  >如果您打算稍後處理尚未達成的目標，建議您將狀態變更為非作用中，而非已關閉。

* 您無法關閉從未啟用的目標，例如草擬的目標。
* 您可以重新開啟已關閉的目標，並繼續處理該目標。
* Workfront目標停止記錄已關閉目標的進度。
* 您無法更新已關閉目標的進度。
* 封閉式目標會顯示在Workfront目標的下列區域中：

   * 目標清單
   * 目標對齊區段（僅對齊的目標）
   * 已關閉目標的資訊也會在圖形區段中考慮。
