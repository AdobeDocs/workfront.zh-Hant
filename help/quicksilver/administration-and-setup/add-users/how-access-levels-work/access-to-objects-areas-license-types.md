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
source-git-commit: 0e690cf9cd6351ee89e32b8f1625e8493aa0ad4b
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 17%

---

# 按許可證類型訪問對象和區域

下表告訴您每個Adobe Workfront授權都允許使用Workfront中的物件和區域的最高存取層級（編輯或檢視）。

* **檢視**:使用者可以檢閱和共用項目。
* **編輯**:使用者可以建立、編輯、刪除和共用項目。

   >[!NOTE]
   >
   >當其他使用者共用物件時，共用者可以指定權限來限制其編輯物件的能力。 如需詳細資訊，請參閱 [對象共用權限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>標準</td>
        <td>輕度</td>
        <td>投稿人</td>
        <td>外部</td>
    </tr>
    <tr>
        <td>專案</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視（僅限「詳細資料」頁面）</td>
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
        <td>報表、控制面板和日曆</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>檢視*</td>
        <td>檢視（僅限日曆，無共用權限）</td>
    </tr>
    <tr>
        <td>篩選器、檢視和群組</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>無權存取</td>
    </tr>
    <tr>
        <td>文件</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>檢視（無共用權限）</td>
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
        <td>無權存取</td>
    </tr>
    <tr>
        <td>範本</td>
        <td>編輯</td>
        <td>無權存取</td>
        <td>無權存取</td>
        <td>無權存取</td>
    </tr>
    <tr>
        <td>財務資料</td>
        <td>編輯</td>
        <td>無權存取</td>
        <td>無權存取</td>
        <td>無權存取</td>
    </tr>
    <tr>
        <td>資源管理</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>無權存取</td>
        <td>無權存取</td>
    </tr>
    <tr>
        <td>案例規劃工具</td>
        <td>編輯</td>
        <td>檢視</td>
        <td>無權存取</td>
        <td>無權存取</td>
    </tr>
    <tr>
        <td>Workfront 目標</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>編輯</td>
        <td>無權存取</td>
    </tr>
</table>

&#42; 擁有貢獻者授權的使用者只能檢視與他們共用的報表、控制面板和日曆。

>[!NOTE]
>
>擁有輕型授權或貢獻者授權的使用者分享功能有限。 如需詳細資訊，請參閱 [授權概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
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
