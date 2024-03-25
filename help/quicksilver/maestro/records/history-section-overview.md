---
title: 歷史記錄區段總覽
description: 您可以在Adobe Workfront規劃中記錄的右側面板中，檢閱系統對記錄所做的變更和記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 4%

---

# 歷史記錄區段總覽

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

您可以在記錄的右側面板中新增評論或回覆，對Adobe Workfront規劃記錄進行共同作業。 您也可以在此區域中檢視系統記錄的其它變更。

記錄的右側面板會顯示下列區段：

* **註解**：顯示使用者新增至記錄的評論和回覆。 如需有關管理Workfront計畫記錄中的註解的詳細資訊，請參閱 [管理記錄註解](/help/quicksilver/maestro/records/manage-record-comments.md).
* **歷史記錄**：顯示使用者對記錄欄位進行的系統記錄變更。

## 找出記錄的「歷史記錄」區段

{{step1-to-maestro}}

預設會開啟上次存取的工作區。

1. 從中選擇表格檢視 **檢視** 下拉式功能表。
1. 按一下表格檢視中的記錄名稱。

   記錄的 **詳細資料** 頁面隨即開啟。 「註解」區域預設會在右側面板中開啟。
1. 按一下 **顯示歷史記錄** 圖示 ![](assets/show-history-icon.png). 對記錄欄位所做的所有變更都會顯示在右側面板中，從最近的變更開始。
1. （可選）按一下 **隱藏歷史記錄** 圖示 ![](assets/hide-history-icon.png) 以關閉右側面板。

## 關於「歷史記錄」段落的考量事項

您可以在記錄的「詳細資訊」頁面右側面板的「歷史記錄」區段中，檢閱對記錄欄位所做的變更。

![](assets/history-area-in-comments.png)

* Workfront planning會在「歷史記錄」區段中記錄下列資訊：

   * 任何欄位變更

   * 當值變更時，欄位的舊值和新值。 舊值會以刪除線格式顯示。

   * 進行變更的使用者全名

   * 變更發生的日期和時間戳記。

* 下列型別的欄位一律會顯示舊值（以刪除線格式）和新值：

   * 文字
   * 段落
   * 貨幣
   * 日期
   * 數字
   * 百分比
   * 單選

* 只有在刪除了多個值中的至少一個時，以下型別的欄位才會以刪除線格式顯示舊值：

   * 多選
   * 連結的記錄欄位
   * 人員

  如果變更僅新增值至欄位，則不會顯示舊值，而只會顯示新欄位值。

* 核取方塊型別的欄位絕不會以刪除線格式顯示舊值。 如果欄位已編輯，則只顯示進行變更時的目前狀態。

  如需Workfront規劃欄位的詳細資訊，請參閱 [建立欄位](/help/quicksilver/maestro/fields/create-fields.md).

* 下列型別的欄位變更不會顯示在「歷史記錄」區段中：

   * 連結（查詢）欄位
   * 公式
   * 建立者
   * 建立日期
   * 上次修改者
   * 上次修改日期

* 如果欄位從系統中移除，對該欄位所做的更新會保留在「歷史記錄」區段中。 沒有跡象顯示欄位在記錄的History區段中已移除。
