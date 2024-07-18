---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: 系統追蹤更新
description: Adobe Workfront會將狀態資訊記錄在物件的[!UICONTROL 更新]區域中，藉此擷取特定物件上發生的活動。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 系統追蹤更新

<!-- Audited: April, 2024-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>-->

[!DNL Adobe Workfront]會記錄物件的[!UICONTROL 更新]區段中的狀態資訊，擷取特定物件上發生的活動。

如需有關「更新」區段的資訊，請參閱[更新區段概觀](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)。

[!UICONTROL 更新]區域包含下列型別的更新：

* **使用者更新：**&#x200B;使用者手動輸入。 也稱為評論、回覆和附註。 使用者更新會顯示在物件「更新」區段的「註釋」和「全部」標籤中。

  如需設定使用者更新的詳細資訊，請參閱[設定使用者更新的偏好設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md)。

  ![](assets/updates-qs-350x125.png)

* **系統更新：**&#x200B;由系統自動進行。 系統更新包含簡短的附註，說明專案已發生何種變更。 系統更新會顯示在物件的「系統活動」和「更新」區段的「全部」標籤中。

  如需有關系統更新摘要以及如何啟用它們的詳細資訊，請參閱[設定系統更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)。

  ![](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## 有關系統追蹤更新的考量事項

並非所有具有「更新」區域的物件都可使用系統追蹤更新。

* [!UICONTROL 更新]區域可用於下列物件：

   * [!UICONTROL 專案]
   * [!UICONTROL 任務]
   * [!UICONTROL 問題]
   * [!UICONTROL Portfolio]
   * [!UICONTROL 程式]
   * [!UICONTROL 使用者]
   * [!UICONTROL 範本]
   * [!UICONTROL 範本任務]
   * [!UICONTROL 團隊]
   * [!UICONTROL 檔案]
   * [!UICONTROL 時程表]
   * [!UICONTROL 劇本]

     在[!DNL Workfront]中，劇本是任務。
   * [!UICONTROL 反複專案]
   * [!UICONTROL 目標]

     您必須有額外的授權才能存取[!UICONTROL 目標]區域。 如需詳細資訊，請參閱[使用Workfront目標的需求](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md)。
   * 主機板上的[!UICONTROL 卡片]

     如需有關卡片更新的詳細資訊，請參閱[在面板上使用連線的卡片](../../../agile/get-started-with-boards/connected-cards.md)。

* [!DNL Workfront]不會追蹤下列物件的系統更新：

   * [!UICONTROL 團隊]
   * [!UICONTROL 範本]
   * [!UICONTROL 範本任務]
   * 臨機[!UICONTROL 卡片]
   * [!UICONTROL 反複專案]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* 使用者更新顯示在「註解」標籤中，而系統更新顯示在「系統活動」和「全部」標籤中。

  如需沒有系統活動或全部標籤的物件清單，請參閱[更新區段總覽](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* 您無法新增回覆至系統更新。 然而，在2024年4月11日之前對舊版註釋體驗中的系統活動記錄所做的任何回覆，都會以唯讀形式填入系統活動標籤中。

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* [!DNL Workfront]管理員可以定義系統應在[!UICONTROL 更新]區域中追蹤的變更型別。 並非所有具有[!UICONTROL 更新]區域的物件都有可設定的[!UICONTROL 更新]摘要。 下列物件有[!UICONTROL 更新]區域，該區域會擷取系統追蹤的更新摘要，但沒有可設定的更新摘要：

   * [!UICONTROL 檔案]
   * [!UICONTROL 時程表]
   * [!UICONTROL 反複專案]
   * [!UICONTROL 目標]


