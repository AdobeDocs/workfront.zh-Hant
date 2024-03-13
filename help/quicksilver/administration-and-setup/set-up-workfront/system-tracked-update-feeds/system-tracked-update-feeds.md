---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: 系統追蹤更新
description: Adobe Workfront會將狀態資訊記錄在物件的上，藉此擷取特定物件上發生的活動 [!UICONTROL 更新] 區域。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# 系統追蹤更新

<span class="preview">此頁面上反白顯示的資訊僅可在預覽環境中使用。</span> <!--and in the Production environment for customers who have opted for the fast release process. For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).-->

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] 擷取特定物件上發生的活動，方法是在物件的 [!UICONTROL 更新] 區域。

此 [!UICONTROL 更新] 區域包含下列型別的更新：

* **使用者更新：** 由使用者手動輸入。 也稱為評論、回覆和附註。

  如需設定使用者更新的詳細資訊，請參閱 [設定使用者更新的偏好設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **系統更新：** 由系統自動進行。 系統更新包含簡短的附註，說明專案已發生何種變更。

  如需有關系統更新摘要及啟用方法的詳細資訊，請參閱 [設定系統更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## 有關系統追蹤更新的考量事項

並非所有具有「更新」區域的物件都可使用系統追蹤更新。

* 此 [!UICONTROL 更新] 區域可用於下列物件：

   * [!UICONTROL 專案]
   * [!UICONTROL 任務]
   * [!UICONTROL 問題]
   * [!UICONTROL Portfolio]
   * [!UICONTROL 計畫]
   * [!UICONTROL 使用者]
   * [!UICONTROL 範本]
   * [!UICONTROL 範本任務]
   * [!UICONTROL 團隊]
   * [!UICONTROL 檔案]
   * [!UICONTROL 時間表]
   * [!UICONTROL Story]

     在 [!DNL Workfront]，本文是任務。
   * [!UICONTROL 反複專案]
   * [!UICONTROL 目標]

     您必須額外擁有授權，才能存取 [!UICONTROL 目標] 區域。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL 卡片] 在展示板上

     如需卡片更新的詳細資訊，請參閱 [在展示板上使用連線的卡片](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] 不會追蹤下列物件的系統更新：

   * [!UICONTROL 團隊]
   * [!UICONTROL 範本]
   * [!UICONTROL 範本任務]
   * 臨機 [!UICONTROL 卡片]
   * [!UICONTROL 反複專案]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* 以下是新版和舊版註釋體驗之間的差異：

   * 使用新的註解體驗時，使用者更新顯示在「註解」標籤中，系統更新顯示在「系統活動」中 <span class="preview">和所有</span> 索引標籤。

     如需有關新註解體驗的詳細資訊，請參閱 [新的評論體驗](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * <span class="preview">使用新的註解體驗時，您無法新增註解到系統更新。 但是，對舊版評論體驗中系統活動記錄所做的任何回覆，都會在新版評論體驗中以唯讀形式填入系統活動標籤中。</span>
   * 使用舊版評論體驗時，系統和使用者更新會顯示在一個連續的摘要中。

   * 使用舊版評論體驗時，使用者可依預設檢視系統更新，也可以選擇不顯示更新。 使用新的註解體驗時，無法停用系統更新。

     如需有關停用系統更新顯示的資訊，請參閱區段 [啟用或停用系統更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) 在文章中 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfront會記錄下列物件的系統追蹤更新，但沒有選項可停用顯示它們：

   * [!UICONTROL Portfolio]
   * [!UICONTROL 計畫]
   * [!UICONTROL 反複專案]

* [!DNL Workfront] 管理員可以定義系統應在中追蹤的變更型別 [!UICONTROL 更新] 區域。 並非所有物件都具有 [!UICONTROL 更新] 區域也有可設定的 [!UICONTROL 更新] 摘要。 下列物件具有 [!UICONTROL 更新] 擷取系統追蹤更新摘要，但沒有可設定更新摘要的區域：

   * [!UICONTROL 檔案]
   * [!UICONTROL 時間表]
   * [!UICONTROL 反複專案]
   * [!UICONTROL 目標]


