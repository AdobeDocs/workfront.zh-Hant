---
title: 授予對報告、儀表板和行事曆的存取權
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中報告、儀表板和行事曆的存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 授予對報告、儀表板和行事曆的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對報告、控制面板和行事曆的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

此存取權也包含外部頁面的存取權。 如需外部頁面的相關資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

>[!NOTE]
>
>* 如果您想要授予使用者對報告、儀表板和行事曆的存取權，您也必須授予這些使用者對篩選器、檢視和群組的存取權。 如需指示，請參閱[授予篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。
>* 當某人與其他使用者共用報告、儀表板或行事曆時，收件者在該報告上的許可權是由兩個專案的組合所決定：收件者的報告、儀表板和行事曆存取層級設定&#x200B;_以及_&#x200B;共用者授予的報告、儀表板或行事曆的任何許可權
>
>如需使用者在共用報表、儀表板或行事曆時可授與的許可權相關資訊，請參閱[共用報表、儀表板和行事曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用自訂存取層級設定使用者對報告、儀表板和行事曆的存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下報告右側![](assets/gear-icon-settings.png)檢視&#x200B;**或**&#x200B;編輯&#x200B;**按鈕上的齒輪圖示**，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![reports_access.png](assets/reports-access.png)

   預設會啟用下列選項：

   * **建立**
   * **刪除**
   * **檢視內建報告**：必須選取此專案，才能檢視Workfront建置的報告。
   * **共用**
   * **公開共用報告**：可與沒有Workfront帳戶的任何人共用報告的公開連結，以公開共用報告。 必須選取此選項以允許此共用層級。
   * **在整個系統內共用**：可與系統中擁有Workfront授權的所有人共用報告。 必須選取此選項以允許此共用層級。

     如需共用報告、儀表板和行事曆的資訊，請參閱[共用報告、儀表板和行事曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 依授權型別存取報告、儀表板和行事曆

如需有關每個存取層級中的使用者可以對問題執行的資訊，請參閱文章[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports)中的[報告](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)小節。

## 存取共用的報告、儀表板和行事曆

作為報告、儀表板或行事曆的擁有者或建立者，您可以授予其他使用者許可權來共用它，如[共用報告、儀表板和行事曆](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)中所述。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

當您與另一個使用者共用任何物件時，收件者對該物件的權利取決於兩個專案的組合：

* 您授予收件者的物件許可權
* 收件者物件型別的存取層級設定
