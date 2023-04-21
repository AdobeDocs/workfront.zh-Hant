---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 按許可證類型訪問對象和區域
description: 下表告訴您每個Adobe Workfront授權都允許使用Workfront中的物件和區域的最高存取層級（編輯或檢視）。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 4644edd2aac8c77508e940ec42c597aa702c4df1
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 19%

---

# 按許可證類型訪問對象和區域

下表告訴您每個Adobe Workfront授權都允許使用Workfront中的物件和區域的最高存取層級（編輯或檢視）。

* **檢視**:使用者可以檢閱和共用項目。
* **編輯**:使用者可以建立、編輯、刪除和共用項目。

   >[!NOTE]
   >
   >當其他使用者共用物件時，共用者可以指定權限來限制其編輯物件的能力。 如需詳細資訊，請參閱 [對象共用權限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | 計劃 | 工作 | 檢閱 | 請求 | 外部 |
|---|---|---|---|---|---|
| 專案 | 編輯 | 編輯（不使用建立權限） | 檢視 | 檢視（僅限「詳細資料」頁面） | 無存取權限 |
| 任務 | 編輯 | 編輯 | 檢視 | 檢視 | 檢視 |
| 問題 | 編輯 | 編輯 | 編輯 | 編輯 | 無存取權限 |
| 專案組合 | 編輯 | 檢視 | 檢視 | 無存取權限 | 無存取權限 |
| 計劃 | 編輯 | 檢視 | 檢視 | 無存取權限 | 無存取權限 |
| 報表、控制面板和日曆 | 編輯 | 檢視 | 檢視 | 檢視「&#42;」 | 檢視（僅限日曆，無共用權限） |
| 篩選器、檢視和群組 | 編輯 | 編輯 | 編輯 | 編輯 | 無權存取 |
| 文件 | 編輯 | 編輯 | 編輯 | 編輯 | 檢視（無共用權限） |
| 使用者 | 編輯 | 檢視 | 檢視 | 檢視 | 檢視 |
| 團隊 | 編輯 | 編輯 | 檢視 | 檢視 | 無權存取 |
| 範本 | 編輯 | 無權存取 | 無權存取 | 無權存取 | 無權存取 |
| 財務資料 | 編輯 | 查看（僅「項目詳細資訊」中的「財務」區域） | 檢視 | 無權存取 | 無權存取 |
| 資源管理 | 編輯 | 檢視 | 檢視 | 無權存取 | 無權存取 |
| 案例規劃工具 | 編輯 | 編輯 | 編輯 | 無權存取 | 無權存取 |
| Workfront 目標 | 編輯 | 編輯 | 編輯 | 編輯 | 無權存取 |

&#42; 擁有請求授權的使用者只能檢視與他們共用的報表、控制面板和日曆。

>[!NOTE]
>
>擁有審核許可證或請求許可證的用戶的共用功能有限。 如需詳細資訊，請參閱 [Adobe Workfront授權概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) 或 [Adobe Workfront授權概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>外部使用者無法在Workfront中搜尋項目。 他們可以查看專門與他們共用的文檔和日曆。 他們也可以看到與他們共用項目的使用者。

您可以在下列文章中找到存取層級對每個物件和區域允許的詳細資訊：

* [授予專案的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [授予問題的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [授予對文檔的訪問權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [授予產品組合的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [授予方案的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [授予對報表、控制面板和日曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [授予篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [授予團隊的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [授予範本的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [授予資源管理的訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [授予方案計畫員的訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [授予Adobe Workfront目標的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
