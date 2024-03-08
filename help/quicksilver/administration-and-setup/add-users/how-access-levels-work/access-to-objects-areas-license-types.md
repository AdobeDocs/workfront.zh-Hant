---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 透過新授權存取物件和區域
description: 下表告訴您每個Adobe Workfront授權對於Workfront中的物件與區域允許的最高存取層級（編輯或檢視）。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: aefa43697ae0d4edd5300acb94a9880b3cd0c94f
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 18%

---

# 透過新授權存取物件和區域

<!-- Audited: 2/2024 -->

下表告訴您每個Adobe Workfront授權對於Workfront中的物件與區域允許的最高存取層級（編輯或檢視）。

* **檢視**：使用者可以檢閱和共用專案。
* **編輯**：使用者可以建立、編輯、刪除和共用專案。

  >[!NOTE]
  >
  >當其他使用者共用物件時，共用者可以指定許可權來限制他們編輯物件的能力。 如需詳細資訊，請參閱 [物件許可權共用概觀](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>標準</td>
        <td>精簡</td>
        <td>貢獻者</td>
        <td>外部</td>
    </tr>
    <tr>
        <td>專案</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視</td>
        <td>無存取權限</td>
    </tr>
    <tr>
        <td>任務</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視</td>
        <td>檢視</td>
    </tr>
    <tr>
        <td>問題</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>無存取權限</td>
    </tr>
    <tr>
        <td>專案組合</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>無存取權限</td>
        <td>無存取權限</td>
    </tr>
    <tr>
        <td>計劃</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>無存取權限</td>
        <td>無存取權限</td>
    </tr>
    <tr>
        <td>報告、儀表板和行事曆</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視*</td>
        <td>檢視（僅限行事曆，無共用許可權）</td>
    </tr>
    <tr>
        <td>篩選器、視圖和分組</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>文件</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>檢視（無共用許可權）</td>
    </tr>
    <tr>
        <td>使用者</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視</td>
        <td>檢視</td>
    </tr>
    <tr>
        <td>團隊</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>範本</td>
        <td>編輯</td>
        <td>無存取權</td>
        <td>無存取權</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>財務資料</td>
        <td>編輯</td>
        <td>無存取權</td>
        <td>無存取權</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>資源管理</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>無存取權</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>情境規劃工具</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>無存取權</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>Workfront Goals</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>無存取權</td>
    </tr>
</table>

&#42; 具有「貢獻者」授權的使用者僅能檢視與其共用的報告、控制面板和行事曆。

>[!NOTE]
>
>擁有輕度授權或貢獻者授權的使用者共用功能有限。 如需詳細資訊，請參閱 [授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>外部使用者無法在Workfront中搜尋專案。 他們可以檢視特別與他們共用的檔案和行事曆。 他們也可以檢視與他們共用專案的使用者。

您可以在下列文章中找到有關每個物件與區域的存取層級所允許的詳細資訊：

* [授予專案存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [授與任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [授予問題的存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [授與檔案的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [授予投資組合的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [授予方案存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [授予對報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [授予對篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [授予團隊存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [授予範本存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [授與資源管理的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [授予Scenario Planner的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [授予Adobe Workfront目標的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
