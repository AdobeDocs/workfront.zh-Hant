---
title: 重設使用者的偏好設定
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您可以重設或移除Workfront系統中任何使用者的使用者偏好設定。 個別使用者也可以重設自己的使用者偏好設定。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# 重設使用者的偏好設定

身為Adobe Workfront管理員，您可以重設或移除Workfront系統中任何使用者的使用者偏好設定。

個別使用者也可以重設自己的使用者偏好設定。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 關於受影響的設定

當您重設用戶首選項時，某些首選項將還原為系統預設值，而其他首選項將清除或刪除：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>喜好設定</strong> </th> 
   <th><strong>重設後的狀態</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>檢視</td> 
   <td> <p> 還原為系統預設值</p> <p>未刪除現有視圖。 您可以再次選取。</p> </td> 
  </tr> 
  <tr> 
   <td>篩選器</td> 
   <td> <p>還原為系統預設值</p> <p>不會刪除現有篩選器。 您可以再次選取。</p> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td> <p>還原為系統預設值</p> <p>不會刪除現有群組。 您可以再次選取。</p> </td> 
  </tr> 
  <tr> 
   <td>最近的項目清單</td> 
   <td>已清除</td> 
  </tr> 
  <tr> 
   <td>收藏夾清單</td> 
   <td>未受影響</td> 
  </tr> 
  <tr> 
   <td>使用者偏好設定</td> 
   <td> <p>還原為系統預設值</p> <p>電子郵件通知將還原為系統預設值</p> </td> 
  </tr> 
  <tr> 
   <td>使用者定義的自訂標籤</td> 
   <td>已移除</td> 
  </tr> 
  <tr> 
   <td>用戶定義的全局導航選項</td> 
   <td>如果未分配佈局模板，則設回佈局模板定義或系統預設值。</td> 
  </tr> 
 </tbody> 
</table>

## 重設使用者偏好設定

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 選擇 **登入方式**.
1. 開始鍵入要重置首選項的用戶的名稱，然後在名稱出現在下拉清單中時按一下。
1. 選擇  **登入**.
1. 在網頁瀏覽器頂端的URL欄位中，新增 `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >區分大小寫。 U必須大寫，其餘字元必須為小寫。 例如：
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Press **輸入**.
1. 要重置所有用戶首選項，請選擇 **重設**.

   或

   若要僅重設自訂標籤，請選取 **重設標籤**.
