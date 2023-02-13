---
title: 授予方案的存取權
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中方案的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 169f6357-1fbb-43e0-83af-1c4be682ddbf
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# 授予方案的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對方案的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

如需使用自訂存取層級來管理使用者對Workfront中其他物件類型的存取權限的相關資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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

## 使用自定義訪問級別配置對程式的用戶訪問

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 或 **編輯** 按鈕，然後選擇要授予的功能 **微調您的設定**.

   如需每個存取層級的使用者可搭配程式執行哪些作業的詳細資訊，請參閱區段 [方案](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

   >[!NOTE]
   >
   >為特定類型的對象配置訪問級別設定時，該配置不會影響用戶對級別較低的對象的訪問。 例如，您可以限制用戶刪除其訪問級別中的程式，但這不會限制用戶刪除與程式排名較低的項目。有關對象層次結構的詳細資訊，請參閱部分 [對象的相互依存和層次](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

   建立存取層級後，您可將其指派給使用者。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按許可證類型訪問程式

如需每個存取層級的使用者可搭配程式執行哪些作業的詳細資訊，請參閱區段 [方案](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 訪問共用程式

作為程式的所有者或建立者，您可以通過授予其他用戶權限來與其共用，如 [共用方案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md).

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
