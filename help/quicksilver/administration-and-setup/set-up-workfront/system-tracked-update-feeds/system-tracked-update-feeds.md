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
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 6%

---

# 系統追蹤更新

[!DNL Adobe Workfront] 擷取特定物件上發生的活動，方法是在物件的 [!UICONTROL 更新] 區域。

此 [!UICONTROL 更新] 區域包含下列型別的更新：

* **使用者更新：** 由使用者手動輸入。 也稱為評論、回覆和附註。

  如需設定使用者更新的詳細資訊，請參閱 [設定使用者更新的偏好設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **系統更新：** 由系統自動進行。 系統更新包含簡短的附註，說明專案已發生何種變更。

  如需有關系統更新摘要及啟用方法的詳細資訊，請參閱 [設定系統更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## 有關系統追蹤更新的考量事項

* 並非所有具有「更新」區域的物件都可使用系統追蹤更新。 此 [!UICONTROL 更新] 區域可用於下列物件：

   * [!UICONTROL 專案]
   * [!UICONTROL 任務]
   * [!UICONTROL 問題]
   * [!UICONTROL 專案組合]
   * [!UICONTROL 方案]
   * [!UICONTROL 使用者]
   * [!UICONTROL 範本]
   * [!UICONTROL 範本任務]
   * [!UICONTROL 團隊]
   * [!UICONTROL 文件]
   * [!UICONTROL 時程表]
   * [!UICONTROL 本文]

     在 [!DNL Workfront]，本文是任務。
   * [!UICONTROL 反覆項目]
   * [!UICONTROL 目標]

     您必須額外擁有授權，才能存取 [!UICONTROL 目標] 區域。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL 卡片] 在展示板上

     如需卡片更新的詳細資訊，請參閱 [新增臨機卡到展示板](../../../agile/get-started-with-boards/add-card-to-board.md).


* [!DNL Workfront] 不會追蹤下列物件的任何系統更新：

   * [!UICONTROL 團隊]
   * [!UICONTROL 範本]
   * [!UICONTROL 範本任務]

<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* 使用者可以依預設檢視系統更新，也可以選擇不顯示系統更新。

  如需有關停用系統更新顯示的資訊，請參閱區段 [啟用或停用系統更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) 在文章中 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

  >[!NOTE]
  >
  >我們目前正在重新設計評論體驗和 [!UICONTROL 更新] 區域於 [!DNL Workfront].
  >
  > 使用新的註解體驗時，您無法隱藏系統更新。
  > 
  >如需有關新註解體驗的詳細資訊，請參閱 [新的評論體驗](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* Workfront會記錄下列物件的系統追蹤更新，但沒有選項可停用顯示它們：

   * [!UICONTROL 專案組合]
   * [!UICONTROL 方案]
   * [!UICONTROL 反覆項目]

* [!DNL Workfront] 管理員可以定義系統應在中追蹤的變更型別 [!UICONTROL 更新] 區域。 並非所有物件都具有 [!UICONTROL 更新] 區域也有可設定的 [!UICONTROL 更新] 摘要。 下列物件具有 [!UICONTROL 更新] 擷取系統追蹤更新摘要，但沒有可設定更新摘要的區域：

   * [!UICONTROL 文件]
   * [!UICONTROL 時程表]
   * [!UICONTROL 反覆項目]

