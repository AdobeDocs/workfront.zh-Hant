---
title: 授予資源管理的訪問權限
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中Resource Management的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# 授予資源管理的訪問權限

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對資源管理的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## 使用自定義訪問級別配置對資源管理工具的用戶訪問

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 或 **編輯** 按鈕（位於「資源管理」的右側），然後選擇要授予的功能 **微調您的設定**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在規劃工具中編輯優先順序和預算</td> 
      <td> <p>允許具有此許可證的用戶執行以下操作：</p> <p>在資源計畫器中排定項目優先順序。</p> <p>在資源計畫工具中為資源分配預算（在項目的業務案例中為「資源計畫員」和「資源預算」部分）。</p> <p>預設會啟用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理資源集區</td> 
      <td> <p>允許具有此許可證的用戶建立、編輯和刪除資源池。 預設會停用此選項。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>更新工作量平衡工具中的計畫時數</span> </td> 
      <td> <p>允許具有此許可證的用戶在更新工作負載平衡器中的用戶分配時更新工作項目的「計畫小時數」。 分配的小時總數將成為工作項的「計畫小時數」。</p> <p>預設會停用此選項。</p> <p> 如需詳細資訊，請參閱 <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作負載平衡器中管理用戶分配</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

   建立存取層級後，您可將其指派給使用者。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按許可證類型訪問資源管理

有關每個訪問級別中的用戶可以使用資源管理執行的操作的資訊，請參見部分 [資源管理](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 存取共用問題

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

當您與其他使用者共用物件時，收件者對該物件的預算或檢視資源分配的權利，由下列三項組合決定：

* 資源管理的收件人的訪問級別設定
* 使用者對財務資料的存取，如 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* 共用者為物件授予的金融資料的任何權限

如需使用者在共用物件時可授予物件之財務資料之權限的相關資訊，請參閱 [共用物件的財務權限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
