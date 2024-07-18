---
user-type: administrator
product-area: system-administration;user-management
keywords: 建立，群組，子群組，新增
navigation-topic: create-and-manage-groups
title: 建立群組
description: 身為Adobe Workfront管理員，您可以建立群組來組織使用者和專案，以及在Workfront中指派存取許可權。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# 建立群組

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

身為Adobe Workfront管理員，您可以建立群組來組織使用者和專案，以及在Workfront中指派存取許可權。 如需詳細資訊，請參閱[群組總覽](../../../administration-and-setup/manage-groups/groups-overview/groups.md)。

每個子群組至少需要一個群組管理員。 群組管理員可以使用「群組」頁面在一個位置管理其群組。

如果您是群組管理員或Workfront管理員，您也可以在群組下建立子群組。 如需指示，請參閱[建立子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授與使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

## 從頭開始建立頂層群組

以下步驟說明如何從頭開始建立新群組。 如需有關複製現有群組或子群組來建立群組或子群組的資訊，請參閱本文中的[複製現有群組或子群組來建立最上層群組](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup)。

您必須是Workfront管理員才能建立頂層群組。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**群組** ![](assets/groups-icon.png)。

1. 在群組清單上方，按一下&#x200B;**新增群組**。

   >[!TIP]
   >
   >在群組清單底部，您也可以按一下[新增更多群組]**以內嵌新增群組，然後在完成新增群組資訊時按一下[輸入]****。**

1. 在顯示的&#x200B;**新群組**&#x200B;方塊中，輸入群組的名稱。
1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">群組名稱</td> 
      <td>變更群組的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入群組的說明。 最多可輸入512個字元。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">為作用中</td> 
      <td> <p>（預設為啟用）在您的Workfront執行個體中啟用群組。</p> <p>在類似下面所示的預先輸入欄位中，當一般使用者搜尋群組以將其附加至物件或與其共用物件時，清單中只會顯示作用中的群組。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>若要簡化使用者的這項作業，您可以停用目前未使用之群組的[作用中]選項。</p> <p>您可以使用此欄位，根據作用中或非作用中狀態輕鬆檢視、篩選及分組群組清單。 如需有關在清單中使用檢視、篩選和群組的資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報告元素：篩選器、檢視和群組</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將此群組及其子群組設定為公開</td> 
      <td> <p>（只有當您檢視最上層群組而非子群組的「詳細資訊」時，才可使用）。 啟用此選項可允許群組中擁有編輯使用者存取許可權的使用者（不是群組的管理員）將此群組及其子群組新增到其他使用者的使用者設定檔中。</p> <p>對於公用群組，任何擁有編輯使用者存取許可權的使用者（在群組內或群組外），都可以將該群組新增到其他使用者的設定檔中。 他們無法為私人群組執行此操作。</p> <p>您只能在具有多個層級的群組階層中的頂層父群組上編輯此選項。 父群組的所有子群組都會繼承其設定。</p> <p><b>附註</b>：  
        <ul> 
         <li>您不能將子群組本身設為公用，但您可以將它的最上層父群組設為公用，這樣也會將父項的所有子群組設為公用。</li> 
         <li>依預設，屬於公用群組的子群組是公用的，因此任何具有編輯使用者存取許可權的使用者也可以將該子群組新增到其他使用者。</li> 
        </ul> </p> <p>如果您需要有關編輯使用者所需存取許可權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>。 如需有關編輯使用者的資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">業務領導者 </td> 
      <td> <p>您可以將一位使用者指派為您管理之群組的業務領導者。 業務主管是負責為群組制定業務決策的人。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">業務負責人概觀</a><span>.</span></p> <p>如果人員不是群組的成員，將其名稱新增至此欄位也會將其新增至群組。</p> <p><b>附註</b>：  
        <ul> 
         <li>您必須先從「業務領導者」欄位中移除其名稱，才能從群組中移除「業務領導者」。</li> 
         <li>如果您從「業務領導者」欄位中移除名稱，除非您將其從群組中移除，否則該使用者仍為群組的成員。 如需從群組移除某人的相關指示，請參閱<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">管理群組</a>一文中的<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">管理群組成員資格</a>小節。</li> 
        </ul> </p> <p>如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">業務負責人概觀</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組成員和群組管理員</td> 
      <td>
        <p>若要新增群組成員，請開始輸入您要新增的現有使用者或群組的名稱，然後在其出現時選取名稱。</p> 
        <p>您新增的使用者和群組可存取與該群組共用的所有物件。</p>
        <p>最上層群組必須至少有一個群組管理員。 </p>
     </tr> 
     <tr> 
      <td role="rowheader">在清單中搜尋人員和群組</td> 
      <td> 如果您需要尋找已指派給此群組的使用者或群組，您可以在此處輸入其名稱，並在其出現時選取它。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**建立群組**。

## 複製現有群組或子群組來建立最上層群組 {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

身為Workfront管理員，您可以複製現有群組或子群組來建立新的頂層群組。

當您要執行此操作時，請記住下列事項：

* 屬於現有群組的所有成員及任何子群組都會複製到新的頂層群組。
* 複製群組的成員會保留其在原始群組中的指派。 因此，原始群組的群組管理員也會被指定為複製群組中的群組管理員。

若要透過複製群組或子群組來建立新的最上層群組：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**群組** ![](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 選取您要複製的群組，然後按一下「複製」圖示![](assets/copy-icon.png)。
1. 在出現的&#x200B;**複製群組**&#x200B;方塊中，輸入複製群組的&#x200B;**群組名稱**。

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">群組名稱</td> 
      <td>變更群組的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入群組的說明。 最多可輸入512個字元。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">為作用中</td> 
      <td> <p>（預設為啟用）在您的Workfront執行個體中啟用群組。</p> <p>在類似下面所示的預先輸入欄位中，當一般使用者搜尋群組以將其附加至物件或與其共用物件時，清單中只會顯示作用中的群組。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>若要簡化使用者的這項作業，您可以停用目前未使用之群組的[作用中]選項。</p> <p>您可以使用此欄位，根據作用中或非作用中狀態輕鬆檢視、篩選及分組群組清單。 如需有關在清單中使用檢視、篩選和群組的資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">報告元素：篩選器、檢視和群組</a>。</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將此群組及其子群組設定為公開</td> 
      <td> <p>（只有當您檢視最上層群組而非子群組的「詳細資訊」時，才可使用）。 啟用此選項可允許群組中擁有編輯使用者存取許可權的使用者（不是群組的管理員）將此群組及其子群組新增到其他使用者的使用者設定檔中。</p> <p>對於公用群組，任何擁有編輯使用者存取許可權的使用者（在群組內或群組外），都可以將該群組新增到其他使用者的設定檔中。 他們無法為私人群組執行此操作。</p> <p>您只能在具有多個層級的群組階層中的頂層父群組上編輯此選項。 父群組的所有子群組都會繼承其設定。</p> <p><b>附註</b>：  
        <ul> 
         <li>您不能將子群組本身設為公用，但您可以將它的最上層父群組設為公用，這樣也會將父項的所有子群組設為公用。</li> 
         <li>依預設，屬於公用群組的子群組是公用的，因此任何具有編輯使用者存取許可權的使用者也可以將該子群組新增到其他使用者。</li> 
        </ul> </p> <p>如果您需要有關編輯使用者所需存取許可權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">授予使用者存取許可權</a>。 如需有關編輯使用者的資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">編輯使用者的設定檔</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">業務領導者 </td> 
      <td> <p>您可以將一位使用者指派為您管理之群組的業務領導者。 業務主管是負責為群組制定業務決策的人。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">業務負責人概觀</a><span>.</span></p> <p>如果人員不是群組的成員，將其名稱新增至此欄位也會將其新增至群組。</p> <p><b>附註</b>：  
        <ul> 
         <li>您必須先從「業務領導者」欄位中移除其名稱，才能從群組中移除「業務領導者」。</li> 
         <li>如果您從「業務領導者」欄位中移除名稱，除非您將其從群組中移除，否則該使用者仍為群組的成員。 如需從群組移除某人的相關指示，請參閱<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">管理群組</a>一文中的<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">管理群組成員資格</a>小節。</li> 
        </ul> </p> <p>如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">業務負責人概觀</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組成員和群組管理員</td> 
      <td> 
       <ul> 
        <li> <p>群組成員：若要新增使用者和群組至群組，請開始輸入您要新增的現有使用者或群組的名稱，然後在其出現時選取名稱。</p> <p>您新增的使用者和群組可存取與該群組共用的所有物件。</p> </li> 
        <li> <p>群組管理員：原始群組的所有群組管理員也會被指定為複製群組中的群組管理員。 您可以使用使用者名稱右側的下拉式功能表，將群組成員指派為群組管理員。</p> <p>最上層群組必須至少有一個群組管理員。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在清單中搜尋人員和群組</td> 
      <td> 如果您需要尋找已指派給此群組的使用者或群組，您可以在此處輸入其名稱，並在其出現時選取它。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* 如果原始群組具有子群組，則子群組會新增至新群組，其名稱預設為「原始子群組名稱（複製）」。
   >* 您可以按一下使用者或子群組名稱右邊的X ，將任何使用者或子群組從原始群組中移除。

1. 按一下&#x200B;**建立群組**。
