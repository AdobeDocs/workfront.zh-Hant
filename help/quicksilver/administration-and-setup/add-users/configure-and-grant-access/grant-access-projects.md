---
title: 授予專案存取權
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中專案的存取權。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---

# 授予專案存取權

<!-- Audited: 12/2023 -->

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對專案的存取權，如下列文章所述：
* [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

如需使用自訂存取層級來管理使用者對Workfront中其他物件型別的存取的相關資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 存取需求

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
   <td> <p>新增：標準 </p>
 <p>或</p> 
<p>目前：計畫 </p> 
</td> 
  </tr>

<tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 使用自訂存取層級設定使用者對專案的存取權

1. 開始建立或編輯存取層級，如中所述 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 於 **檢視** 或 **編輯** 按鈕，然後選取您要授與的功能 **微調您的設定**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* 擁有工作授權的使用者擁有有限的專案權利。 他們可以貢獻專案，但無法管理專案。
   >* 擁有「檢閱」授權的使用者擁有轉換問題專案的檢視許可權，但他們的檢視許可權有限。
   >* 如需關於使用者在與他人共用專案時可授與的許可權的資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* 當您為特定型別的物件設定存取層級設定時，該設定不會影響使用者存取排名較低的物件。 例如，您可以限制使用者刪除其存取層級的專案，但這不會限制他們刪除等級低於專案的工作。如需物件階層的詳細資訊，請參閱區段 [物件的相依性和階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. （選用）按一下 **設定共用預設值** 建立選項的右側，然後 **新增規則** 以新增專案的共用規則。

   當具有此存取層級的使用者建立專案時，專案會自動與您於左側選單中選取的使用者共用。

   ![](assets/project-sharing-menu.png)

   在右側的功能表中，您可指定您希望如何與這些使用者共用專案：

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >如果具有此存取層級的使用者使用專案存取範本，範本會覆寫存取層級中的共用設定。 如需有關專案存取範本的資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   您可以重複此步驟，視需要為存取層級新增任意數量的專案共用規則。

1. 按一下X以關閉 **微調您的設定** 方塊。
1. （選擇性）若要為您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續下列其中一篇文章 [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授與任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱 [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 依授權型別存取報告、儀表板和行事曆

如需每個存取層級中的使用者可解決問題的相關資訊，請參閱區段 [專案](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) 在文章中 [適用於每種物件型別的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 共用專案的存取權

作為問題的擁有者或建立者，您可以授予其他使用者許可權來與其共用，如中所述 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

當您與另一個使用者共用任何物件時，收件者對該物件的權利取決於兩個專案的組合：

* 您授予收件者的物件許可權
* 收件者物件型別的存取層級設定
