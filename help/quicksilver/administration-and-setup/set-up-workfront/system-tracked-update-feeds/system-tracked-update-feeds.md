---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: 系統追蹤更新
description: Adobe Workfront會記錄物件的 [!UICONTROL 更新] 的上界。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# 系統追蹤更新

[!DNL Adobe Workfront] 通過記錄對象中的狀態資訊來捕獲在特定對象上發生的活動 [!UICONTROL 更新] 的上界。

此 [!UICONTROL 更新] 區域包含下列更新類型：

* **用戶更新：** 由使用者手動輸入。 也稱為評論、回覆和附註。

   ![](assets/updates-qs-350x125.png)

* **系統更新：** 由系統自動製作。 系統更新包括描述對項目發生的更改的簡要說明。

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

下列物件可以有更新：

* 專案
* 任務
* 問題
* 專案組合
* 方案
* 使用者
* 範本
* 範本工作
* 文件
* 時程表

您的 [!DNL Workfront] 許可證確定系統更新是否預設顯示在 [!UICONTROL 更新] 對象區域。 [!DNL Workfront] 具有 [!UICONTROL 計畫] 許可證中顯示系統更新 [!UICONTROL 更新] 區域。 不過，使用者可以篩選出系統更新，如 [[!UICONTROL 啟用] 或禁用系統更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) 區段 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 其他 [!DNL Workfront] 許可證預設篩選系統更新。

[!DNL Workfront] 管理員可以定義系統應在 [!UICONTROL 更新] 的上界。 並非所有對象都具有可配置 [!UICONTROL 更新] 狀態摘要。 下列物件具有 [!UICONTROL 更新] 擷取系統追蹤的更新摘要，但沒有可設定的更新狀態摘要的區域：

* 範本
* 範本工作
* 文件
* 時程表

有關係統更新摘要以及如何啟用的詳細資訊，請參閱 [配置系統更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). 如需設定使用者更新的詳細資訊，請參閱 [配置用戶更新的首選項](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
