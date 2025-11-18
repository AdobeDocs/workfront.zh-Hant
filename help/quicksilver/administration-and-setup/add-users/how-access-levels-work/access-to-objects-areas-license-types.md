---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 透過新授權取得物件與區域
description: 下表告訴你每個 Adobe Workfront 授權允許的最高存取層級（編輯或檢視），適用於 Workfront 中的物件和區域。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 29af5a01c1d5fcec35ac0061a478e5721f6770c0
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 23%

---

# 透過新授權取得物件與區域的存取權

<!-- Audited: 2/2024 -->

下表告訴你每個 Adobe Workfront 授權允許的最高存取層級（編輯或檢視），適用於 Workfront 中的物件和區域。

* **檢視**：使用者可以檢視並分享項目。
* **編輯**：使用者可以建立、編輯、刪除及分享項目。

  >[!NOTE]
  >
  >當其他使用者分享物件時，分享者可以指定權限，限制其編輯權限。 欲了解更多資訊，請參閱 [物件](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)共享權限概述。

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
        <td>報告、儀表板與行事曆</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>觀*</td>
        <td>查看（僅限行事曆，無分享權限）</td>
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
        <td>檢視（無分享權限）</td>
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
        <td>財務數據</td>
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

&#42; 持有貢獻者授權的使用者只能查看與他們共享的報告、儀表板和行事曆。

>[!NOTE]
>
>* 擁有輕量授權或貢獻者授權的使用者分享能力有限。 欲了解更多資訊，請參閱 [授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。
>
>* 外部使用者無法在 Workfront 中搜尋項目。 他們可以查看專門與他們共享的文件和行事曆。 他們也能看到與他們分享物品的使用者。
>
>* 貢獻者用戶和外部使用者無法看到系統性分享的內容。  必須明確地與他們分享。

您可以在以下文章中找到關於每個物件與區域存取等級允許的詳細資訊：

* [專案補助取得](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [授權任務存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [授權議題存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [授權取得文件](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [授權作品集存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [授予計畫存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [授權存取報告、儀表板和行事曆](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [授權存取篩選器、檢視和群組](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [授權使用者存取權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [授權團隊存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [授權範本存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [授權取得財務資料](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [授權資源管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [授權使用情境規劃器](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [授權存取 Adobe Workfront 目標](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
