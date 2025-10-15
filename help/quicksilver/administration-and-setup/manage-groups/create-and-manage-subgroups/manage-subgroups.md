---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，子群組，編輯
navigation-topic: create-and-manage-subgroups
title: 管理子群組
description: 身為子群組的群組管理員，您可以建立、移動、檢視、編輯、複製、重新命名、匯出及刪除子群組。 您也可以將子群組從父群組中移除，使其成為最上層群組。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# 管理子群組

身為子群組的群組管理員，您可以建立、移動、檢視、編輯、複製、重新命名、匯出及刪除子群組。

您也可以將子群組從父群組中移除，使其成為最上層群組。

如果您的群組之上有任何群組，其管理員也可以為您的群組執行下列動作。 Workfront管理員也是如此（適用於任何群組）。

如需子群組的詳細資訊，請參閱[子群組總覽](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)。

>[!TIP]
>
>當您管理包含子群組的群組時，能夠識別和篩選有關整個群組及其所有子群組的資料會很有幫助。 您可以使用報表或清單中的「頂層父項ID」欄位來達到此目的。
>
>例如，假設您管理一個大型行銷部門，並且想要一個包含整個部門正在處理之所有專案的清單。
>
>在Workfront中，此行銷部門由稱為行銷的群組表示，有3個稱為現場行銷、產品行銷和數位行銷的子群組。 若要列出屬於整個行銷部門（全部4個群組）的專案，您可以使用以下篩選規則為專案區域建立篩選：
>
>`Group: Top Parent ID > Equal > Marketing`
>
>您也可以使用「頂層父項名稱」欄位來識別與頂層群組相關聯的資料，但僅限於檢視中，而非篩選器或群組中。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr>
  <tr> 
   <td>存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立子群組

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下要新增子群組的群組名稱。
1. 在左側功能表中，按一下&#x200B;**子群組**。
1. 若要從您檢視的群組建立新子群組，請按一下[新增子群組]。**&#x200B;**

   或者，如果您想要在清單中另一個子群組下方建立新的子群組，請選取該子群組，然後按一下[新增子群組]。**&#x200B;**

   如需您可以用來設定子群組的選項相關資訊，請參閱[建立子群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

   群組階層不可超過15個層級，但單一層級可以有不限數量的平行群組。

## 移動子群組

您可以將現有的子群組移至您管理的另一個群組下。

群組階層不可超過15個層級，但單一層級可以有不限數量的平行群組。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下目的地群組的名稱（您將在後續步驟中指定要移動的子群組）。
1. 在左側功能表中，按一下&#x200B;**子群組**。
1. （選擇性）選取一個子群組，使其成為目的地群組。

   如果您略過此步驟，您在步驟3中選取的群組就是目的地群組。

1. 按一下&#x200B;**新增子群組>現有群組**。
1. 在出現的&#x200B;**現有群組**&#x200B;方塊中，開始輸入您要移動的子群組名稱。

   顯示的結果不包含目的地群組上方的群組。

   您可以暫留在群組上，並按一下旁邊顯示的資訊圖示![資訊圖示](assets/info-icon.png)，確定您選取的是正確的群組。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。

1. 在清單中找到要移動的子群組時，請選取該子群組的名稱。
1. 針對您要移至目的地群組的任何其他子群組，重複步驟7-8。
1. 按一下「**儲存**」。

## 編輯子群組

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下包含要編輯之子群組的群組名稱。
1. 在左側功能表中，按一下&#x200B;**子群組**。
1. 選取您要編輯的子群組，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

   如需您可以用來設定子群組的選項相關資訊，請參閱[建立子群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

## 複製子群組

>[!NOTE]
>
>只有系統管理員可以複製子群組。

當您複製子群組時，它會變成父群組。 所有群組成員和子群組都會隨其一起複製。 群組成員會保留其在原始群組中的任何指派。

複製子群組時，請考量下列事項：

* 如果您複製的子群組有自己的子群組，它們會包含在複製中，其名稱的格式如下：

  `Original subgroup name (Copy)`

* 屬於公用群組的任何子群組也是公用的，因此任何有權編輯使用者（在群組內或群組外）的使用者都可以將使用者新增至子群組。

若要複製子群組，請執行下列動作：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下包含要複製之子群組的群組名稱。
1. 在左側功能表中，按一下&#x200B;**子群組**。
1. 選取一個子群組，然後按一下&#x200B;**複製**&#x200B;圖示![復製圖示](assets/copy-icon.png)以根據選取的群組建立新的頂層群組。
1. 設定新群組的設定。

   如需這些設定的說明，請參閱[建立群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup)一文中的[複製現有群組或子群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)以建立最上層群組。

1. 按一下&#x200B;**建立群組**。

## 匯出子群組

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下包含要匯出之子群組的群組名稱。
1. 在左側功能表中，按一下&#x200B;**子群組**。
1. 選取要匯出的子群組。
1. 按一下&#x200B;**匯出**&#x200B;圖示![匯出圖示](assets/export.png)，然後選取您要的檔案格式。

## 從子群組的父群組中移除子群組，並將其設為最上層群組

您可以將子群組從父群組中移除，使其成為最上層群組。

>[!TIP]
>
>當您停用下有子群組的群組時，這些子群組也會變成非使用中。 如果您希望其中一個處於作用中狀態，可以使用這些指示將其從父群組中移除，然後重新啟用它。
>&#x200B;>如需停用及重新啟動群組的說明，請參閱[停用或重新啟動群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。
1. 選取要成為最上層群組的子群組的父群組，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。
1. 在出現的&#x200B;**編輯群組**&#x200B;方塊中，開始在&#x200B;**搜尋**&#x200B;欄位（**群組成員和群組管理員**&#x200B;下）中輸入您要成為最上層群組的子群組名稱，然後在其出現時按一下其名稱右側的X。
1. 按一下「**儲存**」。

## 刪除子群組

>[!IMPORTANT]
>
>刪除群組或子群組時，您需要保留使用者、工作專案以及目前指派給該群組的任何子群組。 為了協助您確定它們會被保留，提示會要求您將群組的物件重新指派給不同的群組。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下包含要刪除之子群組的群組名稱。
1. 在左側功能表中，按一下&#x200B;**子群組**。
1. 選取子群組，然後按一下&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)。

   在出現的&#x200B;**刪除群組**&#x200B;方塊中，開始輸入，然後選取您要移動所刪除群組之成員、工作專案及子群組的群組名稱。

1. 按一下&#x200B;**刪除它**。

## 檢視和管理群組的子群組成員

當您檢視所管理群組的首頁時，可以檢視和管理群組子群組中的所有使用者。 如需指示，請參閱[檢視和管理子群組成員](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)。

