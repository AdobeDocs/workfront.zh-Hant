---
title: 重設使用者的偏好設定
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您可以重設或移除Workfront系統中任何使用者的使用者偏好設定。 個別使用者也可以重設自己的使用者偏好設定。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 2%

---

# 重設使用者的偏好設定

<!-- Audited: 12/2023 -->

身為Adobe Workfront管理員，您可以重設或移除Workfront系統中任何使用者的使用者偏好設定。

個別使用者也可以重設自己的使用者偏好設定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於受影響的設定

當您重設使用者偏好設定時，某些偏好設定會恢復為系統預設值，而其他偏好設定則會清除或移除：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>喜好設定</strong> </th> 
   <th>重設後的<strong>狀態</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>檢視</td> 
   <td> <p> 已恢復為系統預設值</p> <p>不會刪除現有檢視。 您可以再次選取它們。</p> </td> 
  </tr> 
  <tr> 
   <td>篩選器</td> 
   <td> <p>已恢復為系統預設值</p> <p>不會刪除現有的篩選器。 您可以再次選取它們。</p> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td> <p>已恢復為系統預設值</p> <p>不會刪除現有群組。 您可以再次選取它們。</p> </td> 
  </tr> 
  <tr> 
   <td>最近專案清單</td> 
   <td>已清除</td> 
  </tr> 
  <tr> 
   <td>我的最愛清單</td> 
   <td>未受影響</td> 
  </tr> 
  <tr> 
   <td>使用者偏好設定</td> 
   <td> <p>已恢復為系統預設值</p> <p>電子郵件通知會恢復為系統預設值。 預設通知列在Adobe Workfront</a>中可用的<a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">事件通知中。</p> </td> 
  </tr> 
  <tr> 
   <td>使用者定義的自訂標籤</td> 
   <td>已移除</td> 
  </tr> 
  <tr> 
   <td>使用者定義的全域導覽選項</td> 
   <td>設定回版面配置範本定義，如果未指派版面配置範本，則設定為系統預設值。</td> 
  </tr> 
 </tbody> 
</table>

## 重設使用者偏好設定

{{step-1-to-setup}}

1. 選取&#x200B;**登入身份**。
1. 開始輸入您要重設其偏好設定的使用者名稱，然後在名稱出現在下拉式清單中時按一下該名稱。
1. 選取&#x200B;**登入**。
1. 在網頁瀏覽器頂端的URL欄位中，在`workfront.com`之後新增`/resetUser`。

   >[!NOTE]
   >
   >這會區分大小寫。 U必須為大寫，其餘字元必須為小寫。 例如：
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. 按&#x200B;**Enter**。
1. 若要重設所有使用者偏好設定，請選取&#x200B;**重設**。

   或

   若要僅重設自訂標籤，請選取&#x200B;**重設標籤**。
