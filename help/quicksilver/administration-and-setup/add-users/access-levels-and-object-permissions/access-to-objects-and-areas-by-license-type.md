---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 依許可證型別存取物件與區域
description: 下表告訴您每個Adobe Workfront授權對於Workfront中的物件與區域允許的最高存取層級（編輯或檢視）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 23%

---

# 依授權型別存取物件和區域

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>本文資訊參考舊版存取層級。 如需有關目前存取層級的資訊，請參閱[新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。

下表告訴您每個Adobe Workfront授權對於Workfront中的物件與區域允許的最高存取層級（編輯或檢視）。

* 檢視：使用者可以檢閱和共用專案。
* 編輯：使用者可以建立、編輯、刪除和共用專案。

  >[!NOTE]
  >
  >當其他使用者共用物件時，共用者可以指定許可權來限制他們編輯物件的能力。 如需有關新授權型別的詳細資訊，請參閱[物件共用許可權總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

  >[!NOTE]
  >
  >本文包含舊版授權型別物件存取的相關資訊。 如需新授權型別的詳細資訊，請參閱[新存取層級總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)和[新授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。

|   | 規劃 | 工作 | 審閱 | 請求 | 外部 |
|---|---|---|---|---|---|
| 專案 | 編輯 | 編輯（沒有「建立」許可權） | 檢視 | 檢視（僅限「詳細資訊」頁面） | 無存取權 |
| 任務 | 編輯 | 編輯 | 檢視 | 檢視 | 無存取權 |
| 問題 | 編輯 | 編輯 | 編輯 | 編輯 | 無存取權 |
| 專案組合 | 編輯 | 檢視 | 檢視 | 無存取權 | 無存取權 |
| 計劃 | 編輯 | 檢視 | 檢視 | 無存取權 | 無存取權 |
| 報告、儀表板和行事曆 | 編輯 | 檢視 | 檢視 | 檢視&#42; | 檢視（僅限行事曆，無共用許可權） |
| 篩選器、視圖和分組 | 編輯 | 編輯 | 編輯 | 編輯 | 無存取權 |
| 文件 | 編輯 | 編輯 | 編輯 | 編輯 | 檢視（無共用許可權） |
| 使用者 | 編輯 | 檢視 | 檢視 | 檢視 | 檢視 |
| 團隊 | 編輯 | 編輯 | 檢視 | 檢視 | 無存取權 |
| 範本 | 編輯 | 無存取權 | 無存取權 | 無存取權 | 無存取權 |
| 財務資料 | 編輯 | 檢視（僅限專案詳細資訊中的財務區域） | 檢視 | 無存取權 | 無存取權 |
| 資源管理 | 編輯 | 檢視 | 檢視 | 無存取權 | 無存取權 |
| 情境規劃工具 | 編輯 | 編輯 | 編輯 | 無存取權 | 無存取權 |
| Workfront Goals | 編輯 | 編輯 | 編輯 | 編輯 | 無存取權 |

&#42;具有請求授權的使用者只能檢視與他們共用的報告、儀表板和行事曆。

>[!NOTE]
>
>擁有「檢閱」授權或「請求」授權的使用者共用功能有限。 如需詳細資訊，請參閱[授權總覽](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。
>
>外部使用者無法在Workfront中搜尋專案。 他們可以檢視特別與他們共用的檔案和行事曆。 他們也可以檢視與他們共用專案的使用者。

您可以在下列文章中找到有關每個物件與區域的存取層級所允許的詳細資訊：

* [授與專案的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [授與工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [授與問題的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [授與檔案的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [授與投資組合的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [授與程式的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [授與報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [授與篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [授予團隊存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [授與範本存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [授與資源管理的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [授與Scenario Planner](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的存取權
* [授予Adobe Workfront目標的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
