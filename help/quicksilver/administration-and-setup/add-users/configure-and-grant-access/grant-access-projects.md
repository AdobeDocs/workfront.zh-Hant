---
title: 授予專案的存取權
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中專案的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# 授予專案的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對專案的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## 使用自訂存取層級設定使用者對專案的存取權

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 或 **編輯** 按鈕，然後選擇要授予的功能 **微調您的設定**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* 擁有工作授權的使用者擁有有限的專案權利。 他們可以為專案貢獻內容，但無法管理專案。
   >* 具有「審閱」許可的用戶對轉換後問題的項目具有「查看」權限，但其「查看」權限有限。
   >* 如需使用者在與他人共用專案時可授予的權限相關資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* 為特定類型的對象配置訪問級別設定時，該配置不會影響用戶對級別較低的對象的訪問。 例如，您可以限制用戶刪除其訪問級別中的項目，但這不會限制用戶刪除任務，這些任務的排名比項目低。有關對象層次結構的詳細資訊，請參閱部分 [對象的相互依存和層次](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).


1. （選用）按一下 **設定共用預設值** ，然後 **新增規則** 新增新專案的共用規則。

   具有此存取層級的使用者建立專案時，專案會自動與您在左側功能表中選取的使用者共用。

   ![](assets/project-sharing-menu.png)

   在右側的功能表中，您可以指定要如何與這些使用者共用專案：

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >如果具有此訪問級別的用戶使用項目訪問模板，則模板將覆蓋訪問級別中的共用設定。 如需專案存取範本的相關資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   您可以重複此步驟，新增您需要的存取層級專案共用規則。

1. 按一下X以關閉 **微調您的設定** 框。
1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

   建立存取層級後，您可將其指派給使用者。 如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 依授權類型存取報表、控制面板和日曆

如需每個存取層級的使用者可針對問題執行哪些動作的相關資訊，請參閱區段 [專案](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 共用專案的存取權

作為問題的擁有者或建立者，您可以授予其他使用者權限，以與他們共用，如 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

當您與其他使用者共用任何物件時，收件者對其的權利由兩項內容的組合所決定：

* 您授予物件收件者的權限
* 對象類型的收件人的訪問級別設定
