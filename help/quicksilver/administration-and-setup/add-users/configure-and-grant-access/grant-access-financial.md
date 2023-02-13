---
title: 授予金融資料的存取權
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以透過使用者的存取層級，定義使用者對Workfront中財務資料的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# 授予金融資料的存取權

身為Adobe Workfront管理員，您可以透過使用者的存取層級定義使用者對下列項目的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* 關於Workfront項目的財務資訊
* 資源計畫工具中的資源預算資訊

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予金融資料訪問權的考慮事項

在授與使用者存取Workfront中的財務資料時，請考量下列事項：

* 訪問級別不允許訪問財務資料的用戶不能為項目帶來風險。 如需詳細資訊，請參閱 [建立和編輯項目風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* 您還可以使用訪問級別來確定用戶可以採用哪些資源管理活動來預算或查看資源分配。 如需詳細資訊，請參閱 [授予資源管理的訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## 使用自訂存取層級設定金融資料的使用者存取權

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 或 **編輯** 按鈕，然後選擇要授予的功能 **微調您的設定**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. （選用）在 **允許的管理存取** 區域中，選擇以下選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">匯率</td> 
      <td> <p>在Workfront中新增貨幣。</p> <p>若沒有此存取權，使用者只能將現有貨幣新增至所建立的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td> <p>查看Workfront中對象的所有費用。</p> <p>這不允許用戶建立新的費用類型。</p> <p>若沒有此存取權，使用者只能檢視下列項目：</p> 
       <ul> 
        <li>他們管理的項目、任務或問題的費用</li> 
        <li>自費</li> 
        <li>下屬的費用</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) 例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. 完成後，按一下 **儲存**.

   建立存取層級後，您可將其指派給使用者。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 共用財務資訊的存取

您可以授予其權限，以與其他使用者共用專案、任務或問題的財務資訊，如 [共用物件的財務權限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

當您與其他使用者共用任何物件時，收件者對其的權利由兩項內容的組合所決定：

* 您授予物件收件者的權限
* 對象類型的收件人的訪問級別設定

## 按許可證類型訪問財務資訊

有關每個訪問級別的用戶可以使用財務資訊的資訊，請參閱 [財務資料](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 通過設定

下列資訊可協助您了解如何使用存取層級設定來控制使用者對財務資料的存取。

### 無權存取

無權存取金融資料的使用者無權存取下列項目：

* 項目和任務對象下的財務科
* 業務案例
* 開單費率和開單記錄
* 按用戶首選項按小時成本和按小時計費

   您可以使用齒輪圖示來設定 ![](assets/gear-icon-settings.png) 在上方步驟4的「檢視」按鈕上。

* 工作角色上的每小時成本和每小時計費

   您可以使用齒輪圖示來設定 ![](assets/gear-icon-settings.png) 在上方步驟4的「檢視」按鈕上。

### 檢視存取

具有金融資料檢視存取權的使用者可以檢視（無法編輯）下列項目：

* 項目和任務對象下的財務科
* 業務案例
* 開單費率和開單記錄
* 按用戶首選項按小時成本和按小時計費

   您可以使用齒輪圖示來設定 ![](assets/gear-icon-settings.png) 在上方步驟4的「檢視」按鈕上。

* 工作角色上的每小時成本和每小時計費

   您可以使用齒輪圖示來設定 ![](assets/gear-icon-settings.png) 在上方步驟4的「檢視」按鈕上。

### 編輯存取

具有金融資料編輯存取權的使用者可以檢視及編輯下列項目：

* 項目和任務對象下的財務科
* 業務案例
* 開單費率和開單記錄
* 按用戶首選項按小時成本和按小時計費

   您可以使用齒輪圖示來設定 ![](assets/gear-icon-settings.png) 在上方步驟4的「編輯」按鈕上。

* 工作角色上的每小時成本和每小時計費

   您可以使用齒輪圖示來設定 ![](assets/gear-icon-settings.png) 在上方步驟4的「編輯」按鈕上。
