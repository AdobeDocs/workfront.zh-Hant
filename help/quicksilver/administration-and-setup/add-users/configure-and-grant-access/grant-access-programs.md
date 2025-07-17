---
title: 授予對計畫的存取權
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中計畫的存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 169f6357-1fbb-43e0-83af-1c4be682ddbf
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# 授予方案存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對程式的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

如需使用自訂存取層級來管理使用者對Workfront中其他物件型別的存取的相關資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

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
   <td>規劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 使用自訂存取層級設定使用者對程式的存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下程式右側![](assets/gear-icon-settings.png)檢視&#x200B;**或**&#x200B;編輯&#x200B;**按鈕上的齒輪圖示**，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![微調程式設定](assets/fine-tune-programs.png)

   如需有關每個存取層級中的使用者可以對程式執行的資訊，請參閱文章[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs)中的[程式](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一節。

   >[!NOTE]
   >
   >當您為特定型別的物件設定存取層級設定時，該設定不會影響使用者存取排名較低的物件。 例如，您可以限制使用者刪除其存取層級的程式，但這不會限制他們刪除排名低於程式的專案。如需物件階層的詳細資訊，請參閱[瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)一文中的[相互依存性和物件階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一節。

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 依授權型別存取計畫

如需有關每個存取層級中的使用者可以對程式執行的資訊，請參閱文章[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs)中的[程式](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一節。

## 存取共用程式

作為方案的擁有者或建立者，您可以授予其他使用者對方案的許可權，以此與其他使用者共用，如[共用方案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md)中所述。

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
