---
title: 23.2資源管理增強
description: 23.2資源管理增強
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 93071f9c9d359ff98a269b07f81ebcf251b1f23c
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 23.2資源管理增強

本頁面說明在「預覽」環境的23.2版中所做的所有資源管理增強功能。 這些增強功能將於23.2版的生產環境中提供使用。

如需23.2版本週期中此時所有可用變更的清單，請參閱 [23.2版本概觀](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## 引入「工作時間」欄位以準確計算用戶容量

>[!NOTE]
>
>預覽版本：2023年2月16日；計畫生產發行：2023年3月2日

為了讓資源經理能夠準確計算用戶的可用性，並說明用戶投入實際、項目相關工作的時間，我們將「工作時間」概念引入Adobe Workfront。

建立或編輯用戶的配置檔案時，您可以為每個用戶定義「工作時間」欄位的值。 如需詳細資訊，請參閱 [編輯使用者的設定檔](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

「工作時間」欄位表示用戶可用於實際工作（不包括間接費用）的等效全職(FTE)時間的百分比。 工作時間必須是小數位數，值介於0和1之間。 例如，實際工作20%的可用性為0.2。

欄位的預設值為1，表示用戶將其整個FTE用於實際的項目相關工作。

經過此更新後，Workfront將根據您在「資源管理」首選項區域中的選擇，使用以下公式計算用戶的可用性：

* 預設排程:
* 用戶容量= [（計畫小時數 — 計畫例外數）* FTE — 休假時間] *工作時間
* 使用者排程：
* 用戶能力=（計畫小時數 — 計畫例外數 — 超時數）*工作時間。

如需詳細資訊，請參閱 [設定 [!UICONTROL 資源管理] 偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3415608/){target=_blank}