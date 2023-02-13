---
title: 授予對報表、控制面板和日曆的存取權
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中報表、控制面板和日曆的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 授予對報表、控制面板和日曆的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對報表、控制面板和日曆的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

此存取也包含對外部頁面的存取。 如需外部頁面的相關資訊，請參閱 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* 如果您想要授與使用者對報表、控制面板和日曆的存取權，您也必須授予這些使用者對篩選器、檢視和群組的存取權。 如需指示，請參閱 [授予篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* 當某人與其他使用者共用報表、控制面板或行事歷時，收件者對其的權利會由兩項因素的組合決定：報表、控制面板和日曆的收件者存取層級設定 _和_ 共用者授予的報表、控制面板或日曆的任何權限
>
>如需使用者在共用報表、控制面板或行事歷時可授予的權限相關資訊，請參閱 [共用報表、控制面板和日曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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

## 使用自訂存取層級設定使用者對報表、控制面板和日曆的存取權

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 或 **編輯** 按鈕，然後選擇要授予的功能 **微調您的設定**.

   ![reports_access.png](assets/reports-access.png)

   預設會啟用下列選項：

   * **建立**
   * **刪除**
   * **檢視內建報表**:必須選取此選項，才能查看Workfront建置的報表。
   * **共用**
   * **公開共用報表**:可與沒有Workfront帳戶的任何人共用報表的公開連結，以公開共用報表。 必須選取此選項才允許此共用層級。
   * **共用全系統**:報表可與系統中擁有Workfront授權的所有人共用。 必須選取此選項才允許此共用層級。

      如需共用報表、控制面板和日曆的相關資訊，請參閱 [共用報表、控制面板和日曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

   建立存取層級後，您可將其指派給使用者。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 依授權類型存取報表、控制面板和日曆

如需每個存取層級的使用者可針對問題執行哪些動作的相關資訊，請參閱區段 [報表](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 存取共用報表、控制面板和日曆

作為報表、控制面板或日曆的擁有者或建立者，您可以授予其他使用者權限，將其共用給他們，如 [共用報表、控制面板和日曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

當您與其他使用者共用任何物件時，收件者對其的權利由兩項內容的組合所決定：

* 您授予物件收件者的權限
* 對象類型的收件人的訪問級別設定
