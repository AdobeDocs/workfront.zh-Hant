---
title: 23.2資源管理增強功能
description: 23.2資源管理增強功能
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 23.2資源管理增強功能

此頁面說明23.2版本對「預覽」環境所做的所有資源管理增強功能。 這些增強功能將在23.2版本的生產環境中提供。

如需23.2版本週期目前可用的所有變更清單，請參閱 [23.2版本總覽](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## 介紹「工作時間」欄位，以準確計算使用者容量

>[!NOTE]
>
>預覽版本： 2023年2月16日；預計生產版本： 2023年3月2日

為了讓資源管理員能夠準確計算使用者的可用性，並計算使用者用於實際專案相關工作的時間，我們在Adobe Workfront中引入「工作時間」概念。

當您建立或編輯每個使用者的設定檔時，可以為其定義「工作時間」欄位的值。 如需詳細資訊，請參閱 [編輯使用者設定檔](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

「工作時間」欄位代表使用者可用於實際工作（不包括額外負荷）的相當全職(FTE)時間百分比。 「工作時間」必須為介於0和1之間的十進位數字。 例如，實際工作的20%可用性為0.2。

該欄位的預設值為1，這表示使用者將其整個FTE用於實際的、專案相關的工作。

更新後，Workfront會根據您在「資源管理」偏好設定區域中的選取，使用下列公式計算使用者的可用性：

* 預設排程：
* 使用者容量= [（排程時數 — 排程例外） * FTE — 休假] *工作時間
* 使用者排程：
* 使用者產能= （排程時數 — 排程例外 — 休假） *工作時間。

如需詳細資訊，請參閱 [設定 [!UICONTROL 資源管理] 偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3415608/){target=_blank}
