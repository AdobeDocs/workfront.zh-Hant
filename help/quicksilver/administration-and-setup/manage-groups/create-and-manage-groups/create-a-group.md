---
user-type: administrator
product-area: system-administration;user-management
keywords: 建立，組，子組，新建
navigation-topic: create-and-manage-groups
title: 建立群組
description: 身為Adobe Workfront管理員，您可以建立群組來組織使用者和專案，以及在Workfront中指派存取權。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# 建立群組

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

身為Adobe Workfront管理員，您可以建立群組來組織使用者和專案，以及在Workfront中指派存取權。 如需詳細資訊，請參閱 [群組概觀](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

每個子組至少需要一個組管理員。 群組管理員可使用「群組」頁面在單一位置管理其群組。

如果您是群組管理員或Workfront管理員，也可以在群組下建立子群組。 如需指示，請參閱 [建立子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 從頭建立頂層群組

這些步驟說明如何從頭建立新群組。 有關通過複製現有組或子組的資訊，請參閱 [複製現有組或子組以建立頂級組](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) 這篇文章。

您必須是Workfront管理員才能建立頂層群組。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 在群組清單上方，按一下 **新組**.

   >[!TIP]
   >
   >在群組清單底部，您也可以按一下 **新增更多群組** 若要內嵌新增群組，請按一下 **輸入** 完成新增群組資訊時。

1. 在 **新組** 方塊中，輸入群組的名稱。
1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">群組名稱</td> 
      <td>變更群組名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入群組的說明。 您最多可以輸入512個字元。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">活動</td> 
      <td> <p>（預設啟用）讓群組在您的Workfront執行個體中處於作用中狀態。</p> <p>在如下所示的預先輸入欄位中，當常規用戶搜索組以將其附加到對象或與其共用對象時，清單中只顯示活動組。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>若要簡化使用者的作業，您可以針對目前未使用的群組停用「作用中」選項。</p> <p>您可以使用此欄位，輕鬆地根據使用中或非使用中狀態檢視、篩選及分組群組清單。 如需在清單中使用檢視、篩選和群組的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報表元素：篩選器、檢視和群組</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將此群組及其子群組設定為公開</td> 
      <td> <p>(只有在查看頂級組（而非子組）的「詳細資訊」時才可用。) 啟用此選項可允許具有編輯用戶訪問權限的組中的用戶（不是組的管理員）將此組及其子組添加到其他用戶的用戶配置檔案中。</p> <p>對於公用群組，任何具有編輯使用者存取權的使用者（進入或退出群組）都可將群組新增至其他使用者的設定檔。 他們無法為私人群組執行此操作。</p> <p>您只能在具有多個層級之群組階層的上層父群組上編輯此選項。 父組的所有子組都會繼承其設定。</p> <p><b>附註</b>:  
        <ul> 
         <li>不能將子組本身設為公用，但可以將其設為頂級父組的公用，這也會使父組的所有子組均為公用。</li> 
         <li>屬於公用組的子組預設為公用組，因此具有編輯用戶訪問權限的任何用戶也可以將該子組添加到其他用戶。</li> 
        </ul> </p> <p>如果您需要編輯使用者所需存取權的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>. 如需編輯使用者的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">業務領導者 </td> 
      <td> <p>您可以將一個使用者指派為您所管理之群組的業務領導者。 業務領導者是為群組做出業務決策的人。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">業務領導者概觀</a><span>.</span></p> <p>如果人員尚未成為組的成員，則將其名稱添加到此欄位也會將其添加到組中。</p> <p><b>附註</b>:  
        <ul> 
         <li>在從組中刪除業務負責人之前，必須從「業務負責人」欄位中刪除其名稱。</li> 
         <li>如果從「業務負責人」欄位中刪除該名稱，則該用戶仍是組的成員，除非從中刪除它們。 如需從群組中移除某人的指示，請參閱區段 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">管理群組成員</a> 在文章中 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">管理群組</a>.</li> 
        </ul> </p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">業務領導者概觀</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組成員和群組管理員</td> 
      <td> 
       <ul> 
        <p>要添加組成員，請開始鍵入要添加的現有用戶或組的名稱，然後在出現時選擇該名稱。</p> 
        <p>您新增的使用者和群組有權存取與群組共用的所有物件。</p>
        <p>頂級組必須至少有一個組管理員。 </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在清單中搜尋人員和群組</td> 
      <td> 如果需要查找已分配給此組的用戶或組，可以在此處鍵入其名稱並在出現時選擇該名稱。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **建立群組**.

## 複製現有組或子組以建立頂級組 {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

身為Workfront管理員，您可以複製現有群組或子群組，以建立新的頂層群組。

要執行此操作時，請記住以下事項：

* 屬於現有組的所有成員和任何子組都將複製到新的頂級組。
* 複製組的成員將保留其在原始組中的分配。 因此，原始組的組管理員也被指定為複製組中的組管理員。

要通過複製組或子組來建立新的頂級組，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

   在隨即顯示的清單中，您可以看到您管理的群組，以及這些群組擁有的任何子群組。 Adobe Workfront管理員可以查看所有群組。

1. 選取您要複製的群組，然後按一下「複製」圖示 ![](assets/copy-icon.png).
1. 在 **複製組** 框，鍵入 **群組名稱** （針對複製的群組）。

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">群組名稱</td> 
      <td>變更群組名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入群組的說明。 您最多可以輸入512個字元。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">活動</td> 
      <td> <p>（預設啟用）讓群組在您的Workfront執行個體中處於作用中狀態。</p> <p>在如下所示的預先輸入欄位中，當常規用戶搜索組以將其附加到對象或與其共用對象時，清單中只顯示活動組。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>若要簡化使用者的作業，您可以針對目前未使用的群組停用「作用中」選項。</p> <p>您可以使用此欄位，輕鬆地根據使用中或非使用中狀態檢視、篩選及分組群組清單。 如需在清單中使用檢視、篩選和群組的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">報表元素：篩選器、檢視和群組</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將此群組及其子群組設定為公開</td> 
      <td> <p>(只有在查看頂級組（而非子組）的「詳細資訊」時才可用。) 啟用此選項可允許具有編輯用戶訪問權限的組中的用戶（不是組的管理員）將此組及其子組添加到其他用戶的用戶配置檔案中。</p> <p>對於公用群組，任何具有編輯使用者存取權的使用者（進入或退出群組）都可將群組新增至其他使用者的設定檔。 他們無法為私人群組執行此操作。</p> <p>您只能在具有多個層級之群組階層的上層父群組上編輯此選項。 父組的所有子組都會繼承其設定。</p> <p><b>附註</b>:  
        <ul> 
         <li>不能將子組本身設為公用，但可以將其設為頂級父組的公用，這也會使父組的所有子組均為公用。</li> 
         <li>屬於公用組的子組預設為公用組，因此具有編輯用戶訪問權限的任何用戶也可以將該子組添加到其他用戶。</li> 
        </ul> </p> <p>如果您需要編輯使用者所需存取權的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">授予使用者存取權</a>. 如需編輯使用者的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">編輯使用者的設定檔</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">業務領導者 </td> 
      <td> <p>您可以將一個使用者指派為您所管理之群組的業務領導者。 業務領導者是為群組做出業務決策的人。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">業務領導者概觀</a><span>.</span></p> <p>如果人員尚未成為組的成員，則將其名稱添加到此欄位也會將其添加到組中。</p> <p><b>附註</b>:  
        <ul> 
         <li>在從組中刪除業務負責人之前，必須從「業務負責人」欄位中刪除其名稱。</li> 
         <li>如果從「業務負責人」欄位中刪除該名稱，則該用戶仍是組的成員，除非從中刪除它們。 如需從群組中移除某人的指示，請參閱區段 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">管理群組成員</a> 在文章中 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">管理群組</a>.</li> 
        </ul> </p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">業務領導者概觀</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組成員和群組管理員</td> 
      <td> 
       <ul> 
        <li> <p>組成員：若要將使用者和群組新增至群組，請開始輸入您要新增的現有使用者或群組名稱，然後在出現時選取名稱。</p> <p>您新增的使用者和群組有權存取與群組共用的所有物件。</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.copied groups">群組管理員：原始組的任何組管理員也被指定為複製組中的組管理員。 您可以使用使用者名稱右側的下拉式功能表，將群組成員指派為群組的管理員。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">頂級組必須至少有1個組管理員。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在清單中搜尋人員和群組</td> 
      <td> 如果需要查找已分配給此組的用戶或組，可以在此處鍵入其名稱並在出現時選擇該名稱。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* 如果原始組具有子組，則子組將添加到新組，預設情況下，其名稱為「原始子組名稱（複製）」。
   >* 通過按一下用戶或子組名稱右側的X，可以從原始組中消除任何用戶或子組。


1. 按一下 **建立群組**.
