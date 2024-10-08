---
title: 關於預設Adobe Workfront配置
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 預設版面配置是主要功能表、左側面板，以及檢視、群組和篩選器的排列，然後Adobe Workfront管理員才能使用版面配置範本進行任何變更。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 6%

---

# 關於預設Adobe Workfront配置

預設版面配置是主要功能表![](assets/main-menu-icon.png)或主要功能表![](assets/lines-main-menu.png) （如果可用）的排列、左側面板，以及Adobe Workfront管理員使用版面配置範本進行任何變更之前的檢視、群組和篩選器。

如需有關Workfront管理員如何藉由指派配置範本來修改使用者的預設配置的資訊，請參閱[將使用者指派給配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

>[!NOTE]
>
>使用者可以編輯其使用者設定檔偏好設定，以變更自己的版面。 如需詳細資訊，請參閱[設定我的設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)中的[偏好設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences)區段。

## 每個存取層級的預設配置

每個使用者的預設版面配置取決於其存取層級。 視指派給使用者的存取層級而定，某些使用者可能不會在主功能表或某些左側面板專案中看到某些區域。

下表顯示預設登陸區域，以及針對每個存取層級顯示的左側面板專案：

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
   <th>區域</th> 
   <th> 左側面板專案 </th> 
   <th> 系統管理員</th> 
   <th> 規劃工具 </th> 
   <th>工作者</th> 
   <th>檢閱者</th> 
   <th>請求者</th> 
   <th>外部使用者</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>專案</strong> </td> 
   <td><strong>專案</strong> </td> 
   <td>✔ <br> （預設登陸區域）</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br> （預設登陸區域）</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>專案組合</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>報告</strong> </td> 
   <td><strong>報告</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>儀表板</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>行事曆</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>人員</strong> （針對擁有工作授權的使用者重新命名為<strong>團隊</strong>）</td> 
   <td><strong>團隊</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>人員</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> <!--
   <tr> 
    <td><strong>Legacy Resource Planning</strong> </td> 
    <td>✔ </td> 
    <td>✔ </td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
   </tr>
  --> 
  <tr> 
   <td><strong>規劃</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>排程</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>要求</strong> </td> 
   <td>新請求 </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>我已提交的<strong>個要求</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br> （預設登陸區域）</td> 
   <td>✔ <br> （預設登陸區域）</td> 
  </tr> 
  <tr> 
   <td><strong>所有要求</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>時程表</strong> </td> 
   <td><strong>我的時程表</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>我核准的時程表</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>所有時程表</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>文件</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>設定</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>功能有限</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
