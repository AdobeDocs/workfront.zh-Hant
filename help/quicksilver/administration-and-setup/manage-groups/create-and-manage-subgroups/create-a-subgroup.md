---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: 建立子群組
description: 您可以在管理的群組下建立子群組，以組織使用者和專案，以及在Adobe Workfront中指派存取許可權。 通常，群組管理員會管理群組和子群組。 他們可以利用「群組」頁面，集中管理群組和子群組。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 008f96d52632f5f05554d63ae1c38cc37d21544b
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# 建立子群組

您可以在管理的群組下建立子群組，以組織使用者和專案，以及在Adobe Workfront中指派存取許可權。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

不過，通常群組管理員會管理群組和子群組。 他們可以利用「群組」頁面，集中管理群組和子群組。 若要瞭解群組與子群組在Workfront中的運作方式，請參閱[群組總覽](../../../administration-and-setup/manage-groups/groups-overview/groups.md)與[子群組總覽](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)。

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
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 新增子群組

{{step-1-to-setup}}

1. 按一下&#x200B;**群組**。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 選取要新增子群組的現有群組或子群組。
1. 按一下&#x200B;**新增子群組**。
1. 在出現的&#x200B;**新子群組**&#x200B;方塊中，輸入子群組的&#x200B;**群組名稱**。
1. （選擇性）輸入下列任一資訊：

   * **描述**：輸入子群組的描述。 最多可輸入512個字元。
   * **作用中**：此選項預設為啟用，並使群組在您的Workfront執行個體中作用中。

     在如下所示的預先輸入欄位中，當一般使用者搜尋群組以將其附加到物件或與其共用物件時，清單中只會顯示作用中的群組。

     群組![的](assets/typeahead-for-group.png)自動提示欄位

     若要簡化使用者的這項作業，您可以停用目前未使用之群組的&#x200B;**作用中**&#x200B;選項。

     您可以使用此欄位，根據作用中或非作用中狀態輕鬆檢視、篩選及分組群組清單。 如需有關在清單中使用檢視、篩選和群組的資訊，請參閱[報告元素：篩選器、檢視和群組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   * **業務領導者**：您可以指派一位使用者為您管理的子群組的業務領導者。 業務主管是負責制定子群組業務決策的人。 如需詳細資訊，請參閱[業務負責人概觀](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md)。

     如果人員不是子群組的成員，將他們的名稱新增至此欄位也會將他們新增至群組。

     >[!NOTE]
     >
     >* 您必須先從「業務領導者」欄位中移除其名稱，才能從子群組中移除「業務領導者」。
     >* 如果您從「業務領導者」欄位中移除名稱，除非您將其從子群組中移除，否則該使用者會保留子群組的成員。 如需從群組移除某人的相關指示，請參閱[檢視及管理群組的成員資格](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md)。

   * **群組成員和群組管理員**：若要新增使用者和群組作為子群組的成員，請開始輸入您要新增的現有使用者或群組的名稱，然後在其出現時選取名稱。

     您新增的使用者和群組可存取與該群組共用的所有物件。

     子群組會繼承其上方群組的群組管理員，因此指定使用者作為子群組的群組管理員是選擇性的。 您可以使用使用者名稱右側的下拉式功能表，將群組成員指派為群組管理員。

   * **搜尋清單中的人員和群組**：如果您需要尋找已指派給此子群組的使用者或群組，您可以在此處輸入其名稱，並在它出現時選取它。

1. 按一下&#x200B;**儲存。**
