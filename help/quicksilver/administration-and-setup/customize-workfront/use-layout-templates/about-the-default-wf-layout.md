---
title: 關於預設Adobe Workfront配置
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 預設版面配置是主要功能表、左側面板，以及檢視、群組和篩選器的排列，然後Adobe Workfront管理員才能使用版面配置範本進行任何變更。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: 76797ce2afb6a6a929531f02ed3a3b3f75240602
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 9%

---

# 關於預設Adobe Workfront配置

預設版面配置是主功能表![主功能表圖示](assets/main-menu-icon.png)或主功能表![主功能表圖示](assets/main-menu-icon.png) （如果可用）的排列，在Adobe Workfront管理員使用版面配置範本進行任何變更之前，左側面板以及檢視、群組和篩選器。

如需有關Workfront管理員如何藉由指派配置範本來修改使用者的預設配置的資訊，請參閱[將使用者指派給配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

>[!NOTE]
>
>使用者可以編輯其使用者設定檔偏好設定，以變更自己的版面。 如需詳細資訊，請參閱[設定我的設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)中的[偏好設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences)區段。

## 每種授權型別的預設主功能表專案

每個使用者的預設版面配置取決於其授權型別。 視指派給使用者的授權型別而定，某些使用者可能不會在「主功能表」或某些左側面板專案中看到某些區域。

貴組織可指派兩種型別的授權：

* 新授權
* 目前的授權

<!--rename the above if we change Current to Legacy-->

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

### 目前授權型別的預設主功能表

下表顯示預設的主功能表專案，以及每個目前許可證型別所顯示的左面板專案：

<table class="tg"><thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">區域圖</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">左側面板專案</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">系統管理員</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">規劃者</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">工作者</span></th>
    <th class="tg-1wig">檢閱者</th>
    <th class="tg-1wig">請求者</th>
    <th class="tg-1wig">外部使用者</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0lax">首頁</td>
    <td class="tg-0lax">首頁<br>優先順序</td>
    <td class="tg-0lax">✔ （預設登陸頁面）</td>
    <td class="tg-0lax">✔ （預設登陸頁面）</td>
    <td class="tg-0lax">✔ （預設登陸頁面）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">專案</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ </td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">專案組合</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">計劃</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">報告</td>
    <td class="tg-0lax">我的報告<br>與我共用<br>所有報告</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔ （與我共用以及左側面板中的所有報表）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ （與我共用以及左側面板中的所有報表）</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">儀表板</td>
    <td class="tg-0lax">我的儀表板<br>共用儀表板<br>所有儀表板<br>畫布儀表板*</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">行事曆</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">資源分配</td>
    <td class="tg-0lax">計畫者<br>工作負載平衡器<br>使用率<br>資源集區</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔ （左側面板中的「規劃工具與資源集區」）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">團隊</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">使用者</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">請求</td>
    <td class="tg-0lax">已提交<br>草稿</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">時程表</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">文件</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">範本</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">情境</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">展示板</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">藍圖</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ （安裝功能）</td>
    <td class="tg-0lax">✔ （僅限請求功能）</td>
    <td class="tg-0lax">✔ （僅限請求功能）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">優先順序</td>
    <td class="tg-0lax">首頁<br>優先順序</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0lax">設定</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔ （功能有限）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">我的更新</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ （預設登陸頁面）</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>

</tbody></table>

*您必須註冊畫布控制面板Beta版才能檢視此區域。 如需詳細資訊，請參閱[畫布控制面板Beta版資訊](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)。

### 新授權型別的預設主功能表

下表顯示預設的主功能表專案，以及針對每種新授權型別所顯示的左側面板專案：

<table class="tg"><thead>
  <tr>
    <th class="tg-fymr">區域圖</th>
    <th class="tg-fymr">左側面板專案</th>
    <th class="tg-fymr">系統管理員</th>
    <th class="tg-fymr">標準</th>
    <th class="tg-fymr">精簡</th>
    <th class="tg-fymr">貢獻者</th>
    <th class="tg-fymr">外部使用者</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0pky">首頁</td>
    <td class="tg-0pky">首頁<br>優先順序</td>
    <td class="tg-0pky">✔ （預設登陸頁面）</td>
    <td class="tg-0pky">✔ （預設登陸頁面）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ （預設登陸頁面）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">專案</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ </td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">專案組合</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">計劃</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">報告</td>
    <td class="tg-0pky">我的報告<br>與我共用<br>所有報告</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ （與我共用以及左側面板中的所有報表）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">儀表板</td>
    <td class="tg-0pky">我的儀表板<br>共用儀表板<br>所有儀表板<br>畫布儀表板*</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">行事曆</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">資源分配</td>
    <td class="tg-0pky">計畫者<br>工作負載平衡器<br>使用率<br>資源集區</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">團隊</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">使用者</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">請求</td>
    <td class="tg-0pky">已提交<br>草稿</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">時程表</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">文件</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">範本</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">情境</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">展示板</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">藍圖</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ （安裝功能）</td>
    <td class="tg-0pky">✔ （僅限請求功能）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">優先順序</td>
    <td class="tg-0pky">首頁<br>優先順序</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0pky">設定</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔ （功能有限）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">我的更新</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ （預設登陸頁面）</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
</tbody></table>

*您必須註冊畫布控制面板Beta版才能檢視此區域。 如需詳細資訊，請參閱[畫布控制面板Beta版資訊](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)。

<!--

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area</th> 
   <th> Left panel items </th> 
   <th> System Administrator</th> 
   <th> Planner </th> 
   <th>Worker</th> 
   <th>Reviewer</th> 
   <th>Requestor</th> 
   <th>External User</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>Projects</strong> </td> 
   <td><strong>Projects</strong> </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br>(Default landing area)</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Portfolios</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Reporting</strong> </td> 
   <td><strong>Reports</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dashboards</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Calendars</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>People</strong> (renamed to <strong>Teams</strong> for users with a Work license)</td> 
   <td><strong>Teams</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>People</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Planning</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Scheduling</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Requests</strong> </td> 
   <td>New Request </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td><strong>Requests I've Submitted</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td>✔ <br>(Default landing area)</td> 
  </tr> 
  <tr> 
   <td><strong>All Requests</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Timesheet</strong> </td> 
   <td><strong>My Timesheets</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Timesheets I Approve</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>All Timesheets</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Documents</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Setup</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>Limited Functionality</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>
-->
