---
title: 重設使用者的偏好設定
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您可以重設或移除Workfront系統中任何使用者的使用者偏好設定。 個別使用者也可以重設自己的使用者偏好設定。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e25ea757129e9645f7b5f0729cd498d5947f49f2
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 3%

---

# 重設使用者的偏好設定

<!-- Audited: 12/2023 -->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽沙箱」環境中使用，並且正在分階段推出到生產環境。</span>

身為Adobe Workfront管理員，您可以重設或移除Workfront系統中任何使用者的使用者偏好設定。

個別使用者也可以重設自己的使用者偏好設定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於受影響的設定

當您重設使用者偏好設定時，某些偏好設定會恢復為系統預設值，而其他偏好設定則會清除或移除：

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

<div class="preview">

| 喜好設定 | 重設後的狀態 |
| --- | --- |
| 檢視 | 已恢復為系統預設值 <p>不會刪除現有檢視。 您可以再次選取它們。</p> |
| 篩選器 | 已恢復為系統預設值 <p>不會刪除現有的篩選器。 您可以再次選取它們。</p> |
| 群組 | 已恢復為系統預設值 <p>不會刪除現有群組。 您可以再次選取它們。</p> |
| 最近專案清單 | 已清除 |
| 我的最愛清單 | 未受影響 |
| 使用者偏好設定 | 已恢復為系統預設值 <p>電子郵件通知會恢復為系統預設值。 預設通知列在Adobe Workfront[中可用的](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)事件通知中。</p> |

</div>

## 重設使用者偏好設定

{{step-1-to-setup}}

1. 選取&#x200B;**登入身份**。
1. 開始輸入您要重設其偏好設定的使用者名稱，然後在名稱出現在下拉式清單中時按一下該名稱。
1. 選取&#x200B;**登入**。
1. 如果您的組織尚未上線至Adobe Unified Experience，請依照此步驟操作：

   * 在網頁瀏覽器頂端的URL欄位中，在`/resetUser`之後新增`workfront.com`。

     >[!NOTE]
     >
     >這會區分大小寫。 U必須為大寫，其餘字元必須為小寫。 例如：
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. 如果您的組織已上線到Adobe Unified Experience，請依照此步驟操作：

   * 在網頁瀏覽器頂端的URL欄位中，在`/resetUser`之後新增`workfront`。

     >[!NOTE]
     >
     >這會區分大小寫。 U必須為大寫，其餘字元必須為小寫。 例如：
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. 按&#x200B;**Enter**。

<div class="preview">

1. 若要重設所有使用者偏好設定，請按一下[重設]。****

   或

   若只要重設自訂標籤，請按一下&#x200B;**重設左側導覽**。

</div>
