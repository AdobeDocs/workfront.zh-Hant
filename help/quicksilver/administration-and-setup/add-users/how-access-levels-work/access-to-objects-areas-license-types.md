---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 透過新授權存取物件與區域
description: 下表告訴您每個Adobe Workfront授權對於Workfront中的物件與區域允許的最高存取層級（編輯或檢視）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 22%

---

# 透過新授權存取物件和區域

<!-- Audited: 2/2024 -->

>[!NOTE]
>
>本文資訊指的是目前的存取層級。 如需舊版存取層級的資訊，請參閱[存取層級概觀](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。

下表告訴您每個Adobe Workfront授權對於Workfront中的物件與區域允許的最高存取層級（編輯或檢視）。

* **檢視**：使用者可以檢閱和共用專案。
* **編輯**：使用者可以建立、編輯、刪除和共用專案。

  >[!NOTE]
  >
  >當其他使用者共用物件時，共用者可以指定許可權來限制他們編輯物件的能力。 如需詳細資訊，請參閱[物件共用許可權總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

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
        <td>無存取權</td>
    </tr>
    <tr>
        <td>任務</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>問題</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>專案組合</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視</td>
        <td>無存取權</td>
    </tr>
    <tr>
        <td>計劃</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視</td>
        <td>無存取權</td>
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

&#42;具有貢獻者授權的使用者只能檢視與他們共用的報告、儀表板和行事曆。

>[!NOTE]
>
>* 擁有輕度授權或貢獻者授權的使用者共用功能有限。 如需詳細資訊，請參閱[授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。
>
>* 外部使用者無法在Workfront中搜尋專案。 他們可以檢視特別與他們共用的檔案和行事曆。 他們也可以檢視與他們共用專案的使用者。
>
>* 投稿人使用者和外部使用者看不到在整個系統內共用的內容。  必須明確和他們共用。

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
