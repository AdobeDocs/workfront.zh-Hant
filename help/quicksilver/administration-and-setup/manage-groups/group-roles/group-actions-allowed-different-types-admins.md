---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: 允許群組管理員執行的動作
description: 此表格會比較管理Workfront系統的Adobe Workfront管理員、管理最上層群組的群組管理員以及管理子群組的群組管理員可用的管理活動。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f556aa0b-71c5-48a9-8a84-72f1fbb2c86e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 3%

---

# 允許群組管理員執行的動作

此表格列出可用於下列專案的管理活動：

* 管理Workfront系統的Adobe Workfront管理員（以供比較）
* 管理最上層群組的群組管理員
* 管理子群組的群組管理員

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Workfront管理員 </th> 
   <th>群組管理員（動作僅限於管理員管理的群組）</th> 
   <th>子群組管理員（動作僅限於管理員管理的群組）</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td>重設使用者密碼</td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
  </tr> 
  <tr> 
   <td>建立和編輯使用者設定檔</td> 
   <td>✓ (A)</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
  </tr> 
  <tr> 
   <td>建立和管理子群組</td>
   <td>✓ (A) </td> 
   <td>✓ ***</td> 
   <td>✓ ***</td> 
  </tr> 
  <tr> 
   <td>在系統層級設定專案、任務和問題偏好設定</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>啟用和停用群組和子群組的專案、任務和問題偏好設定</td> 
   <td>✓ ***</td> 
   <td>✓ ***</td> 
   <td>✓ ***</td> 
  </tr> 
  <tr> 
   <td>在系統層級設定時程表和小時偏好設定</td> 
   <td>✓ (A) </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>啟用和停用群組和子群組的時程表和小時偏好設定 </td> 
   <td>✓ ***</td> 
   <td>✓ ***</td> 
   <td>✓ ***</td> 
  </tr> 
  <tr> 
   <td>在系統層級設定事件通知電子郵件</td> 
   <td>✓ (A) </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>啟用和停用群組和子群組的事件通知電子郵件</td> 
   <td>✓ *** </td> 
   <td>✓ ***</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>建立和管理自訂表單</td> 
   <td>✓ (A) </td> 
   <td>✓ **</td> 
   <td>✓ **</td> 
  </tr> 
  <tr> 
   <td>建立和管理版面配置範本</td> 
   <td>✓ (A) </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>建立和管理群組的核准流程</td> 
   <td>✓ *** </td> 
   <td>✓ ***</td> 
   <td>✓ ***</td> 
  </tr> 
  <tr> 
   <td>建立及管理團隊</td> 
   <td>✓ (A) </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>建立和管理匯率</td> 
   <td>✓ (A) </td> 
   <td>✓ **</td> 
   <td>✓ **</td> 
  </tr> 
  <tr> 
   <td>建立和管理小時型別</td> 
   <td>✓ (A) </td> 
   <td>✓ **</td> 
   <td>✓ **</td> 
  </tr> 
  <tr> 
   <td>建立和管理里程碑路徑</td> 
   <td>✓ (A) </td> 
   <td>✓ **</td> 
   <td>✓ **</td> 
  </tr> 
  <tr> 
   <td>建立和管理排程</td> 
   <td>✓ (A) </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>建立和管理公司</td> 
   <td>✓ (A) </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>建立和管理週期性時程表</td> 
   <td>✓ (A) </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>建立單一使用時程表</td> 
   <td>✓ (A)</td> 
   <td>✓ **</td> 
   <td>✓ **</td> 
  </tr> 
  <tr> 
   <td>建立和管理職務角色</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>建立並管理優先順序、嚴重性和條件</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>建立及管理風險型別</td> 
   <td>✓ (A) </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>建立和管理狀態</td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>以其他人身分登入</td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
  </tr> 
  <tr> 
   <td>檢視和還原已刪除的專案</td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
  </tr> 
  <tr> 
   <td>檢視和管理還原的專案</td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
  </tr> 
  <tr> 
   <td>檢視目前的授權分配</td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
   <td>✓ (A) </td> 
  </tr> 
  <tr> 
   <td>指派最大授權數量</td> 
   <td>✓ *** </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視稽核記錄</td> 
   <td>✓ (A) </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>使用Kick-Start匯入和匯出資料</td> 
   <td>✓ (A) </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;在群組管理員的存取層級中，必須為&#x200B;**使用者**&#x200B;設定選取&#x200B;**編輯**，並在&#x200B;**微調您的設定** ![微調設定圖示](assets/gear-icon-in-access-levels.png)中選取&#x200B;**使用者管理員（群組使用者）**。 如需詳細資訊，請參閱[授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)一文中的[設定使用者的存取權，以使用自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit)編輯使用者一節。

&#42;&#42;在群組管理員的存取層級中，必須啟用此動作的存取權。 如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

&#42;&#42;&#42;下列活動是「進階企業控制項」的一部份，不適用於「選取」計畫。 只有已購買Prime或Ultimate計畫的組織才能存取這些功能。  如需計畫的詳細資訊，請參閱[Adobe Workfront定價與封裝頁面](https://business.adobe.com/tw/products/workfront/pricing.html)。 （針對使用舊版計畫的組織，上表顯示群組和子群組管理員的活動。）

* 在群組層級設定專案、任務和問題偏好設定
* 在群組層級設定時程表和小時偏好設定
* 在群組層級設定事件通知電子郵件
* 建立及管理群組特定的核准流程
* 依主群組分配授許可權制並檢視其使用率
* 指派子群組的群組管理員
* 允許群組管理員建立子群組
